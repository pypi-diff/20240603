# Comparing `tmp/git_cliff-2.2.2.tar.gz` & `tmp/git_cliff-2.3.0.tar.gz`

## Comparing `git_cliff-2.2.2.tar` & `git_cliff-2.3.0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0     1001      127     2366 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/Cargo.toml
--rw-r--r--   0     1001      127    22801 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/changelog.rs
--rw-r--r--   0     1001      127     2068 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/command.rs
--rw-r--r--   0     1001      127    18530 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/commit.rs
--rw-r--r--   0     1001      127    10306 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/config.rs
--rw-r--r--   0     1001      127     1617 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/embed.rs
--rw-r--r--   0     1001      127     4909 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/error.rs
--rw-r--r--   0     1001      127     7528 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/github.rs
--rw-r--r--   0     1001      127     1278 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/lib.rs
--rw-r--r--   0     1001      127    18124 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/release.rs
--rw-r--r--   0     1001      127     7621 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/repo.rs
--rw-r--r--   0     1001      127     6235 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/src/template.rs
--rw-r--r--   0     1001      127     7500 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff-core/tests/integration_test.rs
--rw-r--r--   0     1001      127     5927 2024-05-11 20:02:07.000000 git_cliff-2.2.2/README.md
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 git_cliff-2.2.2/git-cliff/Cargo.toml
--rw-r--r--   0     1001      127     8460 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/args.rs
--rw-r--r--   0     1001      127      701 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/bin/completions.rs
--rw-r--r--   0     1001      127      754 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/bin/mangen.rs
--rw-r--r--   0     1001      127    13842 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/lib.rs
--rw-r--r--   0     1001      127     3408 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/logger.rs
--rw-r--r--   0     1001      127      546 2024-05-11 20:02:07.000000 git_cliff-2.2.2/git-cliff/src/main.rs
--rw-r--r--   0     1001      127    80522 2024-05-11 20:02:07.000000 git_cliff-2.2.2/Cargo.lock
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 git_cliff-2.2.2/Cargo.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 git_cliff-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 git_cliff-2.2.2/PKG-INFO
+-rw-r--r--   0     1001      127     2927 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/Cargo.toml
+-rw-r--r--   0     1001      127    28194 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/changelog.rs
+-rw-r--r--   0     1001      127     2068 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/command.rs
+-rw-r--r--   0     1001      127    18891 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/commit.rs
+-rw-r--r--   0     1001      127    10457 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/config.rs
+-rw-r--r--   0     1001      127     1617 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/embed.rs
+-rw-r--r--   0     1001      127     5053 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/error.rs
+-rw-r--r--   0     1001      127     1355 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/lib.rs
+-rw-r--r--   0     1001      127    27545 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/release.rs
+-rw-r--r--   0     1001      127     5958 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/remote/bitbucket.rs
+-rw-r--r--   0     1001      127     4253 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/remote/github.rs
+-rw-r--r--   0     1001      127     6679 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/remote/gitlab.rs
+-rw-r--r--   0     1001      127     9770 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/remote/mod.rs
+-rw-r--r--   0     1001      127     7621 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/repo.rs
+-rw-r--r--   0     1001      127     6482 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/src/template.rs
+-rw-r--r--   0     1001      127     7996 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff-core/tests/integration_test.rs
+-rw-r--r--   0     1001      127     5927 2024-06-03 11:19:31.000000 git_cliff-2.3.0/README.md
+-rw-r--r--   0        0        0     3351 1970-01-01 00:00:00.000000 git_cliff-2.3.0/git-cliff/Cargo.toml
+-rw-r--r--   0     1001      127     9451 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/args.rs
+-rw-r--r--   0     1001      127      701 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/bin/completions.rs
+-rw-r--r--   0     1001      127      754 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/bin/mangen.rs
+-rw-r--r--   0     1001      127    15513 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/lib.rs
+-rw-r--r--   0     1001      127     4378 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/logger.rs
+-rw-r--r--   0     1001      127      546 2024-06-03 11:19:31.000000 git_cliff-2.3.0/git-cliff/src/main.rs
+-rw-r--r--   0     1001      127    80730 2024-06-03 11:19:31.000000 git_cliff-2.3.0/Cargo.lock
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 git_cliff-2.3.0/Cargo.toml
+-rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 git_cliff-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 git_cliff-2.3.0/PKG-INFO
```

### Comparing `git_cliff-2.2.2/git-cliff-core/Cargo.toml` & `git_cliff-2.3.0/git-cliff-core/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "git-cliff-core"
-version = "2.2.2" # managed by release.sh
+version = "2.3.0" # managed by release.sh
 description = "Core library of git-cliff"
 authors = ["git-cliff contributors <git-cliff@protonmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "../README.md"
 homepage = "https://github.com/orhun/git-cliff"
 repository = "https://github.com/orhun/git-cliff"
 keywords = ["changelog", "generator", "conventional", "commit"]
@@ -23,46 +23,67 @@
 github = [
   "dep:reqwest",
   "dep:http-cache-reqwest",
   "dep:reqwest-middleware",
   "dep:tokio",
   "dep:futures",
 ]
+## Enable integration with GitLab.
+## You can turn this off if you don't use GitLab and don't want
+## to make network requests to the GitLab API.
+gitlab = [
+  "dep:reqwest",
+  "dep:http-cache-reqwest",
+  "dep:reqwest-middleware",
+  "dep:tokio",
+  "dep:futures",
+]
+## Enable integration with Bitbucket.
+## You can turn this off if you don't use Bitbucket and don't want
+## to make network requests to the Bitbucket API.
+bitbucket = [
+  "dep:reqwest",
+  "dep:http-cache-reqwest",
+  "dep:reqwest-middleware",
+  "dep:tokio",
+  "dep:futures",
+]
 
 [dependencies]
 glob = { workspace = true, optional = true }
 regex.workspace = true
 log.workspace = true
 secrecy.workspace = true
 dirs.workspace = true
 lazy_static.workspace = true
-thiserror = "1.0.60"
-serde = { version = "1.0.201", features = ["derive"] }
+thiserror = "1.0.61"
+serde = { version = "1.0.203", features = ["derive"] }
 serde_json = "1.0.117"
 serde_regex = "1.1.0"
-tera = "1.19.1"
+tera = "1.20.0"
 indexmap = { version = "2.2.6", optional = true }
-toml = "0.8.12"
+toml = "0.8.13"
 lazy-regex = "3.1.0"
-next_version = "0.2.16"
+next_version = "0.2.17"
 semver = "1.0.23"
 document-features = { version = "0.2.8", optional = true }
 reqwest = { version = "0.12.4", default-features = false, features = [
   "rustls-tls",
   "json",
   "zstd",
 ], optional = true }
 http-cache-reqwest = { version = "0.14.0", optional = true }
 reqwest-middleware = { version = "0.3.1", optional = true }
-tokio = { version = "1.37.0", features = [
+tokio = { version = "1.38.0", features = [
   "rt-multi-thread",
   "macros",
 ], optional = true }
 futures = { version = "0.3.30", optional = true }
 url = "2.5.0"
+dyn-clone = "1.0.17"
 
 [dependencies.git2]
 version = "0.18.3"
 default-features = false
 optional = true
 
 [dependencies.config]
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/changelog.rs` & `git_cliff-2.3.0/git-cliff-core/src/changelog.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 use crate::commit::Commit;
 use crate::config::{
 	Config,
 	GitConfig,
 };
 use crate::error::Result;
-#[cfg(feature = "github")]
-use crate::github::{
-	GitHubClient,
-	GitHubCommit,
-	GitHubPullRequest,
-	FINISHED_FETCHING_MSG,
-	START_FETCHING_MSG,
-};
 use crate::release::{
 	Release,
 	Releases,
 };
+#[cfg(feature = "bitbucket")]
+use crate::remote::bitbucket::BitbucketClient;
+#[cfg(feature = "github")]
+use crate::remote::github::GitHubClient;
+#[cfg(feature = "gitlab")]
+use crate::remote::gitlab::GitLabClient;
 use crate::template::Template;
 use std::collections::HashMap;
 use std::io::Write;
 use std::time::{
 	SystemTime,
 	UNIX_EPOCH,
 };
@@ -194,40 +192,167 @@
 	///
 	/// Each of these are paginated requests so they are being run in parallel
 	/// for speedup.
 	///
 	/// If no GitHub related variable is used in the template then this function
 	/// returns empty vectors.
 	#[cfg(feature = "github")]
-	fn get_github_metadata(
-		&self,
-	) -> Result<(Vec<GitHubCommit>, Vec<GitHubPullRequest>)> {
-		if self.body_template.contains_github_variable() ||
+	fn get_github_metadata(&self) -> Result<crate::remote::RemoteMetadata> {
+		use crate::remote::github;
+		if self
+			.body_template
+			.contains_variable(github::TEMPLATE_VARIABLES) ||
 			self.footer_template
 				.as_ref()
-				.map(|v| v.contains_github_variable())
+				.map(|v| v.contains_variable(github::TEMPLATE_VARIABLES))
 				.unwrap_or(false)
 		{
 			warn!("You are using an experimental feature! Please report bugs at <https://git-cliff.org/issues>");
 			let github_client =
 				GitHubClient::try_from(self.config.remote.github.clone())?;
-			info!("{START_FETCHING_MSG} ({})", self.config.remote.github);
+			info!(
+				"{} ({})",
+				github::START_FETCHING_MSG,
+				self.config.remote.github
+			);
 			let data = tokio::runtime::Builder::new_multi_thread()
 				.enable_all()
 				.build()?
 				.block_on(async {
 					let (commits, pull_requests) = tokio::try_join!(
 						github_client.get_commits(),
 						github_client.get_pull_requests(),
 					)?;
 					debug!("Number of GitHub commits: {}", commits.len());
 					debug!("Number of GitHub pull requests: {}", commits.len());
 					Ok((commits, pull_requests))
 				});
-			info!("{FINISHED_FETCHING_MSG}");
+			info!("{}", github::FINISHED_FETCHING_MSG);
+			data
+		} else {
+			Ok((vec![], vec![]))
+		}
+	}
+
+	/// Returns the GitLab metadata needed for the changelog.
+	///
+	/// This function creates a multithread async runtime for handling the
+	///
+	/// requests. The following are fetched from the GitLab REST API:
+	///
+	/// - Commits
+	/// - Marge requests
+	///
+	/// Each of these are paginated requests so they are being run in parallel
+	/// for speedup.
+	///
+	///
+	/// If no GitLab related variable is used in the template then this function
+	/// returns empty vectors.
+	#[cfg(feature = "gitlab")]
+	fn get_gitlab_metadata(&self) -> Result<crate::remote::RemoteMetadata> {
+		use crate::remote::gitlab;
+		if self
+			.body_template
+			.contains_variable(gitlab::TEMPLATE_VARIABLES) ||
+			self.footer_template
+				.as_ref()
+				.map(|v| v.contains_variable(gitlab::TEMPLATE_VARIABLES))
+				.unwrap_or(false)
+		{
+			warn!("You are using an experimental feature! Please report bugs at <https://git-cliff.org/issues>");
+			let gitlab_client =
+				GitLabClient::try_from(self.config.remote.gitlab.clone())?;
+			info!(
+				"{} ({})",
+				gitlab::START_FETCHING_MSG,
+				self.config.remote.gitlab
+			);
+			let data = tokio::runtime::Builder::new_multi_thread()
+				.enable_all()
+				.build()?
+				.block_on(async {
+					// Map repo/owner to gitlab id
+					let project_id = match tokio::join!(gitlab_client.get_project())
+					{
+						(Ok(project),) => project.id,
+						(Err(err),) => {
+							error!("Failed to lookup project! {}", err);
+							return Err(err);
+						}
+					};
+					let (commits, merge_requests) = tokio::try_join!(
+						// Send id to these functions
+						gitlab_client.get_commits(project_id),
+						gitlab_client.get_merge_requests(project_id),
+					)?;
+					debug!("Number of GitLab commits: {}", commits.len());
+					debug!(
+						"Number of GitLab merge requests: {}",
+						merge_requests.len()
+					);
+					Ok((commits, merge_requests))
+				});
+			info!("{}", gitlab::FINISHED_FETCHING_MSG);
+			data
+		} else {
+			Ok((vec![], vec![]))
+		}
+	}
+
+	/// Returns the Bitbucket metadata needed for the changelog.
+	///
+	/// This function creates a multithread async runtime for handling the
+	///
+	/// requests. The following are fetched from the bitbucket REST API:
+	///
+	/// - Commits
+	/// - Pull requests
+	///
+	/// Each of these are paginated requests so they are being run in parallel
+	/// for speedup.
+	///
+	///
+	/// If no bitbucket related variable is used in the template then this
+	/// function returns empty vectors.
+	#[cfg(feature = "bitbucket")]
+	fn get_bitbucket_metadata(&self) -> Result<crate::remote::RemoteMetadata> {
+		use crate::remote::bitbucket;
+		if self
+			.body_template
+			.contains_variable(bitbucket::TEMPLATE_VARIABLES) ||
+			self.footer_template
+				.as_ref()
+				.map(|v| v.contains_variable(bitbucket::TEMPLATE_VARIABLES))
+				.unwrap_or(false)
+		{
+			warn!("You are using an experimental feature! Please report bugs at <https://git-cliff.org/issues>");
+			let bitbucket_client =
+				BitbucketClient::try_from(self.config.remote.bitbucket.clone())?;
+			info!(
+				"{} ({})",
+				bitbucket::START_FETCHING_MSG,
+				self.config.remote.bitbucket
+			);
+			let data = tokio::runtime::Builder::new_multi_thread()
+				.enable_all()
+				.build()?
+				.block_on(async {
+					let (commits, pull_requests) = tokio::try_join!(
+						bitbucket_client.get_commits(),
+						bitbucket_client.get_pull_requests()
+					)?;
+					debug!("Number of Bitbucket commits: {}", commits.len());
+					debug!(
+						"Number of Bitbucket pull requests: {}",
+						pull_requests.len()
+					);
+					Ok((commits, pull_requests))
+				});
+			info!("{}", bitbucket::FINISHED_FETCHING_MSG);
 			data
 		} else {
 			Ok((vec![], vec![]))
 		}
 	}
 
 	/// Increments the version for the unreleased changes based on semver.
@@ -253,15 +378,35 @@
 		debug!("Generating changelog...");
 		let mut additional_context = self.additional_context.clone();
 		additional_context.insert(
 			"remote".to_string(),
 			serde_json::to_value(self.config.remote.clone())?,
 		);
 		#[cfg(feature = "github")]
-		let (github_commits, github_pull_requests) = self.get_github_metadata()?;
+		let (github_commits, github_pull_requests) = if self.config.remote.github.is_set() {
+			self.get_github_metadata()
+				.expect("Could not get github metadata")
+		} else {
+			(vec![], vec![])
+		};
+		#[cfg(feature = "gitlab")]
+		let (gitlab_commits, gitlab_merge_request) = if self.config.remote.gitlab.is_set() {
+			self.get_gitlab_metadata()
+				.expect("Could not get gitlab metadata")
+		} else {
+			(vec![], vec![])
+		};
+		#[cfg(feature = "bitbucket")]
+		let (bitbucket_commits, bitbucket_pull_request) =
+			if self.config.remote.bitbucket.is_set() {
+				self.get_bitbucket_metadata()
+					.expect("Could not get bitbucket metadata")
+			} else {
+				(vec![], vec![])
+			};
 		let postprocessors = self
 			.config
 			.changelog
 			.postprocessors
 			.clone()
 			.unwrap_or_default();
 		if let Some(header) = &self.config.changelog.header {
@@ -275,14 +420,24 @@
 		let mut releases = self.releases.clone();
 		for release in releases.iter_mut() {
 			#[cfg(feature = "github")]
 			release.update_github_metadata(
 				github_commits.clone(),
 				github_pull_requests.clone(),
 			)?;
+			#[cfg(feature = "gitlab")]
+			release.update_gitlab_metadata(
+				gitlab_commits.clone(),
+				gitlab_merge_request.clone(),
+			)?;
+			#[cfg(feature = "bitbucket")]
+			release.update_bitbucket_metadata(
+				bitbucket_commits.clone(),
+				bitbucket_pull_request.clone(),
+			)?;
 			let write_result = write!(
 				out,
 				"{}",
 				self.body_template.render(
 					&release,
 					Some(&additional_context),
 					&postprocessors
@@ -513,15 +668,25 @@
 				ignore_tags:              None,
 				topo_order:               Some(false),
 				sort_commits:             Some(String::from("oldest")),
 				link_parsers:             None,
 				limit_commits:            None,
 			},
 			remote:    RemoteConfig {
-				github: Remote {
+				github:    Remote {
+					owner: String::from("coolguy"),
+					repo:  String::from("awesome"),
+					token: None,
+				},
+				gitlab:    Remote {
+					owner: String::from("coolguy"),
+					repo:  String::from("awesome"),
+					token: None,
+				},
+				bitbucket: Remote {
 					owner: String::from("coolguy"),
 					repo:  String::from("awesome"),
 					token: None,
 				},
 			},
 			bump:      Bump::default(),
 		};
@@ -585,15 +750,23 @@
 					String::from("revert(app): skip this commit"),
 				),
 			],
 			commit_id: Some(String::from("0bc123")),
 			timestamp: 50000000,
 			previous: None,
 			#[cfg(feature = "github")]
-			github: crate::github::GitHubReleaseMetadata {
+			github: crate::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "gitlab")]
+			gitlab: crate::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "bitbucket")]
+			bitbucket: crate::remote::RemoteReleaseMetadata {
 				contributors: vec![],
 			},
 		};
 		let releases = vec![
 			test_release.clone(),
 			Release {
 				version: Some(String::from("v3.0.0")),
@@ -632,15 +805,23 @@
 						String::from("revert(app): skip this commit"),
 					),
 				],
 				commit_id: None,
 				timestamp: 1000,
 				previous: Some(Box::new(test_release)),
 				#[cfg(feature = "github")]
-				github: crate::github::GitHubReleaseMetadata {
+				github: crate::remote::RemoteReleaseMetadata {
+					contributors: vec![],
+				},
+				#[cfg(feature = "gitlab")]
+				gitlab: crate::remote::RemoteReleaseMetadata {
+					contributors: vec![],
+				},
+				#[cfg(feature = "bitbucket")]
+				bitbucket: crate::remote::RemoteReleaseMetadata {
 					contributors: vec![],
 				},
 			},
 		];
 		(config, releases)
 	}
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/command.rs` & `git_cliff-2.3.0/git-cliff-core/src/command.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff-core/src/commit.rs` & `git_cliff-2.3.0/git-cliff-core/src/commit.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 	LinkParser,
 	TextProcessor,
 };
 use crate::error::{
 	Error as AppError,
 	Result,
 };
