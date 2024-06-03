# Comparing `tmp/mergify_cli-2024.5.22.8.6.tar.gz` & `tmp/mergify_cli-2024.6.3.8.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergify_cli-2024.5.22.8.6.tar", max compression
+gzip compressed data, was "mergify_cli-2024.6.3.8.29.tar", max compression
```

## Comparing `mergify_cli-2024.5.22.8.6.tar` & `mergify_cli-2024.6.3.8.29.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10143 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/LICENSE
--rw-r--r--   0        0        0     1127 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/README.md
--rwxr-xr-x   0        0        0    27218 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/mergify_cli/__init__.py
--rw-r--r--   0        0        0     1797 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/mergify_cli/hooks/commit-msg
--rw-r--r--   0        0        0        0 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/mergify_cli/tests/__init__.py
--rw-r--r--   0        0        0    18368 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/mergify_cli/tests/test_mergify_cli.py
--rw-r--r--   0        0        0     2558 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/mergify_cli/tests/utils.py
--rw-r--r--   0        0        0     2625 2024-05-22 08:06:58.625818 mergify_cli-2024.5.22.8.6/pyproject.toml
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 mergify_cli-2024.5.22.8.6/PKG-INFO
+-rw-r--r--   0        0        0    10143 2024-06-03 08:29:54.307582 mergify_cli-2024.6.3.8.29/LICENSE
+-rw-r--r--   0        0        0     1127 2024-06-03 08:29:54.307582 mergify_cli-2024.6.3.8.29/README.md
+-rwxr-xr-x   0        0        0    26661 2024-06-03 08:29:54.307582 mergify_cli-2024.6.3.8.29/mergify_cli/__init__.py
+-rw-r--r--   0        0        0     1797 2024-06-03 08:29:54.311582 mergify_cli-2024.6.3.8.29/mergify_cli/hooks/commit-msg
+-rw-r--r--   0        0        0        0 2024-06-03 08:29:54.311582 mergify_cli-2024.6.3.8.29/mergify_cli/tests/__init__.py
+-rw-r--r--   0        0        0    18719 2024-06-03 08:29:54.311582 mergify_cli-2024.6.3.8.29/mergify_cli/tests/test_mergify_cli.py
+-rw-r--r--   0        0        0     2558 2024-06-03 08:29:54.311582 mergify_cli-2024.6.3.8.29/mergify_cli/tests/utils.py
+-rw-r--r--   0        0        0     2625 2024-06-03 08:29:54.311582 mergify_cli-2024.6.3.8.29/pyproject.toml
+-rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 mergify_cli-2024.6.3.8.29/PKG-INFO
```

### Comparing `mergify_cli-2024.5.22.8.6/LICENSE` & `mergify_cli-2024.6.3.8.29/LICENSE`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.5.22.8.6/README.md` & `mergify_cli-2024.6.3.8.29/README.md`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.5.22.8.6/mergify_cli/__init__.py` & `mergify_cli-2024.6.3.8.29/mergify_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,14 @@
 DRAFT_TEMPLATE = 'mutation { convertPullRequestToDraft(input: { pullRequestId: "%s" }) { clientMutationId } }'
 console = rich.console.Console(log_path=False, log_time=False)
 
 DEBUG = False
 TMP_STACK_BRANCH = "mergify-cli-tmp"
 
 
-def check_for_graphql_errors(response: httpx.Response) -> None:
-    data = response.json()
-    if "errors" in data:
-        console.print(f"url: {response.request.url}", style="red")
-        console.print(f"data: {response.request.content.decode()}", style="red")
-        if "errors" in data:
-            console.print(
-                "\n".join(f"* {e.get('message') or e}" for e in data["errors"]),
-                style="red",
-            )
-        sys.exit(1)
-
-
 def check_for_status(response: httpx.Response) -> None:
     if response.status_code < 400:
         return
 
     if response.status_code < 500:
         data = response.json()
         console.print(f"url: {response.request.url}", style="red")
@@ -400,41 +387,14 @@
                 },
             )
             check_for_status(r)
             pull = typing.cast(PullRequest, r.json())
     return pull, action
 
 