-#[cfg(feature = "github")]
-use crate::github::GitHubContributor;
 #[cfg(feature = "repo")]
 use git2::{
 	Commit as GitCommit,
 	Signature as CommitSignature,
 };
 use git_conventional::{
 	Commit as ConventionalCommit,
@@ -122,15 +120,21 @@
 	pub author:        Signature,
 	/// Committer.
 	pub committer:     Signature,
 	/// Whether if the commit has two or more parents.
 	pub merge_commit:  bool,
 	/// GitHub metadata of the commit.
 	#[cfg(feature = "github")]
-	pub github:        GitHubContributor,
+	pub github:        crate::remote::RemoteContributor,
+	/// GitLab metadata of the commit.
+	#[cfg(feature = "gitlab")]
+	pub gitlab:        crate::remote::RemoteContributor,
+	/// Bitbucket metadata of the commit.
+	#[cfg(feature = "bitbucket")]
+	pub bitbucket:     crate::remote::RemoteContributor,
 }
 
 impl<'a> From<String> for Commit<'a> {
 	fn from(message: String) -> Self {
 		if let Some(captures) = SHA1_REGEX.captures(&message) {
 			if let (Some(id), Some(message)) = (
 				captures.get(1).map(|v| v.as_str()),
@@ -436,14 +440,18 @@
 		commit.serialize_field("links", &self.links)?;
 		commit.serialize_field("author", &self.author)?;
 		commit.serialize_field("committer", &self.committer)?;
 		commit.serialize_field("conventional", &self.conv.is_some())?;
 		commit.serialize_field("merge_commit", &self.merge_commit)?;
 		#[cfg(feature = "github")]
 		commit.serialize_field("github", &self.github)?;
+		#[cfg(feature = "gitlab")]
+		commit.serialize_field("gitlab", &self.gitlab)?;
+		#[cfg(feature = "bitbucket")]
+		commit.serialize_field("bitbucket", &self.bitbucket)?;
 		commit.end()
 	}
 }
 
 #[cfg(test)]
 mod test {
 	use super::*;
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/config.rs` & `git_cliff-2.3.0/git-cliff-core/src/config.rs`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,22 @@
 	pub limit_commits:            Option<usize>,
 }
 
 /// Remote configuration.
 #[derive(Default, Debug, Clone, Serialize, Deserialize)]
 pub struct RemoteConfig {
 	/// GitHub remote.
-	pub github: Remote,
+	#[serde(default)]
+	pub github:    Remote,
+	/// GitLab remote.
+	#[serde(default)]
+	pub gitlab:    Remote,
+	/// Bitbucket remote.
+	#[serde(default)]
+	pub bitbucket: Remote,
 }
 
 /// A single remote.
 #[derive(Debug, Default, Clone, Serialize, Deserialize)]
 pub struct Remote {
 	/// Owner of the remote.
 	pub owner: String,
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/embed.rs` & `git_cliff-2.3.0/git-cliff-core/src/embed.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff-core/src/error.rs` & `git_cliff-2.3.0/git-cliff-core/src/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -73,25 +73,25 @@
 	FieldError(String),
 	/// Error that may occur while parsing a SemVer version or version
 	/// requirement.
 	#[error("Semver error: `{0}`")]
 	SemverError(#[from] semver::Error),
 	/// The errors that may occur when processing a HTTP request.
 	#[error("HTTP client error: `{0}`")]
-	#[cfg(feature = "github")]
+	#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
 	HttpClientError(#[from] reqwest::Error),
 	/// The errors that may occur while constructing the HTTP client with
 	/// middleware.
 	#[error("HTTP client with middleware error: `{0}`")]
-	#[cfg(feature = "github")]
+	#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
 	HttpClientMiddlewareError(#[from] reqwest_middleware::Error),
 	/// A possible error when converting a HeaderValue from a string or byte
 	/// slice.
 	#[error("HTTP header error: `{0}`")]
-	#[cfg(feature = "github")]
+	#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
 	HttpHeaderError(#[from] reqwest::header::InvalidHeaderValue),
 	/// Error that may occur during handling pages.
 	#[error("Pagination error: `{0}`")]
 	PaginationError(String),
 	/// The errors that may occur while parsing URLs.
 	#[error("URL parse error: `{0}`")]
 	UrlParseError(#[from] url::ParseError),
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/github.rs` & `git_cliff-2.3.0/git-cliff-core/src/remote/mod.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+/// GitHub client.
+#[cfg(feature = "github")]
+pub mod github;
+
+/// GitLab client.
+#[cfg(feature = "gitlab")]
+pub mod gitlab;
+
+/// Bitbucket client.
+#[cfg(feature = "bitbucket")]
+pub mod bitbucket;
+
 use crate::config::Remote;
-use crate::error::*;
+use crate::error::{
+	Error,
+	Result,
+};
+use dyn_clone::DynClone;
 use futures::{
 	future,
 	stream,
 	StreamExt,
 };
 use http_cache_reqwest::{
 	CACacheManager,
@@ -23,223 +39,190 @@
 };
 use secrecy::ExposeSecret;
 use serde::de::DeserializeOwned;
 use serde::{
 	Deserialize,
 	Serialize,
 };
-use std::env;
 use std::hash::{
 	Hash,
 	Hasher,
 };
 use std::time::Duration;
 
-/// GitHub REST API url.
-const GITHUB_API_URL: &str = "https://api.github.com";
-
-/// Environment variable for overriding the GitHub REST API url.
-const GITHUB_API_URL_ENV: &str = "GITHUB_API_URL";
-
 /// User agent for interacting with the GitHub API.
 ///
 /// This is needed since GitHub API does not accept empty user agent.
-const USER_AGENT: &str = concat!(env!("CARGO_PKG_NAME"), env!("CARGO_PKG_VERSION"));
+pub(crate) const USER_AGENT: &str =
+	concat!(env!("CARGO_PKG_NAME"), env!("CARGO_PKG_VERSION"));
 
 /// Request timeout value in seconds.
-const REQUEST_TIMEOUT: u64 = 30;
+pub(crate) const REQUEST_TIMEOUT: u64 = 30;
 
 /// TCP keeplive value in seconds.
-const REQUEST_KEEP_ALIVE: u64 = 60;
+pub(crate) const REQUEST_KEEP_ALIVE: u64 = 60;
 
 /// Maximum number of entries to fetch in a single page.
-const MAX_PAGE_SIZE: usize = 100;
-
-/// Log message to show while fetching data from GitHub.
-pub const START_FETCHING_MSG: &str = "Retrieving data from GitHub...";
-
-/// Log message to show when done fetching from GitHub.
-pub const FINISHED_FETCHING_MSG: &str = "Done fetching GitHub data.";
-
-/// Returns the GitHub API url either from environment or from default value.
-fn get_github_api_url() -> String {
-	env::var(GITHUB_API_URL_ENV)
-		.ok()
-		.unwrap_or_else(|| GITHUB_API_URL.to_string())
-}
+pub(crate) const MAX_PAGE_SIZE: usize = 100;
 
-/// Trait for handling the different entries returned from the GitHub API.
-trait GitHubEntry {
+/// Trait for handling the different entries returned from the remote.
+pub trait RemoteEntry {
 	/// Returns the API URL for fetching the entries at the specified page.
-	fn url(owner: &str, repo: &str, page: i32) -> String;
+	fn url(project_id: i64, api_url: &str, remote: &Remote, page: i32) -> String;
 	/// Returns the request buffer size.
 	fn buffer_size() -> usize;
+	/// Whether if exit early.
+	fn early_exit(&self) -> bool;
 }
 
-/// Representation of a single commit.
-#[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
-pub struct GitHubCommit {
-	/// SHA.
-	pub sha:    String,
-	/// Author of the commit.
-	pub author: Option<GitHubCommitAuthor>,
-}
-
-impl GitHubEntry for GitHubCommit {
-	fn url(owner: &str, repo: &str, page: i32) -> String {
-		format!(
-			"{}/repos/{}/{}/commits?per_page={MAX_PAGE_SIZE}&page={page}",
-			get_github_api_url(),
-			owner,
-			repo
-		)
-	}
-	fn buffer_size() -> usize {
-		10
-	}
-}
-
-/// Author of the commit.
-#[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
-pub struct GitHubCommitAuthor {
-	/// Username.
-	pub login: Option<String>,
-}
-
-/// Label of the pull request.
-#[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
-#[serde(rename_all = "camelCase")]
-pub struct PullRequestLabel {
-	/// Name of the label.
-	pub name: String,
-}
-
-/// Representation of a single pull request.
-#[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
-pub struct GitHubPullRequest {
-	/// Pull request number.
-	pub number:           i64,
-	/// Pull request title.
-	pub title:            Option<String>,
-	/// SHA of the merge commit.
-	pub merge_commit_sha: Option<String>,
+/// Trait for handling remote commits.
+pub trait RemoteCommit: DynClone {
+	/// Commit SHA.
+	fn id(&self) -> String;
+	/// Commit author.
+	fn username(&self) -> Option<String>;
+}
+
+dyn_clone::clone_trait_object!(RemoteCommit);
+
+/// Trait for handling remote pull requests.
+pub trait RemotePullRequest: DynClone {
+	/// Number.
+	fn number(&self) -> i64;
+	/// Title.
+	fn title(&self) -> Option<String>;
 	/// Labels of the pull request.
-	pub labels:           Vec<PullRequestLabel>,
+	fn labels(&self) -> Vec<String>;
+	/// Merge commit SHA.
+	fn merge_commit(&self) -> Option<String>;
 }
 
-impl GitHubEntry for GitHubPullRequest {
-	fn url(owner: &str, repo: &str, page: i32) -> String {
-		format!(
-			"{}/repos/{}/{}/pulls?per_page={MAX_PAGE_SIZE}&page={page}&state=closed",
-			get_github_api_url(),
-			owner,
-			repo
-		)
-	}
+dyn_clone::clone_trait_object!(RemotePullRequest);
 
-	fn buffer_size() -> usize {
-		5
-	}
-}
+/// Result of a remote metadata.
+pub type RemoteMetadata =
+	(Vec<Box<dyn RemoteCommit>>, Vec<Box<dyn RemotePullRequest>>);
 
-/// Metadata of a GitHub release.
+/// Metadata of a remote release.
 #[derive(Debug, Default, Clone, Eq, PartialEq, Deserialize, Serialize)]
-pub struct GitHubReleaseMetadata {
+pub struct RemoteReleaseMetadata {
 	/// Contributors.
-	pub contributors: Vec<GitHubContributor>,
+	pub contributors: Vec<RemoteContributor>,
 }
 
-/// Representation of a GitHub contributor.
+/// Representation of a remote contributor.
 #[derive(Debug, Default, Clone, Eq, PartialEq, Deserialize, Serialize)]
-pub struct GitHubContributor {
+pub struct RemoteContributor {
 	/// Username.
 	pub username:      Option<String>,
 	/// Title of the pull request.
 	pub pr_title:      Option<String>,
 	/// The pull request that the user created.
 	pub pr_number:     Option<i64>,
 	/// Labels of the pull request.
 	pub pr_labels:     Vec<String>,
 	/// Whether if the user contributed for the first time.
 	pub is_first_time: bool,
 }
 
-impl Hash for GitHubContributor {
+impl Hash for RemoteContributor {
 	fn hash<H: Hasher>(&self, state: &mut H) {
 		self.username.hash(state);
 	}
 }
 
-/// HTTP client for handling GitHub REST API requests.
-#[derive(Debug, Clone)]
-pub struct GitHubClient {
-	/// Owner of the repository.
-	owner:  String,
-	/// GitHub repository.
-	repo:   String,
-	/// HTTP client.
-	client: ClientWithMiddleware,
-}
-
-/// Constructs a GitHub client from the remote configuration.
-impl TryFrom<Remote> for GitHubClient {
-	type Error = Error;
-	fn try_from(remote: Remote) -> Result<Self> {
-		if !remote.is_set() {
-			return Err(Error::RemoteNotSetError);
-		}
-		let mut headers = HeaderMap::new();
+/// Creates a HTTP client for the remote.
+fn create_remote_client(
+	remote: &Remote,
+	accept_header: &str,
+) -> Result<ClientWithMiddleware> {
+	if !remote.is_set() {
+		return Err(Error::RemoteNotSetError);
+	}
+	let mut headers = HeaderMap::new();
+	headers.insert(
+		reqwest::header::ACCEPT,
+		HeaderValue::from_str(accept_header)?,
+	);
+	if let Some(token) = &remote.token {
 		headers.insert(
-			reqwest::header::ACCEPT,
-			HeaderValue::from_static("application/vnd.github+json"),
+			reqwest::header::AUTHORIZATION,
+			format!("Bearer {}", token.expose_secret()).parse()?,
 		);
-		if let Some(token) = remote.token {
-			headers.insert(
-				reqwest::header::AUTHORIZATION,
-				format!("Bearer {}", token.expose_secret()).parse()?,
-			);
-		}
-		headers.insert(reqwest::header::USER_AGENT, USER_AGENT.parse()?);
-		let client = Client::builder()
-			.timeout(Duration::from_secs(REQUEST_TIMEOUT))
-			.tcp_keepalive(Duration::from_secs(REQUEST_KEEP_ALIVE))
-			.default_headers(headers)
-			.build()?;
-		let client = ClientBuilder::new(client)
-			.with(Cache(HttpCache {
-				mode:    CacheMode::Default,
-				manager: CACacheManager {
-					path: dirs::cache_dir()
-						.ok_or_else(|| {
-							Error::DirsError(String::from(
-								"failed to find the user's cache directory",
-							))
-						})?
-						.join(env!("CARGO_PKG_NAME")),
-				},
-				options: HttpCacheOptions::default(),
-			}))
-			.build();
-		Ok(Self {
-			owner: remote.owner,
-			repo: remote.repo,
-			client,
-		})
 	}
-}
+	headers.insert(reqwest::header::USER_AGENT, USER_AGENT.parse()?);
+	let client = Client::builder()
+		.timeout(Duration::from_secs(REQUEST_TIMEOUT))
+		.tcp_keepalive(Duration::from_secs(REQUEST_KEEP_ALIVE))
+		.default_headers(headers)
+		.build()?;
+	let client = ClientBuilder::new(client)
+		.with(Cache(HttpCache {
+			mode:    CacheMode::Default,
+			manager: CACacheManager {
+				path: dirs::cache_dir()
+					.ok_or_else(|| {
+						Error::DirsError(String::from(
+							"failed to find the user's cache directory",
+						))
+					})?
+					.join(env!("CARGO_PKG_NAME")),
+			},
+			options: HttpCacheOptions::default(),
+		}))
+		.build();
+	Ok(client)
+}
+
+/// Trait for handling the API connection and fetching.
+pub trait RemoteClient {
+	/// Returns the API url.
+	fn api_url() -> String;
+
+	/// Returns the remote repository information.
+	fn remote(&self) -> Remote;
+
+	/// Returns the HTTP client for making requests.
+	fn client(&self) -> ClientWithMiddleware;
+
+	/// Returns true if the client should early exit.
+	fn early_exit<T: DeserializeOwned + RemoteEntry>(&self, page: &T) -> bool {
+		page.early_exit()
+	}
+
+	/// Retrieves a single object.
+	async fn get_entry<T: DeserializeOwned + RemoteEntry>(
+		&self,
+		project_id: i64,
+		page: i32,
+	) -> Result<T> {
+		let url = T::url(project_id, &Self::api_url(), &self.remote(), page);
+		debug!("Sending request to: {url}");
+		let response = self.client().get(&url).send().await?;
+		let response_text = if response.status().is_success() {
+			let text = response.text().await?;
+			trace!("Response: {:?}", text);
+			text
+		} else {
+			let text = response.text().await?;
+			error!("Request error: {}", text);
+			text
+		};
+		Ok(serde_json::from_str::<T>(&response_text)?)
+	}
 
-impl GitHubClient {
 	/// Retrieves a single page of entries.
-	async fn get_entries_with_page<T: DeserializeOwned + GitHubEntry>(
+	async fn get_entries_with_page<T: DeserializeOwned + RemoteEntry>(
 		&self,
+		project_id: i64,
 		page: i32,
 	) -> Result<Vec<T>> {
-		let url = T::url(&self.owner, &self.repo, page);
+		let url = T::url(project_id, &Self::api_url(), &self.remote(), page);
 		debug!("Sending request to: {url}");
-		let response = self.client.get(&url).send().await?;
+		let response = self.client().get(&url).send().await?;
 		let response_text = if response.status().is_success() {
 			let text = response.text().await?;
 			trace!("Response: {:?}", text);
 			text
 		} else {
 			let text = response.text().await?;
 			error!("Request error: {}", text);
@@ -249,18 +232,23 @@
 		if response.is_empty() {
 			Err(Error::PaginationError(String::from("end of entries")))
 		} else {
 			Ok(response)
 		}
 	}
 
-	/// Fetches the GitHub API returns the given entry.
-	async fn fetch<T: DeserializeOwned + GitHubEntry>(&self) -> Result<Vec<T>> {
-		let entries: Vec<Vec<T>> = stream::iter(1..)
-			.map(|i| self.get_entries_with_page(i))
+	/// Fetches the remote API and returns the given entry.
+	///
+	/// See `fetch_with_early_exit` for the early exit version of this method.
+	async fn fetch<T: DeserializeOwned + RemoteEntry>(
+		&self,
+		project_id: i64,
+	) -> Result<Vec<T>> {
+		let entries: Vec<Vec<T>> = stream::iter(0..)
+			.map(|i| self.get_entries_with_page(project_id, i))
 			.buffered(T::buffer_size())
 			.take_while(|page| {
 				if let Err(e) = page {
 					debug!("Error while fetching page: {:?}", e);
 				}
 				future::ready(page.is_ok())
 			})
@@ -272,17 +260,109 @@
 				}
 			})
 			.collect()
 			.await;
 		Ok(entries.into_iter().flatten().collect())
 	}
 
-	/// Fetches the GitHub API and returns the commits.
-	pub async fn get_commits(&self) -> Result<Vec<GitHubCommit>> {
-		self.fetch::<GitHubCommit>().await
+	/// Fetches the remote API and returns the given entry.
+	///
+	/// Early exits based on the response.
+	async fn fetch_with_early_exit<T: DeserializeOwned + RemoteEntry>(
+		&self,
+		project_id: i64,
+	) -> Result<Vec<T>> {
+		let entries: Vec<T> = stream::iter(0..)
+			.map(|i| self.get_entry::<T>(project_id, i))
+			.buffered(T::buffer_size())
+			.take_while(|page| {
+				let status = match page {
+					Ok(v) => !self.early_exit(v),
+					Err(e) => {
+						debug!("Error while fetching page: {:?}", e);
+						true
+					}
+				};
+				future::ready(status && page.is_ok())
+			})
+			.map(|page| match page {
+				Ok(v) => v,
+				Err(ref e) => {
+					log::error!("{:#?}", e);
+					page.expect("failed to fetch page: {}")
+				}
+			})
+			.collect()
+			.await;
+		Ok(entries)
 	}
+}
 
-	/// Fetches the GitHub API and returns the pull requests.
-	pub async fn get_pull_requests(&self) -> Result<Vec<GitHubPullRequest>> {
-		self.fetch::<GitHubPullRequest>().await
-	}
+/// Generates a function for updating the release metadata for a remote.
+#[doc(hidden)]
+#[macro_export]
+macro_rules! update_release_metadata {
+	($remote: ident, $fn: ident) => {
+		impl<'a> Release<'a> {
+			/// Updates the remote metadata that is contained in the release.
+			///
+			/// This function takes two arguments:
+			///
+			/// - Commits: needed for associating the Git user with the GitHub
+			///   username.
+			/// - Pull requests: needed for generating the contributor list for the
+			///   release.
+			pub fn $fn(
+				&mut self,
+				mut commits: Vec<Box<dyn RemoteCommit>>,
+				pull_requests: Vec<Box<dyn RemotePullRequest>>,
+			) -> Result<()> {
+				let mut contributors: Vec<RemoteContributor> = Vec::new();
+				// retain the commits that are not a part of this release for later
+				// on checking the first contributors.
+				commits.retain(|v| {
+					if let Some(commit) =
+						self.commits.iter_mut().find(|commit| commit.id == v.id())
+					{
+						let pull_request = pull_requests
+							.iter()
+							.find(|pr| pr.merge_commit() == Some(v.id().clone()));
+						commit.$remote.username = v.username();
+						commit.$remote.pr_number = pull_request.map(|v| v.number());
+						commit.$remote.pr_title =
+							pull_request.and_then(|v| v.title().clone());
+						commit.$remote.pr_labels = pull_request
+							.map(|v| v.labels().clone())
+							.unwrap_or_default();
+						if !contributors
+							.iter()
+							.any(|v| commit.$remote.username == v.username)
+						{
+							contributors.push(RemoteContributor {
+								username:      commit.$remote.username.clone(),
+								pr_title:      commit.$remote.pr_title.clone(),
+								pr_number:     commit.$remote.pr_number,
+								pr_labels:     commit.$remote.pr_labels.clone(),
+								is_first_time: false,
+							});
+						}
+						false
+					} else {
+						true
+					}
+				});
+				// mark contributors as first-time
+				self.$remote.contributors = contributors
+					.into_iter()
+					.map(|mut v| {
+						v.is_first_time = !commits
+							.iter()
+							.map(|v| v.username())
+							.any(|login| login == v.username);
+						v
+					})
+					.collect();
+				Ok(())
+			}
+		}
+	};
 }
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/lib.rs` & `git_cliff-2.3.0/git-cliff-core/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 pub mod commit;
 /// Config file parser.
 pub mod config;
 /// Embedded file handler.
 pub mod embed;
 /// Error handling.
 pub mod error;
-/// GitHub client.
-#[cfg(feature = "github")]
-pub mod github;
 /// Common release type.
 pub mod release;
-#[cfg(feature = "repo")]
+/// Remote handler.
+#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
+#[allow(async_fn_in_trait)]
+pub mod remote;
 /// Git repository.
+#[cfg(feature = "repo")]
 pub mod repo;
 /// Template engine.
 pub mod template;
 
 #[macro_use]
 extern crate log;
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/release.rs` & `git_cliff-2.3.0/git-cliff-core/src/release.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 use crate::commit::Commit;
 use crate::config::Bump;
 use crate::error::Result;
-#[cfg(feature = "github")]
-use crate::github::{
-	GitHubCommit,
-	GitHubContributor,
-	GitHubPullRequest,
-	GitHubReleaseMetadata,
+#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
+use crate::remote::{
+	RemoteCommit,
+	RemoteContributor,
+	RemotePullRequest,
+	RemoteReleaseMetadata,
 };
 use next_version::VersionUpdater;
 use semver::Version;
 use serde::{
 	Deserialize,
 	Serialize,
 };
@@ -28,80 +28,33 @@
 	pub commit_id: Option<String>,
 	/// Timestamp of the release in seconds, from epoch.
 	pub timestamp: i64,
 	/// Previous release.
 	pub previous:  Option<Box<Release<'a>>>,
 	/// Contributors.
 	#[cfg(feature = "github")]
-	pub github:    GitHubReleaseMetadata,
+	pub github:    RemoteReleaseMetadata,
+	/// Contributors.
+	#[cfg(feature = "gitlab")]
+	pub gitlab:    RemoteReleaseMetadata,
+	/// Contributors.
+	#[cfg(feature = "bitbucket")]
+	pub bitbucket: RemoteReleaseMetadata,
 }
 
-impl<'a> Release<'a> {
-	/// Updates the GitHub metadata that is contained in the release.
-	///
-	/// This function takes two arguments:
-	///
-	/// - GitHub commits: needed for associating the Git user with the GitHub
-	///   username.
-	/// - GitHub pull requests: needed for generating the contributor list for
-	///   the release.
-	#[cfg(feature = "github")]
-	pub fn update_github_metadata(
-		&mut self,
-		mut github_commits: Vec<GitHubCommit>,
-		github_pull_requests: Vec<GitHubPullRequest>,
-	) -> Result<()> {
-		let mut contributors: Vec<GitHubContributor> = Vec::new();
-		// retain the commits that are not a part of this release for later on
-		// checking the first contributors.
-		github_commits.retain(|v| {
-			if let Some(commit) =
-				self.commits.iter_mut().find(|commit| commit.id == v.sha)
-			{
-				let pull_request = github_pull_requests
-					.iter()
-					.find(|pr| pr.merge_commit_sha == Some(v.sha.clone()));
+#[cfg(feature = "github")]
+crate::update_release_metadata!(github, update_github_metadata);
 
-				commit.github.username = v.author.clone().and_then(|v| v.login);
-				commit.github.pr_number = pull_request.map(|v| v.number);
-				commit.github.pr_title = pull_request.and_then(|v| v.title.clone());
-				commit.github.pr_labels = pull_request
-					.map(|v| v.labels.iter().map(|v| v.name.clone()).collect())
-					.unwrap_or_default();
-				if !contributors
-					.iter()
-					.any(|v| commit.github.username == v.username)
-				{
-					contributors.push(GitHubContributor {
-						username:      commit.github.username.clone(),
-						pr_title:      commit.github.pr_title.clone(),
-						pr_number:     commit.github.pr_number,
-						pr_labels:     commit.github.pr_labels.clone(),
-						is_first_time: false,
-					});
-				}
-				false
-			} else {
-				true
-			}
-		});
-		// mark contributors as first-time
-		self.github.contributors = contributors
-			.into_iter()
-			.map(|mut v| {
-				v.is_first_time = !github_commits
-					.iter()
-					.map(|v| v.author.clone().and_then(|v| v.login))
-					.any(|login| login == v.username);
-				v
-			})
-			.collect();
-		Ok(())
-	}
+#[cfg(feature = "gitlab")]
+crate::update_release_metadata!(gitlab, update_gitlab_metadata);
+
+#[cfg(feature = "bitbucket")]
+crate::update_release_metadata!(bitbucket, update_bitbucket_metadata);
 
+impl<'a> Release<'a> {
 	/// Calculates the next version based on the commits.
 	///
 	/// It uses the default bump version configuration to calculate the next
 	/// version.
 	pub fn calculate_next_version(&self) -> Result<String> {
 		self.calculate_next_version_with_config(&Bump::default())
 	}
@@ -198,15 +151,23 @@
 				commit_id: None,
 				timestamp: 0,
 				previous: Some(Box::new(Release {
 					version: Some(String::from(version)),
 					..Default::default()
 				})),
 				#[cfg(feature = "github")]
-				github: crate::github::GitHubReleaseMetadata {
+				github: crate::remote::RemoteReleaseMetadata {
+					contributors: vec![],
+				},
+				#[cfg(feature = "gitlab")]
+				gitlab: crate::remote::RemoteReleaseMetadata {
+					contributors: vec![],
+				},
+				#[cfg(feature = "bitbucket")]
+				bitbucket: crate::remote::RemoteReleaseMetadata {
 					contributors: vec![],
 				},
 			}
 		}
 
 		let test_shared = [
 			("1.0.0", "1.1.0", vec!["feat: add xyz", "fix: fix xyz"]),
@@ -343,16 +304,20 @@
 		}
 		Ok(())
 	}
 
 	#[cfg(feature = "github")]
 	#[test]
 	fn update_github_metadata() -> Result<()> {
-		use crate::github::GitHubCommitAuthor;
-		use crate::github::PullRequestLabel;
+		use crate::remote::github::{
+			GitHubCommit,
+			GitHubCommitAuthor,
+			GitHubPullRequest,
+			PullRequestLabel,
+		};
 
 		let mut release = Release {
 			version:   None,
 			commits:   vec![
 				Commit::from(String::from(
 					"1d244937ee6ceb8e0314a4a201ba93a7a61f2071 add github \
 					 integration",
@@ -376,15 +341,21 @@
 			],
 			commit_id: None,
 			timestamp: 0,
 			previous:  Some(Box::new(Release {
 				version: Some(String::from("1.0.0")),
 				..Default::default()
 			})),
-			github:    GitHubReleaseMetadata {
+			github:    RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			gitlab:    RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			bitbucket: RemoteReleaseMetadata {
 				contributors: vec![],
 			},
 		};
 		release.update_github_metadata(
 			vec![
 				GitHubCommit {
 					sha:    String::from("1d244937ee6ceb8e0314a4a201ba93a7a61f2071"),
@@ -432,15 +403,18 @@
 					sha:    String::from("kk34967147560e809658776d4901709139b4ad68"),
 					author: None,
 				},
 				GitHubCommit {
 					sha:    String::new(),
 					author: None,
 				},
-			],
+			]
+			.into_iter()
+			.map(|v| Box::new(v) as Box<dyn RemoteCommit>)
+			.collect(),
 			vec![
 				GitHubPullRequest {
 					title:            Some(String::from("1")),
 					number:           42,
 					merge_commit_sha: Some(String::from(
 						"1d244937ee6ceb8e0314a4a201ba93a7a61f2071",
 					)),
@@ -484,81 +458,84 @@
 					merge_commit_sha: Some(String::from(
 						"5a55e92e5a62dc5bf9872ffb2566959fad98bd05",
 					)),
 					labels:           vec![PullRequestLabel {
 						name: String::from("github"),
 					}],
 				},
-			],
+			]
+			.into_iter()
+			.map(|v| Box::new(v) as Box<dyn RemotePullRequest>)
+			.collect(),
 		)?;
 		let expected_commits = vec![
 			Commit {
 				id: String::from("1d244937ee6ceb8e0314a4a201ba93a7a61f2071"),
 				message: String::from("add github integration"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("orhun")),
 					pr_title:      Some(String::from("1")),
 					pr_number:     Some(42),
 					pr_labels:     vec![String::from("rust")],
 					is_first_time: false,
 				},
 				..Default::default()
 			},
 			Commit {
 				id: String::from("21f6aa587fcb772de13f2fde0e92697c51f84162"),
 				message: String::from("fix github integration"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("orhun")),
 					pr_title:      Some(String::from("2")),
 					pr_number:     Some(66),
 					pr_labels:     vec![String::from("rust")],
 					is_first_time: false,
 				},
 				..Default::default()
 			},
 			Commit {
 				id: String::from("35d8c6b6329ecbcf131d7df02f93c3bbc5ba5973"),
 				message: String::from("update metadata"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("nuhro")),
 					pr_title:      Some(String::from("3")),
 					pr_number:     Some(53),
 					pr_labels:     vec![String::from("deps")],
 					is_first_time: false,
 				},
 				..Default::default()
 			},
 			Commit {
 				id: String::from("4d3ffe4753b923f4d7807c490e650e6624a12074"),
 				message: String::from("do some stuff"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("awesome_contributor")),
 					pr_title:      Some(String::from("4")),
 					pr_number:     Some(1000),
 					pr_labels:     vec![String::from("deps")],
 					is_first_time: false,
 				},
 				..Default::default()
 			},
 			Commit {
 				id: String::from("5a55e92e5a62dc5bf9872ffb2566959fad98bd05"),
 				message: String::from("alright"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("orhun")),
 					pr_title:      Some(String::from("5")),
 					pr_number:     Some(999999),
 					pr_labels:     vec![String::from("github")],
 					is_first_time: false,
 				},
 				..Default::default()
 			},
 			Commit {
 				id: String::from("6c34967147560ea09658776d4901709139b4ad66"),
 				message: String::from("should be fine"),
-				github: GitHubContributor {
+				github: RemoteContributor {
 					username:      Some(String::from("someone")),
 					pr_title:      None,
 					pr_number:     None,
 					pr_labels:     vec![],
 					is_first_time: false,
 				},
 				..Default::default()
@@ -567,44 +544,380 @@
 		assert_eq!(expected_commits, release.commits);
 
 		release
 			.github
 			.contributors
 			.sort_by(|a, b| a.pr_number.cmp(&b.pr_number));
 
-		let expected_metadata = GitHubReleaseMetadata {
+		let expected_metadata = RemoteReleaseMetadata {
 			contributors: vec![
-				GitHubContributor {
+				RemoteContributor {
 					username:      Some(String::from("someone")),
 					pr_title:      None,
 					pr_number:     None,
 					pr_labels:     vec![],
 					is_first_time: true,
 				},
-				GitHubContributor {
+				RemoteContributor {
 					username:      Some(String::from("orhun")),
 					pr_title:      Some(String::from("1")),
 					pr_number:     Some(42),
 					pr_labels:     vec![String::from("rust")],
 					is_first_time: true,
 				},
-				GitHubContributor {
+				RemoteContributor {
 					username:      Some(String::from("nuhro")),
 					pr_title:      Some(String::from("3")),
 					pr_number:     Some(53),
 					pr_labels:     vec![String::from("deps")],
 					is_first_time: true,
 				},
-				GitHubContributor {
+				RemoteContributor {
 					username:      Some(String::from("awesome_contributor")),
 					pr_title:      Some(String::from("4")),
 					pr_number:     Some(1000),
 					pr_labels:     vec![String::from("deps")],
 					is_first_time: true,
 				},
 			],
 		};
 		assert_eq!(expected_metadata, release.github);
 
 		Ok(())
 	}
+
+	#[cfg(feature = "gitlab")]
+	#[test]
+	fn update_gitlab_metadata() -> Result<()> {
+		use crate::remote::gitlab::{
+			GitLabCommit,
+			GitLabMergeRequest,
+			GitLabUser,
+		};
+
+		let mut release = Release {
+			version:   None,
+			commits:   vec![
+				Commit::from(String::from(
+					"1d244937ee6ceb8e0314a4a201ba93a7a61f2071 add github \
+					 integration",
+				)),
+				Commit::from(String::from(
+					"21f6aa587fcb772de13f2fde0e92697c51f84162 fix github \
+					 integration",
+				)),
+				Commit::from(String::from(
+					"35d8c6b6329ecbcf131d7df02f93c3bbc5ba5973 update metadata",
+				)),
+				Commit::from(String::from(
+					"4d3ffe4753b923f4d7807c490e650e6624a12074 do some stuff",
+				)),
+				Commit::from(String::from(
+					"5a55e92e5a62dc5bf9872ffb2566959fad98bd05 alright",
+				)),
+				Commit::from(String::from(
+					"6c34967147560ea09658776d4901709139b4ad66 should be fine",
+				)),
+			],
+			commit_id: None,
+			timestamp: 0,
+			previous:  Some(Box::new(Release {
+				version: Some(String::from("1.0.0")),
+				..Default::default()
+			})),
+			github:    RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			gitlab:    RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			bitbucket: RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+		};
+		release.update_gitlab_metadata(
+			vec![
+				GitLabCommit {
+					id:              String::from(
+						"1d244937ee6ceb8e0314a4a201ba93a7a61f2071",
+					),
+					author_name:     String::from("orhun"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"21f6aa587fcb772de13f2fde0e92697c51f84162",
+					),
+					author_name:     String::from("orhun"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"35d8c6b6329ecbcf131d7df02f93c3bbc5ba5973",
+					),
+					author_name:     String::from("nuhro"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"4d3ffe4753b923f4d7807c490e650e6624a12074",
+					),
+					author_name:     String::from("awesome_contributor"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"5a55e92e5a62dc5bf9872ffb2566959fad98bd05",
+					),
+					author_name:     String::from("orhun"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"6c34967147560ea09658776d4901709139b4ad66",
+					),
+					author_name:     String::from("someone"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"0c34967147560e809658776d4901709139b4ad68",
+					),
+					author_name:     String::from("idk"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+				GitLabCommit {
+					id:              String::from(
+						"kk34967147560e809658776d4901709139b4ad68",
+					),
+					author_name:     String::from("orhun"),
+					short_id:        String::from(""),
+					title:           String::from(""),
+					author_email:    String::from(""),
+					authored_date:   String::from(""),
+					committer_name:  String::from(""),
+					committer_email: String::from(""),
+					committed_date:  String::from(""),
+					created_at:      String::from(""),
+					message:         String::from(""),
+					parent_ids:      vec![],
+					web_url:         String::from(""),
+				},
+			]
+			.into_iter()
+			.map(|v| Box::new(v) as Box<dyn RemoteCommit>)
+			.collect(),
+			vec![Box::new(GitLabMergeRequest {
+				title:             String::from("1"),
+				merge_commit_sha:  Some(String::from(
+					"1d244937ee6ceb8e0314a4a201ba93a7a61f2071",
+				)),
+				id:                1,
+				iid:               1,
+				project_id:        1,
+				description:       String::from(""),
+				state:             String::from(""),
+				created_at:        String::from(""),
+				author:            GitLabUser {
+					id:         1,
+					name:       String::from("42"),
+					username:   String::from("42"),
+					state:      String::from("42"),
+					avatar_url: None,
+					web_url:    String::from("42"),
+				},
+				sha:               String::from(
+					"1d244937ee6ceb8e0314a4a201ba93a7a61f2071",
+				),
+				web_url:           String::from(""),
+				squash_commit_sha: None,
+				labels:            vec![String::from("rust")],
+			})],
+		)?;
+		let expected_commits = vec![
+			Commit {
+				id: String::from("1d244937ee6ceb8e0314a4a201ba93a7a61f2071"),
+				message: String::from("add github integration"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("orhun")),
+					pr_title:      Some(String::from("1")),
+					pr_number:     Some(1),
+					pr_labels:     vec![String::from("rust")],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+			Commit {
+				id: String::from("21f6aa587fcb772de13f2fde0e92697c51f84162"),
+				message: String::from("fix github integration"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("orhun")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+			Commit {
+				id: String::from("35d8c6b6329ecbcf131d7df02f93c3bbc5ba5973"),
+				message: String::from("update metadata"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("nuhro")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+			Commit {
+				id: String::from("4d3ffe4753b923f4d7807c490e650e6624a12074"),
+				message: String::from("do some stuff"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("awesome_contributor")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+			Commit {
+				id: String::from("5a55e92e5a62dc5bf9872ffb2566959fad98bd05"),
+				message: String::from("alright"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("orhun")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+			Commit {
+				id: String::from("6c34967147560ea09658776d4901709139b4ad66"),
+				message: String::from("should be fine"),
+				gitlab: RemoteContributor {
+					username:      Some(String::from("someone")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: false,
+				},
+				..Default::default()
+			},
+		];
+		assert_eq!(expected_commits, release.commits);
+
+		release
+			.github
+			.contributors
+			.sort_by(|a, b| a.pr_number.cmp(&b.pr_number));
+
+		let expected_metadata = RemoteReleaseMetadata {
+			contributors: vec![
+				RemoteContributor {
+					username:      Some(String::from("orhun")),
+					pr_title:      Some(String::from("1")),
+					pr_number:     Some(1),
+					pr_labels:     vec![String::from("rust")],
+					is_first_time: false,
+				},
+				RemoteContributor {
+					username:      Some(String::from("nuhro")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: true,
+				},
+				RemoteContributor {
+					username:      Some(String::from("awesome_contributor")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: true,
+				},
+				RemoteContributor {
+					username:      Some(String::from("someone")),
+					pr_title:      None,
+					pr_number:     None,
+					pr_labels:     vec![],
+					is_first_time: true,
+				},
+			],
+		};
+		assert_eq!(expected_metadata, release.gitlab);
+
+		Ok(())
+	}
 }
```

### Comparing `git_cliff-2.2.2/git-cliff-core/src/repo.rs` & `git_cliff-2.3.0/git-cliff-core/src/repo.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff-core/src/template.rs` & `git_cliff-2.3.0/git-cliff-core/src/template.rs`

 * *Files 7% similar despite different names*

```diff
@@ -127,23 +127,20 @@
 		let ast = &tera.get_template("template")?.ast;
 		for node in ast {
 			Self::find_identifiers(node, &mut variables);
 		}
 		Ok(variables.into_iter().collect())
 	}
 
-	/// Returns `true` if the template contains GitHub related variables.
-	///
-	/// Note that this checks the variables starting with "github" and
-	/// "commit.github" and ignores "remote.github" values.
-	#[cfg(feature = "github")]
-	pub(crate) fn contains_github_variable(&self) -> bool {
-		self.variables
+	/// Returns `true` if the template contains one of the given variables.
+	#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
+	pub(crate) fn contains_variable(&self, variables: &[&str]) -> bool {
+		variables
 			.iter()
-			.any(|v| v.starts_with("github") || v.starts_with("commit.github"))
+			.any(|var| self.variables.iter().any(|v| v.starts_with(var)))
 	}
 
 	/// Renders the template.
 	pub fn render<C: Serialize, T: Serialize, S: Into<String> + Clone>(
 		&self,
 		context: &C,
 		additional_context: Option<&HashMap<S, T>>,
@@ -224,15 +221,23 @@
 					.into_iter()
 					.filter_map(|c| c.into_conventional().ok())
 					.collect(),
 					commit_id: None,
 					timestamp: 0,
 					previous: None,
 					#[cfg(feature = "github")]
-					github: crate::github::GitHubReleaseMetadata {
+					github: crate::remote::RemoteReleaseMetadata {
+						contributors: vec![],
+					},
+					#[cfg(feature = "gitlab")]
+					gitlab: crate::remote::RemoteReleaseMetadata {
+						contributors: vec![],
+					},
+					#[cfg(feature = "bitbucket")]
+					bitbucket: crate::remote::RemoteReleaseMetadata {
 						contributors: vec![],
 					},
 				},
 				Option::<HashMap<&str, String>>::None.as_ref(),
 				&[TextProcessor {
 					pattern:         Regex::new("<DATE>")
 						.expect("failed to compile regex"),
@@ -248,11 +253,14 @@
 				String::from("commit.message"),
 				String::from("commits"),
 				String::from("version"),
 			],
 			template.variables
 		);
 		#[cfg(feature = "github")]
-		assert!(!template.contains_github_variable());
+		{
+			assert!(!template.contains_variable(&["commit.github"]));
+			assert!(template.contains_variable(&["commit.group"]));
+		}
 		Ok(())
 	}
 }
```

### Comparing `git_cliff-2.2.2/git-cliff-core/tests/integration_test.rs` & `git_cliff-2.3.0/git-cliff-core/tests/integration_test.rs`

 * *Files 7% similar despite different names*

```diff
@@ -185,15 +185,23 @@
 			.iter()
 			.filter_map(|c| c.process(&git_config).ok())
 			.collect::<Vec<Commit>>(),
 			commit_id: None,
 			timestamp: 0,
 			previous:  None,
 			#[cfg(feature = "github")]
-			github: git_cliff_core::github::GitHubReleaseMetadata {
+			github: git_cliff_core::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "gitlab")]
+			gitlab: git_cliff_core::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "bitbucket")]
+			bitbucket: git_cliff_core::remote::RemoteReleaseMetadata {
 				contributors: vec![],
 			},
 		},
 		Release {
 			version:   Some(String::from("v1.0.0")),
 			commits:   vec![
 				Commit::new(
@@ -213,15 +221,23 @@
 			.into_iter()
 			.filter_map(|c| c.into_conventional().ok())
 			.collect::<Vec<Commit>>(),
 			commit_id: None,
 			timestamp: 0,
 			previous:  None,
 			#[cfg(feature = "github")]
-			github: git_cliff_core::github::GitHubReleaseMetadata {
+			github: git_cliff_core::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "gitlab")]
+			gitlab: git_cliff_core::remote::RemoteReleaseMetadata {
+				contributors: vec![],
+			},
+			#[cfg(feature = "bitbucket")]
+			bitbucket: git_cliff_core::remote::RemoteReleaseMetadata {
 				contributors: vec![],
 			},
 		},
 	];
 
 	let out = &mut String::new();
 	let template = Template::new(changelog_config.body.unwrap(), false)?;
```

### Comparing `git_cliff-2.2.2/README.md` & `git_cliff-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff/Cargo.toml` & `git_cliff-2.3.0/git-cliff/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 [package]
 name = "git-cliff"
-version = "2.2.2" # managed by release.sh
+version = "2.3.0" # managed by release.sh
 description = "A highly customizable changelog generator ⛰️"
 authors = ["git-cliff contributors <git-cliff@protonmail.com>"]
 license = "MIT OR Apache-2.0"
 readme = "../README.md"
 homepage = "https://github.com/orhun/git-cliff"
 repository = "https://github.com/orhun/git-cliff"
 keywords = ["changelog", "generator", "conventional", "commit"]
 categories = ["command-line-utilities"]
 default-run = "git-cliff"
 edition = "2021"
-rust-version = "1.74.1"
+rust-version = "1.75.0"
 
 [[bin]]
 name = "git-cliff-completions"
 path = "src/bin/completions.rs"
 
 [[bin]]
 name = "git-cliff-mangen"
 path = "src/bin/mangen.rs"
 
 [features]
 # check for new versions
-default = ["update-informer", "github"]
+default = ["update-informer", "github", "gitlab", "bitbucket"]
 # inform about new releases
 update-informer = ["dep:update-informer"]
 # enable GitHub integration
 github = ["git-cliff-core/github", "dep:indicatif"]
+# enable GitLab integration
+gitlab = ["git-cliff-core/gitlab", "dep:indicatif"]
+# enable Bitbucket integration
+bitbucket = ["git-cliff-core/bitbucket", "dep:indicatif"]
 
 [dependencies]
 glob.workspace = true
 regex.workspace = true
 log.workspace = true
 secrecy.workspace = true
 lazy_static.workspace = true
@@ -41,15 +45,15 @@
 clap_mangen = "0.2.20"
 shellexpand = "3.1.0"
 update-informer = { version = "1.1.0", optional = true }
 indicatif = { version = "0.17.8", optional = true }
 env_logger = "0.10.2"
 
 [dependencies.git-cliff-core]
-version = "2.2.2" # managed by release.sh
+version = "2.3.0" # managed by release.sh
 path = "../git-cliff-core"
 
 [dev-dependencies]
 pretty_assertions = "1.4.0"
 
 # metadata for cargo-binstall to get the right artifacts
 [package.metadata.binstall]
```

### Comparing `git_cliff-2.2.2/git-cliff/src/args.rs` & `git_cliff-2.3.0/git-cliff/src/args.rs`

 * *Files 6% similar despite different names*

```diff
@@ -60,191 +60,229 @@
 		short,
 		long,
 		action = ArgAction::Help,
 		global = true,
 		help = "Prints help information",
 		help_heading = "FLAGS"
 	)]
-	pub help:           Option<bool>,
+	pub help:            Option<bool>,
 	#[arg(
 		short = 'V',
 		long,
 		action = ArgAction::Version,
 		global = true,
 		help = "Prints version information",
 		help_heading = "FLAGS"
 	)]
-	pub version:        Option<bool>,
+	pub version:         Option<bool>,
 	/// Increases the logging verbosity.
 	#[arg(short, long, action = ArgAction::Count, alias = "debug", help_heading = Some("FLAGS"))]
-	pub verbose:        u8,
+	pub verbose:         u8,
 	/// Writes the default configuration file to cliff.toml
 	#[arg(
 	    short,
 	    long,
 	    value_name = "CONFIG",
 	    num_args = 0..=1,
 	    required = false
 	)]
-	pub init:           Option<Option<String>>,
+	pub init:            Option<Option<String>>,
 	/// Sets the configuration file.
 	#[arg(
 	    short,
 	    long,
 	    env = "GIT_CLIFF_CONFIG",
 	    value_name = "PATH",
 	    default_value = DEFAULT_CONFIG,
 	    value_parser = Opt::parse_dir
 	)]
-	pub config:         PathBuf,
+	pub config:          PathBuf,
 	/// Sets the working directory.
 	#[arg(
 	    short,
 	    long,
 	    env = "GIT_CLIFF_WORKDIR",
 	    value_name = "PATH",
 	    value_parser = Opt::parse_dir
 	)]
-	pub workdir:        Option<PathBuf>,
+	pub workdir:         Option<PathBuf>,
 	/// Sets the git repository.
 	#[arg(
 		short,
 		long,
 		env = "GIT_CLIFF_REPOSITORY",
 		value_name = "PATH",
 		num_args(1..),
 		value_parser = Opt::parse_dir
 	)]