-async def check_and_update_pull_status(
-    client: httpx.AsyncClient,
-    pull: PullRequest,
-    create_as_draft: bool,
-) -> str:
-    if create_as_draft:
-        action = "draft"
-        template = DRAFT_TEMPLATE
-    else:
-        action = "ready_for_review"
-        template = READY_FOR_REVIEW_TEMPLATE
-
-    r = await client.post(
-        "https://api.github.com/graphql",
-        headers={
-            "Accept": "application/vnd.github.v4.idl",
-            "User-Agent": f"mergify_cli/{VERSION}",
-            "Authorization": client.headers["Authorization"],
-        },
-        json={"query": template % pull["node_id"]},
-    )
-    check_for_status(r)
-    check_for_graphql_errors(r)
-
-    return action
-
-
 async def delete_stack(
     client: httpx.AsyncClient,
     stack_prefix: str,
     changeid: ChangeId,
     known_changeids: KnownChangeIDs,
 ) -> None:
     r = await client.delete(
@@ -527,14 +487,15 @@
         msg = "Local branch is a branch generated by Mergify CLI"
         raise LocalBranchInvalidError(msg)
 
 
 # TODO(charly): fix code to conform to linter (number of arguments, local
 # variables, statements, positional arguments, branches)
 async def stack(  # noqa: PLR0913, PLR0914, PLR0915, PLR0917, PLR0912
+    github_server: str,
     token: str,
     skip_rebase: bool,
     next_only: bool,
     branch_prefix: str,
     dry_run: bool,
     trunk: tuple[str, str],
     create_as_draft: bool = False,
@@ -596,15 +557,15 @@
 
     if DEBUG:
         event_hooks = {"request": [log_httpx_request], "response": [log_httpx_response]}
     else:
         event_hooks = {}
 
     async with httpx.AsyncClient(
-        base_url=f"https://api.github.com/repos/{user}/{repo}/",
+        base_url=f"{github_server}/repos/{user}/{repo}/",
         headers={
             "Accept": "application/vnd.github.v3+json",
             "User-Agent": f"mergify_cli/{VERSION}",
             "Authorization": f"token {token}",
         },
         event_hooks=event_hooks,  # type: ignore[arg-type]
         follow_redirects=True,
@@ -722,14 +683,30 @@
 
 def GitHubToken(v: str) -> str:  # noqa: N802
     if not v:
         raise ValueError
     return v
 
 
+async def get_default_github_server() -> str:
+    try:
+        result = await git("config", "--get", "mergify-cli.github-server")
+    except CommandError:
+        result = ""
+
+    url = parse.urlparse(result or "https://api.github.com/")
+    url = url._replace(scheme="https")
+
+    if url.hostname == "api.github.com":
+        url = url._replace(path="")
+    else:
+        url = url._replace(path="/api/v3")
+    return url.geturl()
+
+
 async def get_default_branch_prefix() -> str:
     try:
         result = await git("config", "--get", "mergify-cli.stack-branch-prefix")
     except CommandError:
         result = ""
 
     return result or "mergify_cli"
@@ -761,14 +738,15 @@
 
 async def stack_main(args: argparse.Namespace) -> None:
     if args.setup:
         await do_setup()
         return
 
     await stack(
+        args.github_server,
         args.token,
         args.skip_rebase,
         args.next_only,
         args.branch_prefix,
         args.dry_run,
         args.trunk,
         args.draft,
@@ -789,14 +767,19 @@
     parser.add_argument(
         "--token",
         default=await get_default_token(),
         type=GitHubToken,
         help="GitHub personal access token",
     )
     parser.add_argument("--dry-run", "-n", action="store_true")
+    parser.add_argument(
+        "--github-server",
+        action="store_true",
+        default=await get_default_github_server(),
+    )
     sub_parsers = parser.add_subparsers(dest="action")
 
     stack_parser = sub_parsers.add_parser(
         "stack",
         description="Stacked Pull Requests CLI",
         help="Create a pull requests stack",
     )
```

### Comparing `mergify_cli-2024.5.22.8.6/mergify_cli/hooks/commit-msg` & `mergify_cli-2024.6.3.8.29/mergify_cli/hooks/commit-msg`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.5.22.8.6/mergify_cli/tests/test_mergify_cli.py` & `mergify_cli-2024.6.3.8.29/mergify_cli/tests/test_mergify_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     )
     respx_mock.get("/repos/user/repo/issues/2/comments").respond(200, json=[])
     post_comment2_mock = respx_mock.post("/repos/user/repo/issues/2/comments").respond(
         200,
     )
 
     await mergify_cli.stack(
+        github_server="https://api.github.com/",
         token="",
         skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
@@ -285,14 +286,15 @@
             "draft": False,
             "node_id": "",
         },
     )
     respx_mock.get("/repos/user/repo/issues/1/comments").respond(200, json=[])
 
     await mergify_cli.stack(
+        github_server="https://api.github.com/",
         token="",
         skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
@@ -361,14 +363,15 @@
                 "url": "https://api.github.com/repos/user/repo/issues/comments/456",
             },
         ],
     )
     respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
 
     await mergify_cli.stack(
+        github_server="https://api.github.com/",
         token="",
         skip_rebase=True,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
@@ -437,14 +440,15 @@
                 "url": "https://api.github.com/repos/user/repo/issues/comments/456",
             },
         ],
     )
     respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
 
     await mergify_cli.stack(
+        github_server="https://api.github.com/",
         token="",
         skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
     )
@@ -514,14 +518,15 @@
                 "url": "https://api.github.com/repos/user/repo/issues/comments/456",
             },
         ],
     )
     respx_mock.patch("/repos/user/repo/issues/comments/456").respond(200)
 
     await mergify_cli.stack(
+        github_server="https://api.github.com/",
         token="",
         skip_rebase=False,
         next_only=False,
         branch_prefix="",
         dry_run=False,
         trunk=("origin", "main"),
         keep_pull_request_title_and_body=True,
@@ -540,14 +545,15 @@
 async def test_stack_on_destination_branch_raises_an_error(
     git_mock: test_utils.GitMock,
 ) -> None:
     git_mock.mock("rev-parse", "--abbrev-ref", "HEAD", output="main")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
+            github_server="https://api.github.com/",
             token="",
             skip_rebase=False,
             next_only=False,
             branch_prefix="",
             dry_run=False,
             trunk=("origin", "main"),
         )
@@ -557,14 +563,15 @@
 async def test_stack_without_common_commit_raises_an_error(
     git_mock: test_utils.GitMock,
 ) -> None:
     git_mock.mock("merge-base", "--fork-point", "origin/main", output="")
 
     with pytest.raises(SystemExit, match="1"):
         await mergify_cli.stack(
+            github_server="https://api.github.com/",
             token="",
             skip_rebase=False,
             next_only=False,
             branch_prefix="",
             dry_run=False,
             trunk=("origin", "main"),
         )
```

### Comparing `mergify_cli-2024.5.22.8.6/mergify_cli/tests/utils.py` & `mergify_cli-2024.6.3.8.29/mergify_cli/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.5.22.8.6/pyproject.toml` & `mergify_cli-2024.6.3.8.29/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [tool.poetry-version-plugin]
 source = "git-tag"
 
 [tool.poetry.group.dev.dependencies]
 mypy = {version = ">=0.930"}
 mypy-extensions = "^1.0.0"
-ruff = ">=0.0.277,<0.4.5"
+ruff = ">=0.0.277,<0.4.8"
 pytest = {version = ">=6.2.5"}
 poethepoet = ">=0.21,<0.27"
 pytest-asyncio = "^0.23.2"
 respx = ">=0.20.2,<0.22.0"
 types-aiofiles = "^23.2.0.20240106"
 
 [tool.poetry.scripts]
```

### Comparing `mergify_cli-2024.5.22.8.6/PKG-INFO` & `mergify_cli-2024.6.3.8.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergify_cli
-Version: 2024.5.22.8.6
+Version: 2024.6.3.8.29
 Summary: Mergify CLI is a tool that automates the creation and management of stacked pull requests on GitHub
 License: Apache License
 Author: Mehdi Abaakouk
 Author-email: sileht@mergify.com
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