-	pub repository:     Option<Vec<PathBuf>>,
+	pub repository:      Option<Vec<PathBuf>>,
 	/// Sets the path to include related commits.
 	#[arg(
 		long,
 		env = "GIT_CLIFF_INCLUDE_PATH",
 		value_name = "PATTERN",
 		num_args(1..)
 	)]
-	pub include_path:   Option<Vec<Pattern>>,
+	pub include_path:    Option<Vec<Pattern>>,
 	/// Sets the path to exclude related commits.
 	#[arg(
 		long,
 		env = "GIT_CLIFF_EXCLUDE_PATH",
 		value_name = "PATTERN",
 		num_args(1..)
 	)]
-	pub exclude_path:   Option<Vec<Pattern>>,
+	pub exclude_path:    Option<Vec<Pattern>>,
 	/// Sets the regex for matching git tags.
 	#[arg(long, env = "GIT_CLIFF_TAG_PATTERN", value_name = "PATTERN")]
-	pub tag_pattern:    Option<Regex>,
+	pub tag_pattern:     Option<Regex>,
 	/// Sets custom commit messages to include in the changelog.
 	#[arg(
 		long,
 		env = "GIT_CLIFF_WITH_COMMIT",
 		value_name = "MSG",
 		num_args(1..)
 	)]
-	pub with_commit:    Option<Vec<String>>,
+	pub with_commit:     Option<Vec<String>>,
 	/// Sets commits that will be skipped in the changelog.
 	#[arg(
 		long,
 		env = "GIT_CLIFF_SKIP_COMMIT",
 		value_name = "SHA1",
 		num_args(1..)
 	)]
-	pub skip_commit:    Option<Vec<String>>,
+	pub skip_commit:     Option<Vec<String>>,
 	/// Prepends entries to the given changelog file.
 	#[arg(
 	    short,
 	    long,
 	    env = "GIT_CLIFF_PREPEND",
 	    value_name = "PATH",
 	    value_parser = Opt::parse_dir
 	)]
-	pub prepend:        Option<PathBuf>,
+	pub prepend:         Option<PathBuf>,
 	/// Writes output to the given file.
 	#[arg(
 	    short,
 	    long,
 	    env = "GIT_CLIFF_OUTPUT",
 	    value_name = "PATH",
 	    value_parser = Opt::parse_dir,
 	    num_args = 0..=1,
 	    default_missing_value = DEFAULT_OUTPUT
 	)]
-	pub output:         Option<PathBuf>,
+	pub output:          Option<PathBuf>,
 	/// Sets the tag for the latest version.
 	#[arg(
 		short,
 		long,
 		env = "GIT_CLIFF_TAG",
 		value_name = "TAG",
 		allow_hyphen_values = true
 	)]
-	pub tag:            Option<String>,
+	pub tag:             Option<String>,
 	/// Bumps the version for unreleased changes.
 	#[arg(long, help_heading = Some("FLAGS"))]
-	pub bump:           bool,
+	pub bump:            bool,
 	/// Prints bumped version for unreleased changes.
 	#[arg(long, help_heading = Some("FLAGS"))]
-	pub bumped_version: bool,
+	pub bumped_version:  bool,
 	/// Sets the template for the changelog body.
 	#[arg(
 		short,
 		long,
 		env = "GIT_CLIFF_TEMPLATE",
 		value_name = "TEMPLATE",
 		allow_hyphen_values = true
 	)]
-	pub body:           Option<String>,
+	pub body:            Option<String>,
 	/// Processes the commits starting from the latest tag.
 	#[arg(short, long, help_heading = Some("FLAGS"))]
-	pub latest:         bool,
+	pub latest:          bool,
 	/// Processes the commits that belong to the current tag.
 	#[arg(long, help_heading = Some("FLAGS"))]
-	pub current:        bool,
+	pub current:         bool,
 	/// Processes the commits that do not belong to a tag.
 	#[arg(short, long, help_heading = Some("FLAGS"))]
-	pub unreleased:     bool,
+	pub unreleased:      bool,
 	/// Sorts the tags topologically.
 	#[arg(long, help_heading = Some("FLAGS"))]
-	pub topo_order:     bool,
+	pub topo_order:      bool,
 	/// Disables the external command execution.
 	#[arg(long, help_heading = Some("FLAGS"))]
-	pub no_exec:        bool,
+	pub no_exec:         bool,
 	/// Prints changelog context as JSON.
 	#[arg(short = 'x', long, help_heading = Some("FLAGS"))]
-	pub context:        bool,
+	pub context:         bool,
 	/// Strips the given parts from the changelog.
 	#[arg(short, long, value_name = "PART", value_enum)]
-	pub strip:          Option<Strip>,
+	pub strip:           Option<Strip>,
 	/// Sets sorting of the commits inside sections.
 	#[arg(
 		long,
 		value_enum,
 		default_value_t = Sort::Oldest
 	)]
-	pub sort:           Sort,
+	pub sort:            Sort,
 	/// Sets the commit range to process.
 	#[arg(value_name = "RANGE", help_heading = Some("ARGS"))]
-	pub range:          Option<String>,
+	pub range:           Option<String>,
 	/// Sets the GitHub API token.
 	#[arg(
 		long,
 		env = "GITHUB_TOKEN",
 		value_name = "TOKEN",
-		hide_env_values = true
+		hide_env_values = true,
+		hide = !cfg!(feature = "github"),
 	)]
-	pub github_token:   Option<SecretString>,
+	pub github_token:    Option<SecretString>,
 	/// Sets the GitHub repository.
 	#[arg(
-	    long,
-	    env = "GITHUB_REPO",
-	    value_parser = clap::value_parser!(RemoteValue),
-	    value_name = "OWNER/REPO"
+		long,
+		env = "GITHUB_REPO",
+		value_parser = clap::value_parser!(RemoteValue),
+		value_name = "OWNER/REPO",
+		hide = !cfg!(feature = "github"),
+	)]
+	pub github_repo:     Option<RemoteValue>,
+	/// Sets the GitLab API token.
+	#[arg(
+		long,
+		env = "GITLAB_TOKEN",
+		value_name = "TOKEN",
+		hide_env_values = true,
+		hide = !cfg!(feature = "gitlab"),
+	)]
+	pub gitlab_token:    Option<SecretString>,
+	/// Sets the GitLab repository.
+	#[arg(
+		long,
+		env = "GITLAB_REPO",
+		value_parser = clap::value_parser!(RemoteValue),
+		value_name = "OWNER/REPO",
+		hide = !cfg!(feature = "gitlab"),
+	)]
+	pub gitlab_repo:     Option<RemoteValue>,
+	/// Sets the Bitbucket API token.
+	#[arg(
+		long,
+		env = "BITBUCKET_TOKEN",
+		value_name = "TOKEN",
+		hide_env_values = true,
+		hide = !cfg!(feature = "bitbucket"),
+	)]
+	pub bitbucket_token: Option<SecretString>,
+	/// Sets the Bitbucket repository.
+	#[arg(
+		long,
+		env = "BITBUCKET_REPO",
+		value_parser = clap::value_parser!(RemoteValue),
+		value_name = "OWNER/REPO",
+		hide = !cfg!(feature = "bitbucket"),
 	)]
-	pub github_repo:    Option<RemoteValue>,
+	pub bitbucket_repo:  Option<RemoteValue>,
 }
 
 /// Custom type for the remote value.
 #[derive(Clone, Debug, PartialEq)]
 pub struct RemoteValue(pub Remote);
 
 impl ValueParserFactory for RemoteValue {
```

### Comparing `git_cliff-2.2.2/git-cliff/src/bin/completions.rs` & `git_cliff-2.3.0/git-cliff/src/bin/completions.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff/src/bin/mangen.rs` & `git_cliff-2.3.0/git-cliff/src/bin/mangen.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/git-cliff/src/lib.rs` & `git_cliff-2.3.0/git-cliff/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 	self,
 	File,
 };
 use std::io::{
 	self,
 	Write,
 };
+use std::path::PathBuf;
 use std::time::{
 	SystemTime,
 	UNIX_EPOCH,
 };
 
 /// Checks for a new version on crates.io
 #[cfg(feature = "update-informer")]
@@ -115,15 +116,37 @@
 		match repository.upstream_remote() {
 			Ok(remote) => {
 				debug!("No GitHub remote is set, using remote: {}", remote);
 				config.remote.github.owner = remote.owner;
 				config.remote.github.repo = remote.repo;
 			}
 			Err(e) => {
-				debug!("Failed to get remote from repository: {:?}", e);
+				debug!("Failed to get remote from GitHub repository: {:?}", e);
+			}
+		}
+	} else if !config.remote.gitlab.is_set() {
+		match repository.upstream_remote() {
+			Ok(remote) => {
+				debug!("No GitLab remote is set, using remote: {}", remote);
+				config.remote.gitlab.owner = remote.owner;
+				config.remote.gitlab.repo = remote.repo;
+			}
+			Err(e) => {
+				debug!("Failed to get remote from GitLab repository: {:?}", e);
+			}
+		}
+	} else if !config.remote.bitbucket.is_set() {
+		match repository.upstream_remote() {
+			Ok(remote) => {
+				debug!("No Bitbucket remote is set, using remote: {}", remote);
+				config.remote.bitbucket.owner = remote.owner;
+				config.remote.bitbucket.repo = remote.repo;
+			}
+			Err(e) => {
+				debug!("Failed to get remote from Bitbucket repository: {:?}", e);
 			}
 		}
 	}
 
 	// Print debug information about configuration and arguments.
 	log::trace!("Arguments: {:#?}", args);
 	log::trace!("Config: {:#?}", config);
@@ -381,14 +404,23 @@
 		config.changelog.footer = None;
 		if !(args.unreleased || args.latest || args.range.is_some()) {
 			return Err(Error::ArgumentError(String::from(
 				"'-u' or '-l' is not specified",
 			)));
 		}
 	}
+	if args.output.is_some() &&
+		args.prepend.is_some() &&
+		args.output.as_ref() == args.prepend.as_ref()
+	{
+		return Err(Error::ArgumentError(String::from(
+			"'-o' and '-p' can only be used together if they point to different \
+			 files",
+		)));
+	}
 	if args.body.is_some() {
 		config.changelog.body.clone_from(&args.body);
 	}
 	if args.sort == Sort::Oldest {
 		if let Some(ref sort_commits) = config.git.sort_commits {
 			args.sort = Sort::from_str(sort_commits, true)
 				.expect("Incorrect config value for 'sort_commits'");
@@ -398,18 +430,36 @@
 		if let Some(topo_order) = config.git.topo_order {
 			args.topo_order = topo_order;
 		}
 	}
 	if args.github_token.is_some() {
 		config.remote.github.token.clone_from(&args.github_token);
 	}
+	if args.gitlab_token.is_some() {
+		config.remote.gitlab.token.clone_from(&args.gitlab_token);
+	}
+	if args.bitbucket_token.is_some() {
+		config
+			.remote
+			.bitbucket
+			.token
+			.clone_from(&args.bitbucket_token);
+	}
 	if let Some(ref remote) = args.github_repo {
 		config.remote.github.owner = remote.0.owner.to_string();
 		config.remote.github.repo = remote.0.repo.to_string();
 	}
+	if let Some(ref remote) = args.gitlab_repo {
+		config.remote.gitlab.owner = remote.0.owner.to_string();
+		config.remote.gitlab.repo = remote.0.repo.to_string();
+	}
+	if let Some(ref remote) = args.bitbucket_repo {
+		config.remote.bitbucket.owner = remote.0.owner.to_string();
+		config.remote.bitbucket.repo = remote.0.repo.to_string();
+	}
 	if args.no_exec {
 		if let Some(ref mut preprocessors) = config.git.commit_preprocessors {
 			preprocessors
 				.iter_mut()
 				.for_each(|v| v.replace_command = None);
 		}
 		if let Some(ref mut postprocessors) = config.changelog.postprocessors {
@@ -494,15 +544,19 @@
 			changelog.write_context(&mut io::stdout())
 		};
 	}
 	if let Some(ref path) = args.prepend {
 		changelog.prepend(fs::read_to_string(path)?, &mut File::create(path)?)?;
 	}
 	if let Some(path) = args.output {
-		let mut output = File::create(path)?;
+		let mut output: Box<dyn Write> = if path == PathBuf::from("-") {
+			Box::new(io::stdout())
+		} else {
+			Box::new(File::create(path)?)
+		};
 		if args.context {
 			changelog.write_context(&mut output)
 		} else {
 			changelog.generate(&mut output)
 		}
 	} else if args.prepend.is_none() {
 		changelog.generate(&mut io::stdout())
```

### Comparing `git_cliff-2.2.2/git-cliff/src/logger.rs` & `git_cliff-2.3.0/git-cliff/src/logger.rs`

 * *Files 26% similar despite different names*

```diff
@@ -6,20 +6,15 @@
 	},
 	Builder,
 };
 use git_cliff_core::error::{
 	Error,
 	Result,
 };
-#[cfg(feature = "github")]
-use git_cliff_core::github::{
-	FINISHED_FETCHING_MSG,
-	START_FETCHING_MSG,
-};
-#[cfg(feature = "github")]
+#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
 use indicatif::{
 	ProgressBar,
 	ProgressStyle,
 };
 use log::Level;
 use std::io::Write;
 use std::sync::atomic::{
@@ -67,15 +62,15 @@
 		Level::Debug => style.set_color(Color::Blue).value("DEBUG"),
 		Level::Info => style.set_color(Color::Green).value("INFO "),
 		Level::Warn => style.set_color(Color::Yellow).value("WARN "),
 		Level::Error => style.set_color(Color::Red).value("ERROR"),
 	}
 }
 
-#[cfg(feature = "github")]
+#[cfg(any(feature = "github", feature = "gitlab", feature = "bitbucket"))]
 lazy_static::lazy_static! {
 	/// Lazily initialized progress bar.
 	pub static ref PROGRESS_BAR: ProgressBar = {
 		let progress_bar = ProgressBar::new_spinner();
 		progress_bar.set_style(
 			ProgressStyle::with_template("{spinner:.green} {msg}")
 				.unwrap()
@@ -93,47 +88,85 @@
 	};
 }
 
 /// Initializes the global logger.
 ///
 /// This method also creates a progress bar which is triggered
 /// by the network operations that are related to GitHub.
+#[allow(unreachable_code, clippy::needless_return)]
 pub fn init() -> Result<()> {
 	let mut builder = Builder::new();
 	builder.format(move |f, record| {
 		let target = record.target();
 		let max_width = max_target_width(target);
 
 		let mut style = f.style();
 		let level = colored_level(&mut style, record.level());
 
 		let mut style = f.style();
 		let target = style.set_bold(true).value(Padded {
 			value: target,
 			width: max_width,
 		});
+
 		#[cfg(feature = "github")]
 		{
 			let message = record.args().to_string();
-			if message.starts_with(START_FETCHING_MSG) {
+			if message
+				.starts_with(git_cliff_core::remote::github::START_FETCHING_MSG)
+			{
 				PROGRESS_BAR
 					.enable_steady_tick(std::time::Duration::from_millis(80));
 				PROGRESS_BAR.set_message(message);
-				Ok(())
-			} else if message.starts_with(FINISHED_FETCHING_MSG) {
+				return Ok(());
+			} else if message
+				.starts_with(git_cliff_core::remote::github::FINISHED_FETCHING_MSG)
+			{
 				PROGRESS_BAR.finish_and_clear();
-				Ok(())
-			} else {
-				writeln!(f, " {} {} > {}", level, target, record.args(),)
+				return Ok(());
 			}
 		}
-		#[cfg(not(feature = "github"))]
+
+		#[cfg(feature = "gitlab")]
 		{
-			writeln!(f, " {} {} > {}", level, target, record.args(),)
+			let message = record.args().to_string();
+			if message
+				.starts_with(git_cliff_core::remote::gitlab::START_FETCHING_MSG)
+			{
+				PROGRESS_BAR
+					.enable_steady_tick(std::time::Duration::from_millis(80));
+				PROGRESS_BAR.set_message(message);
+				return Ok(());
+			} else if message
+				.starts_with(git_cliff_core::remote::gitlab::FINISHED_FETCHING_MSG)
+			{
+				PROGRESS_BAR.finish_and_clear();
+				return Ok(());
+			}
 		}
+
+		#[cfg(feature = "bitbucket")]
+		{
+			let message = record.args().to_string();
+			if message
+				.starts_with(git_cliff_core::remote::bitbucket::START_FETCHING_MSG)
+			{
+				PROGRESS_BAR
+					.enable_steady_tick(std::time::Duration::from_millis(80));
+				PROGRESS_BAR.set_message(message);
+				return Ok(());
+			} else if message.starts_with(
+				git_cliff_core::remote::bitbucket::FINISHED_FETCHING_MSG,
+			) {
+				PROGRESS_BAR.finish_and_clear();
+				return Ok(());
+			}
+		}
+
+		writeln!(f, " {} {} > {}", level, target, record.args())
 	});
 
 	if let Ok(var) = env::var(LOGGER_ENV) {
 		builder.parse_filters(&var);
 	}
 
 	builder
```

### Comparing `git_cliff-2.2.2/git-cliff/src/main.rs` & `git_cliff-2.3.0/git-cliff/src/main.rs`

 * *Files identical despite different names*

### Comparing `git_cliff-2.2.2/Cargo.lock` & `git_cliff-2.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -266,28 +266,28 @@
  "iana-time-zone",
  "num-traits",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.6"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d59ae0466b83e838b81a54256c39d5d7c20b9d7daa10510a242d9b75abd5936e"
+checksum = "93698b29de5e97ad0ae26447b344c482a7284c737d9ddc5f9e52b74a336671bb"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
 name = "chrono-tz-build"
-version = "0.2.1"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "433e39f13c9a060046954e0592a8d0a4bcb1040125cbf91cb8ee58964cfb350f"
+checksum = "0c088aee841df9c3041febbb73934cfc39708749bf96dc827e3359cd39ef11b1"
 dependencies = [
  "parse-zoneinfo",
  "phf",
  "phf_codegen",
 ]
 
 [[package]]
@@ -541,14 +541,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
  "litrs",
 ]
 
 [[package]]
+name = "dyn-clone"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
+
+[[package]]
 name = "either"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encode_unicode"
@@ -749,15 +755,15 @@
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "git-cliff"
-version = "2.2.2"
+version = "2.3.0"
 dependencies = [
  "clap",
  "clap_complete",
  "clap_mangen",
  "dirs",
  "env_logger",
  "git-cliff-core",
@@ -770,19 +776,20 @@
  "secrecy",
  "shellexpand",
  "update-informer",
 ]
 
 [[package]]
 name = "git-cliff-core"
-version = "2.2.2"
+version = "2.3.0"
 dependencies = [
  "config",
  "dirs",
  "document-features",
+ "dyn-clone",
  "expect-test",
  "futures",
  "git-conventional",
  "git2",
  "glob",
  "http-cache-reqwest",
  "indexmap",
@@ -849,19 +856,19 @@
  "log",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "globwalk"
-version = "0.8.1"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93e3af942408868f6934a7b85134a3230832b9977cf66125df2f9edcfce4ddcc"
+checksum = "0bf760ebf69878d9fd8f110c89703d90ce35095324d1f1edcb595c63945ee757"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "ignore",
  "walkdir",
 ]
 
 [[package]]
 name = "h2"
 version = "0.3.26"
@@ -1486,17 +1493,17 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "next_version"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3e541a09da6184deaa5f0c9eeec570dbea6ea841d92c84cdfa4ff985aa535fa"
+checksum = "7beae5e84c3330a90f0f89eae10f5cd4c17c3be0f119ab36d94fd908c7b8c8fb"
 dependencies = [
  "conventional_commit_parser",
  "semver",
 ]
 
 [[package]]
 name = "nom"
@@ -2126,26 +2133,26 @@
 name = "semver"
 version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "serde"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.201"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
@@ -2167,17 +2174,17 @@
 dependencies = [
  "regex",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
+checksum = "79e674e01f999af37c49f70a6ede167a8a60b2503e56c5599532a65baa5969a0"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -2367,17 +2374,17 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "tera"
-version = "1.19.1"
+version = "1.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "970dff17c11e884a4a09bc76e3a17ef71e01bb13447a11e85226e254fe6d10b8"
+checksum = "ab9d851b45e865f178319da0abdbfe6acbc4328759ff18dafc3a41c16b4cd2ee"
 dependencies = [
  "chrono",
  "chrono-tz",
  "globwalk",
  "humansize",
  "lazy_static",
  "percent-encoding",
@@ -2408,26 +2415,26 @@
 dependencies = [
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.60"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
@@ -2474,34 +2481,34 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.37.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
+checksum = "5f5ae998a069d4b5aba8ee9dad856af7d520c3699e6159b185c2acd48155d39a"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
@@ -2547,38 +2554,38 @@
  "futures-sink",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "toml"
-version = "0.8.12"
+version = "0.8.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
+checksum = "a4e43f8cc456c9704c851ae29c67e17ef65d2c30017c17a9765b89c382dc8bba"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.12"
+version = "0.22.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
+checksum = "c127785850e8c20836d49732ae6abfa47616e60bf9d9f57c43c250361a9db96c"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
```

### Comparing `git_cliff-2.2.2/PKG-INFO` & `git_cliff-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: git-cliff
-Version: 2.2.2
+Version: 2.3.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A highly customizable changelog generator ⛰️
 Keywords: changelog,generator,conventional,commit
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: git-cliff Version: 2.2.2 Classifier: Intended
+Metadata-Version: 2.3 Name: git-cliff Version: 2.3.0 Classifier: Intended
 Audience :: Developers Classifier: Topic :: Software Development Classifier:
 Programming Language :: Rust Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Summary: A highly customizable changelog generator
 â°ï¸ Keywords: changelog,generator,conventional,commit Home-Page: https://
 github.com/orhun/git-cliff Author: git-cliff contributors
 protonmail.com> Author-email: git-cliff contributors
```

