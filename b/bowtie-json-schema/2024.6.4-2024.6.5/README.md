# Comparing `tmp/bowtie_json_schema-2024.6.4.tar.gz` & `tmp/bowtie_json_schema-2024.6.5.tar.gz`

## Comparing `bowtie_json_schema-2024.6.4.tar` & `bowtie_json_schema-2024.6.5.tar`

### file list

```diff
@@ -1,296 +1,295 @@
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.gitpod.Dockerfile
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.gitpod.yml
--rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.prettierrc.json
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.readthedocs.yaml
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/action.yml
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/noxfile.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/requirements.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/test-requirements.in
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/test-requirements.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.devcontainer/devcontainer.json
--rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.pre-commit-hooks/check-dependabot
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.pre-commit-hooks/check-lintsonschema-schema
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/__main__.py
--rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_cli.py
--rw-r--r--   0        0        0    12452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_commands.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_connectables.py
--rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_containers.py
--rw-r--r--   0        0        0    21846 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_core.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_direct_connectable.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_registry.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_report.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/_suite.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/exceptions.py
--rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/hypothesis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/py.typed
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/report.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/cli/filter-implementations.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/cli/smoke.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/cli/statistics.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/cli/summary.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/bowtie/schemas/models/test.json
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/data/dialects.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/Makefile
--rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/cli.rst
--rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/conf.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/contributing.rst
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/github-actions.rst
--rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/implementers.rst
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/index.rst
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/motd.txt
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/requirements.in
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/requirements.txt
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/_static/bowtie_diagram_dark.svg
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/_static/bowtie_diagram_light.svg
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/docs/_static/logo.svg
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/index.html
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/package.json
--rw-r--r--   0        0        0   163693 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/pnpm-lock.yaml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/tsconfig.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/vite.config.ts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/public/favicon.svg
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/DialectReportView.tsx
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/MainContainer.tsx
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/ReportDataHandler.tsx
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/global.css
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/index.tsx
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/assets/landscape-logo.svg
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/CopyToClipboard.tsx
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/FilterSection.module.css
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/FilterSection.tsx
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/LoadingAnimation.tsx
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/NavBar.tsx
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/OtherImplementations.tsx
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseItem.tsx
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseResultSvg.test.tsx
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseResultSvg.tsx
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CasesSection.tsx
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Cases/SchemaDisplay.tsx
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/DragAndDrop/DragAndDrop.module.css
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/EmbedBadges.module.css
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Modals/DetailsButtonModal.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/RunInfo/RunInfoSection.tsx
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Summary/ImplementationRow.css
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Summary/ImplementationRow.tsx
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Summary/SummarySection.tsx
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/components/Summary/SummaryTable.tsx
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/context/BowtieVersionContext.tsx
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/context/ThemeContext.tsx
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Badge.test.ts
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Badge.ts
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Dialect.test.ts
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Dialect.ts
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Site.test.ts
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/Site.ts
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/mapLanguage.ts
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/parseReportData.test.ts
--rw-r--r--   0        0        0     9248 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/data/parseReportData.ts
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/frontend/src/hooks/useSearchParams.ts
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/.java-implementations-pmd-ruleset.xml
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/clojure-json-schema/Dockerfile
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/clojure-json-schema/project.clj
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/cpp-valijson/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/cpp-valijson/.gitignore
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/cpp-valijson/Dockerfile
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/cpp-valijson/bowtie_valijson.cpp
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/cpp-valijson/compile_flags.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/.clang-format
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/.editorconfig
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/Dockerfile
--rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/Program.cs
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/content.json
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/format.json
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/content.json
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-annotation.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-assertion.json
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/unevaluated.json
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/.clang-format
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/.gitignore
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/Dockerfile
--rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/Program.cs
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/Dockerfile
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/bowtie_gojsonschema.go
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/go.mod
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/go.sum
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-jsonschema/Dockerfile
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-jsonschema/bowtie_jsonschema.go
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-jsonschema/go.mod
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/go-jsonschema/go.sum
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-schema/BowtieJsonSchema.java
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-schema/Dockerfile
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-schema/build.gradle
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-tools-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-json-tools-json-schema-validator/build.gradle
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-jsonschemafriend/Dockerfile
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-jsonschemafriend/build.gradle
--rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-networknt-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-networknt-json-schema-validator/build.gradle
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/.dockerignore
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/.editorconfig
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/Dockerfile
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/build.gradle.kts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/gradle.properties
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/justfile
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/settings.gradle.kts
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/gradle/libs.versions.toml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-ajv/Dockerfile
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-ajv/bowtie_ajv.js
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-ajv/package-lock.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-ajv/package.json
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-hyperjump/Dockerfile
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-hyperjump/bowtie_hyperjump.js
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-hyperjump/package.json
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-json-schema/Dockerfile
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-json-schema/bowtie_json_schema.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-json-schema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-jsonschema/bowtie_jsonschema.js
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-jsonschema/package.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-schemasafe/Dockerfile
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-schemasafe/bowtie_schemasafe.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/js-schemasafe/package.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/.gitignore
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/Dockerfile
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
--rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/Dockerfile
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/bowtie_jsonschema.lua
--rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/json.lua
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/stylua.toml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/php-opis-json-schema/Dockerfile
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/php-opis-json-schema/bowtieJsonSchema.php
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/php-opis-json-schema/composer.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-fastjsonschema/Dockerfile
--rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-jschon/Dockerfile
--rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-jschon/bowtie_jschon.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-jsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/python-jsonschema/bowtie_jsonschema.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/.rubocop.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/Dockerfile
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/Gemfile
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/Gemfile.lock
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb
--rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-boon/Cargo.lock
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-boon/Cargo.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-boon/Dockerfile
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-boon/build.rs
--rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-boon/src/main.rs
--rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/Cargo.lock
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/Cargo.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/Dockerfile
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/build.rs
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/src/main.rs
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/Dockerfile
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/Harness.scala
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/project/plugins.sbt
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/Dockerfile
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/Harness.scala
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/build.sbt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/project/build.properties
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/project/plugins.sbt
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ts-vscode-json-languageservice/Dockerfile
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ts-vscode-json-languageservice/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/implementations/ts-vscode-json-languageservice/tsconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/conftest.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_cli.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_connectables.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_dialect.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_github.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_hypothesis.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_implementation.py
--rw-r--r--   0        0        0    75510 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_integration.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_registry.py
--rw-r--r--   0        0        0    10199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_report.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/test_schemas.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/envsonschema/Dockerfile
--rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/envsonschema/envsonschema
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/Dockerfile
--rwxr-xr-x   0        0        0     3069 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/lintsonschema
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/connectables.json
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/report.json
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/filter-implementations.json
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/.gitignore
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/LICENSE
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/README.rst
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/hatch_build.py
--rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/pyproject.toml
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.4/PKG-INFO
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.gitpod.Dockerfile
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.gitpod.yml
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.prettierrc.json
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/action.yml
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/noxfile.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/test-requirements.in
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/test-requirements.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.devcontainer/devcontainer.json
+-rwxr-xr-x   0        0        0     2229 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.pre-commit-hooks/check-dependabot
+-rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.pre-commit-hooks/check-lintsonschema-schema
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/__main__.py
+-rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_cli.py
+-rw-r--r--   0        0        0    12452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_commands.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_connectables.py
+-rw-r--r--   0        0        0    11585 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_containers.py
+-rw-r--r--   0        0        0    21846 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_core.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_direct_connectable.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_registry.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_report.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/_suite.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/exceptions.py
+-rw-r--r--   0        0        0     9633 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/hypothesis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/py.typed
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/bowtie/schemas/models/test.json
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/data/dialects.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/Makefile
+-rw-r--r--   0        0        0    11572 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/cli.rst
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/conf.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/contributing.rst
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/github-actions.rst
+-rw-r--r--   0        0        0    36467 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/implementers.rst
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/index.rst
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/motd.txt
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/requirements.in
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/requirements.txt
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/_static/bowtie_diagram_dark.svg
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/_static/bowtie_diagram_light.svg
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/docs/_static/logo.svg
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/index.html
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/package.json
+-rw-r--r--   0        0        0   163693 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/pnpm-lock.yaml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/tsconfig.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/vite.config.ts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/public/favicon.svg
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/DialectReportView.tsx
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/MainContainer.tsx
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/ReportDataHandler.tsx
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/global.css
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/index.tsx
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/assets/landscape-logo.svg
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/CopyToClipboard.tsx
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/FilterSection.module.css
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/FilterSection.tsx
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/LoadingAnimation.tsx
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/NavBar.tsx
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/OtherImplementations.tsx
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseItem.tsx
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseResultSvg.test.tsx
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseResultSvg.tsx
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CasesSection.tsx
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Cases/SchemaDisplay.tsx
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/DragAndDrop/DragAndDrop.module.css
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/EmbedBadges.module.css
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Modals/DetailsButtonModal.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/RunInfo/RunInfoSection.tsx
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Summary/ImplementationRow.tsx
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Summary/SummarySection.tsx
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/components/Summary/SummaryTable.tsx
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/context/BowtieVersionContext.tsx
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/context/ThemeContext.tsx
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Badge.test.ts
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Badge.ts
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Dialect.test.ts
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Dialect.ts
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Site.test.ts
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/Site.ts
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/mapLanguage.ts
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/parseReportData.test.ts
+-rw-r--r--   0        0        0     9055 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/data/parseReportData.ts
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/frontend/src/hooks/useSearchParams.ts
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/.java-implementations-pmd-ruleset.xml
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/clojure-json-schema/Dockerfile
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/clojure-json-schema/project.clj
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/cpp-valijson/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/cpp-valijson/.gitignore
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/cpp-valijson/Dockerfile
+-rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/cpp-valijson/bowtie_valijson.cpp
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/cpp-valijson/compile_flags.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/.clang-format
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/.editorconfig
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/Dockerfile
+-rw-r--r--   0        0        0    22323 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/Program.cs
+-rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/content.json
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/format.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/content.json
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-annotation.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/format-assertion.json
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/unevaluated.json
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/.clang-format
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/.gitignore
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/Dockerfile
+-rw-r--r--   0        0        0     7305 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/Program.cs
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/bowtie_json_everything.csproj
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/Properties/launchSettings.json
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/Dockerfile
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/bowtie_gojsonschema.go
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/go.mod
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/go.sum
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-jsonschema/bowtie_jsonschema.go
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-jsonschema/go.mod
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/go-jsonschema/go.sum
+-rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-schema/BowtieJsonSchema.java
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-schema/Dockerfile
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-schema/build.gradle
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-tools-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-json-tools-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-jsonschemafriend/Dockerfile
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-jsonschemafriend/build.gradle
+-rw-r--r--   0        0        0     9453 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-networknt-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-networknt-json-schema-validator/build.gradle
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/.dockerignore
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/.editorconfig
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/Dockerfile
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/build.gradle.kts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/gradle.properties
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/justfile
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/settings.gradle.kts
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/gradle/libs.versions.toml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/Main.kt
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Configuration.kt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Dialect.kt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StopCmd.kt
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-ajv/Dockerfile
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-ajv/bowtie_ajv.js
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-ajv/package-lock.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-ajv/package.json
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-hyperjump/Dockerfile
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-hyperjump/bowtie_hyperjump.js
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-hyperjump/package.json
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-json-schema/Dockerfile
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-json-schema/bowtie_json_schema.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-json-schema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-jsonschema/bowtie_jsonschema.js
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-jsonschema/package.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-schemasafe/Dockerfile
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-schemasafe/bowtie_schemasafe.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/js-schemasafe/package.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/.gitignore
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/Dockerfile
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/settings.gradle.kts
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/gradle/libs.versions.toml
+-rw-r--r--   0        0        0     7879 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/Dockerfile
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/bowtie_jsonschema.lua
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/json.lua
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/stylua.toml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/php-opis-json-schema/Dockerfile
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/php-opis-json-schema/bowtieJsonSchema.php
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/php-opis-json-schema/composer.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-fastjsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     2980 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-jschon/Dockerfile
+-rwxr-xr-x   0        0        0     3844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-jschon/bowtie_jschon.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-jsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/python-jsonschema/bowtie_jsonschema.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/.rubocop.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/Dockerfile
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/Gemfile
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/Gemfile.lock
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb
+-rw-r--r--   0        0        0    13409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-boon/Cargo.lock
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-boon/Cargo.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-boon/Dockerfile
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-boon/build.rs
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-boon/src/main.rs
+-rw-r--r--   0        0        0    39299 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/Cargo.lock
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/Cargo.toml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/Dockerfile
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/build.rs
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/src/main.rs
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/Dockerfile
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/Harness.scala
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/Dockerfile
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/Harness.scala
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/build.sbt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/project/build.properties
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/project/plugins.sbt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ts-vscode-json-languageservice/Dockerfile
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ts-vscode-json-languageservice/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/implementations/ts-vscode-json-languageservice/tsconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/conftest.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_cli.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_connectables.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_dialect.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_github.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_hypothesis.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_implementation.py
+-rw-r--r--   0        0        0    75674 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_integration.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_registry.py
+-rw-r--r--   0        0        0    10199 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_report.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/test_schemas.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/envsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     6837 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/envsonschema/envsonschema
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/Dockerfile
+-rwxr-xr-x   0        0        0     3069 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/lintsonschema
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/.gitattributes
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/connectables.json
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/report.json
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/filter-implementations.json
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/stop.json
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation-id.json
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/registry.json
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/.gitignore
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/LICENSE
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/README.rst
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/hatch_build.py
+-rw-r--r--   0        0        0     5390 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 bowtie_json_schema-2024.6.5/PKG-INFO
```

### Comparing `bowtie_json_schema-2024.6.4/.gitpod.yml` & `bowtie_json_schema-2024.6.5/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/.pre-commit-config.yaml` & `bowtie_json_schema-2024.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/CONTRIBUTING.rst` & `bowtie_json_schema-2024.6.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/action.yml` & `bowtie_json_schema-2024.6.5/action.yml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/noxfile.py` & `bowtie_json_schema-2024.6.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/requirements.txt` & `bowtie_json_schema-2024.6.5/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # via httpx
 attrs==23.2.0
     # via
     #   bowtie-json-schema (pyproject.toml)
     #   aiohttp
     #   jsonschema
     #   referencing
-certifi==2024.2.2
+certifi==2024.6.2
     # via
     #   httpcore
     #   httpx
     #   requests
 cffi==1.16.0
     # via cryptography
 charset-normalizer==3.3.2
@@ -101,15 +101,15 @@
     # via python-dateutil
 sniffio==1.3.1
     # via
     #   anyio
     #   httpx
 structlog==24.2.0
     # via bowtie-json-schema (pyproject.toml)
-typing-extensions==4.12.0
+typing-extensions==4.12.1
     # via
     #   aiodocker
     #   rich-click
 uritemplate==4.1.1
     # via github3-py
 url-py==0.10.0
     # via bowtie-json-schema (pyproject.toml)
```

### Comparing `bowtie_json_schema-2024.6.4/test-requirements.txt` & `bowtie_json_schema-2024.6.5/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/.pre-commit-hooks/check-dependabot` & `bowtie_json_schema-2024.6.5/.pre-commit-hooks/check-dependabot`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/.pre-commit-hooks/check-lintsonschema-schema` & `bowtie_json_schema-2024.6.5/.pre-commit-hooks/check-lintsonschema-schema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_cli.py` & `bowtie_json_schema-2024.6.5/bowtie/_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_commands.py` & `bowtie_json_schema-2024.6.5/bowtie/_commands.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_connectables.py` & `bowtie_json_schema-2024.6.5/bowtie/_connectables.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_containers.py` & `bowtie_json_schema-2024.6.5/bowtie/_containers.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_core.py` & `bowtie_json_schema-2024.6.5/bowtie/_core.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_direct_connectable.py` & `bowtie_json_schema-2024.6.5/bowtie/_direct_connectable.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 """
 Direct connectables do not really connect anywhere and just operate in-memory.
 """
 
 from __future__ import annotations
 
 from contextlib import asynccontextmanager
+from importlib import metadata
 from typing import TYPE_CHECKING, Any, Generic
+import platform
 
 from attrs import asdict, field, frozen, mutable
-from attrs.validators import in_
 from referencing.jsonschema import EMPTY_REGISTRY
 from url import URL
 
 from bowtie._commands import CaseResult, Started, StartedDialect, TestResult
 from bowtie._core import Connection, Dialect, ImplementationInfo
 from bowtie._registry import E_co, SchemaCompiler
 
 if TYPE_CHECKING:
-    from collections.abc import AsyncIterator, Callable
+    from collections.abc import AsyncIterator, Callable, Iterable
+
+    from jsonschema import ValidationError
+    from jsonschema.protocols import Validator
+    from referencing.jsonschema import Schema, SchemaRegistry
 
     from bowtie._commands import Message
     from bowtie._connectables import ConnectableId
 
 
-def not_yet_connected(*_: Any):
-    def _not_yet_connected(*_: Any):
+class NoDirectConnection(Exception):
+    @classmethod
+    def check(cls, _: Any, __: Any, id: ConnectableId):
+        if id not in IMPLEMENTATIONS:
+            raise cls(id)
+
+    def __str__(self):
+        return f"No direct connection can be made to {self.args[0]!r}."
+
+
+def not_yet_connected(schema: Schema, registry: SchemaRegistry):
+    def _not_yet_connected(instance: Any):
         raise RuntimeError("Not yet connected!")
 
     return _not_yet_connected
 
 
 @mutable
 class Unconnection(Generic[E_co]):
@@ -58,20 +73,25 @@
                 )
                 return asdict(started)
             case {"cmd": "dialect", "dialect": uri}:
                 dialect = Dialect.by_uri()[URL.parse(uri)]
                 self._for_current_dialect = self._compile(dialect)
                 return asdict(StartedDialect.OK)
             case {"cmd": "run", "seq": seq, "case": case}:
-                validate = self._for_current_dialect(
+                errors_for = self._for_current_dialect(
                     case["schema"],
                     case.get("registry", EMPTY_REGISTRY),
                 )
                 results = [
-                    TestResult(valid=bool(validate(test["instance"])))
+                    TestResult(
+                        valid=(
+                            next(iter(errors_for(test["instance"])), None)
+                            is None
+                        ),
+                    )
                     for test in case["tests"]
                 ]
                 return {  # FIXME: Bleh this is not SeqResult
                     "seq": seq,
                     **CaseResult(results=results).serializable(),
                 }
             case {"cmd": "stop"}:
@@ -81,14 +101,79 @@
 
     async def poison(self, message: Message) -> None:
         """
         Do nothing.
         """
 
 
+def jsonschema(id: str) -> Unconnection[ValidationError]:
+    """
+    An (un)connection to the python-jsonschema implementation.
+    """
+    dialects = Dialect.by_alias()
+
+    from jsonschema.validators import (
+        validator_for,  # type: ignore[reportUnknownVariableType]
+    )
+
+    def compile(dialect: Dialect) -> SchemaCompiler[ValidationError]:
+        def _compile(
+            schema: Schema,
+            registry: SchemaRegistry,
+        ) -> Callable[[Any], Iterable[ValidationError]]:
+            DialectValidator: type[Validator] = validator_for(  # type: ignore[reportUnknownVariableType]
+                schema,
+                default=validator_for({"$schema": str(dialect.uri)}),
+            )
+            validator: Validator = DialectValidator(schema, registry=registry)  # type: ignore[reportUnknownVariableType]
+            return validator.iter_errors  # type: ignore[reportUnknownMemberType]
+
+        return _compile
+
+    return Unconnection(
+        id=id,
+        info=ImplementationInfo(
+            language="python",
+            name="jsonschema",
+            version=metadata.version("jsonschema"),
+            homepage=URL.parse(
+                "https://python-jsonschema.readthedocs.io/",
+            ),
+            documentation=URL.parse(
+                "https://python-jsonschema.readthedocs.io/",
+            ),
+            issues=URL.parse(
+                "https://github.com/python-jsonschema/jsonschema/issues",
+            ),
+            source=URL.parse(
+                "https://github.com/python-jsonschema/jsonschema",
+            ),
+            dialects=frozenset(
+                [
+                    dialects["2020"],
+                    dialects["2019"],
+                    dialects["7"],
+                    dialects["6"],
+                    dialects["4"],
+                    dialects["3"],
+                ],
+            ),
+            os=platform.system(),
+            os_version=platform.release(),
+            language_version=platform.python_version(),
+        ),
+        compile=compile,
+    )
+
+
+IMPLEMENTATIONS = {
+    "python-jsonschema": jsonschema,
+}
+
+
 @frozen
 class Direct:
     """
     A direct connectable connects by simply importing some Python object.
 
     This is generally going to be suitable only to implementations written in
     Python or to a language where a wrapper (PyO3, CFFI, ...) can expose
@@ -96,70 +181,14 @@
 
     This object represents only the lazy import.
     Connecting will lookup and call the object from the identified location.
     The return value should then be an object which makes use of a specific
     target implementation.
     """
 
-    _id: ConnectableId = field(
-        repr=False,
-        validator=in_(["jsonschema"]),
-        alias="id",
-    )
+    _id: ConnectableId = field(alias="id", validator=NoDirectConnection.check)
 
     connector = "direct"
 
     @asynccontextmanager
     async def connect(self, **kwargs: Any) -> AsyncIterator[Connection]:
-        from importlib import metadata
-        import platform
-
-        dialects = Dialect.by_alias()
-
-        from jsonschema.validators import (
-            validator_for,  # type: ignore[reportUnknownVariableType]
-        )
-
-        yield Unconnection(
-            id=f"{self.connector}:{self._id}",
-            info=ImplementationInfo(
-                language="python",
-                name="jsonschema",
-                version=metadata.version("jsonschema"),
-                homepage=URL.parse(
-                    "https://python-jsonschema.readthedocs.io/",
-                ),
-                documentation=URL.parse(
-                    "https://python-jsonschema.readthedocs.io/",
-                ),
-                issues=URL.parse(
-                    "https://github.com/python-jsonschema/jsonschema/issues",
-                ),
-                source=URL.parse(
-                    "https://github.com/python-jsonschema/jsonschema",
-                ),
-                dialects=frozenset(
-                    [
-                        dialects["2020"],
-                        dialects["2019"],
-                        dialects["7"],
-                        dialects["6"],
-                        dialects["4"],
-                        dialects["3"],
-                    ],
-                ),
-                os=platform.system(),
-                os_version=platform.release(),
-                language_version=platform.python_version(),
-            ),
-            compile=lambda dialect: (
-                lambda schema, registry: (  # type: ignore[reportUnknownMemberType]
-                    validator_for(
-                        schema,
-                        default=validator_for({"$schema": str(dialect.uri)}),
-                    )(
-                        schema,
-                        registry=registry,
-                    ).iter_errors
-                )
-            ),
-        )
+        yield IMPLEMENTATIONS[self._id](f"{self.connector}:{self._id}")
```

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_registry.py` & `bowtie_json_schema-2024.6.5/bowtie/_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 if TYPE_CHECKING:
     from jsonschema.exceptions import ValidationError
     from referencing.jsonschema import SchemaResource
 
 
 E_co = TypeVar("E_co", bound=Exception, covariant=True)
 ErrorsFor = Callable[[Any], Iterable[E_co]]
-SchemaCompiler = Callable[
-    [Schema, SchemaRegistry],
-    Callable[[Any], ErrorsFor[E_co]],
-]
+SchemaCompiler = Callable[[Schema, SchemaRegistry], ErrorsFor[E_co]]
 
 
 class UnexpectedlyValid(Exception):
     """
     An instance which was expected to be invalid just isn't.
     """
```

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_report.py` & `bowtie_json_schema-2024.6.5/bowtie/_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/_suite.py` & `bowtie_json_schema-2024.6.5/bowtie/_suite.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/exceptions.py` & `bowtie_json_schema-2024.6.5/bowtie/exceptions.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/hypothesis.py` & `bowtie_json_schema-2024.6.5/bowtie/hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/connectables.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/connectables.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/report.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/cli/info.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/cli/statistics.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/cli/statistics.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/io/v1.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/models/group.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/bowtie/schemas/models/test.json` & `bowtie_json_schema-2024.6.5/bowtie/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/data/dialects.json` & `bowtie_json_schema-2024.6.5/data/dialects.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/Makefile` & `bowtie_json_schema-2024.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/cli.rst` & `bowtie_json_schema-2024.6.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/conf.py` & `bowtie_json_schema-2024.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/contributing.rst` & `bowtie_json_schema-2024.6.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/github-actions.rst` & `bowtie_json_schema-2024.6.5/docs/github-actions.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/implementers.rst` & `bowtie_json_schema-2024.6.5/docs/implementers.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/index.rst` & `bowtie_json_schema-2024.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/motd.txt` & `bowtie_json_schema-2024.6.5/docs/motd.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/requirements.txt` & `bowtie_json_schema-2024.6.5/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/_static/bowtie_diagram_dark.svg` & `bowtie_json_schema-2024.6.5/docs/_static/bowtie_diagram_dark.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/_static/bowtie_diagram_light.svg` & `bowtie_json_schema-2024.6.5/docs/_static/bowtie_diagram_light.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/docs/_static/logo.svg` & `bowtie_json_schema-2024.6.5/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/package.json` & `bowtie_json_schema-2024.6.5/frontend/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9447368421052632%*

 * *Differences: {"'devDependencies'": "{'@typescript-eslint/eslint-plugin': '^7.11.0', "*

 * *                      "'@typescript-eslint/parser': '^7.11.0', 'eslint-plugin-react': '7.34.2', "*

 * *                      "'vite': '^5.2.12'}",*

 * * "'packageManager'": "'pnpm@9.1.4'"}*

```diff
@@ -13,26 +13,26 @@
     "description": "The UI displays the outcomes generated by Bowtie, which serves as a meta-validator for the JSON Schema specification",
     "devDependencies": {
         "@types/react": "^18.3.3",
         "@types/react-dom": "^18.3.0",
         "@types/react-syntax-highlighter": "^15.5.13",
         "@types/react-test-renderer": "^18.3.0",
         "@types/urijs": "^1.19.25",
-        "@typescript-eslint/eslint-plugin": "^7.10.0",
-        "@typescript-eslint/parser": "^7.10.0",
+        "@typescript-eslint/eslint-plugin": "^7.11.0",
+        "@typescript-eslint/parser": "^7.11.0",
         "@vitejs/plugin-react": "^4.3.0",
         "eslint": "8.57.0",
-        "eslint-plugin-react": "7.34.1",
+        "eslint-plugin-react": "7.34.2",
         "eslint-plugin-react-hooks": "4.6.2",
         "jsdom": "^24.1.0",
         "react-test-renderer": "^18.3.1",
         "ts-loader": "^9.5.1",
         "ts-node": "^10.9.2",
         "typescript": "^5.4.5",
-        "vite": "^5.2.11",
+        "vite": "^5.2.12",
         "vite-bundle-visualizer": "^1.2.1",
         "vitest": "^1.6.0"
     },
     "engines": {
         "node": ">=21.0.0"
     },
     "eslintConfig": {
@@ -70,15 +70,15 @@
         "settings": {
             "react": {
                 "version": "18.2"
             }
         }
     },
     "name": "bowtie",
-    "packageManager": "pnpm@9.1.2",
+    "packageManager": "pnpm@9.1.4",
     "scripts": {
         "build": "tsc && vite build",
         "bundle-visualizer": "vite-bundle-visualizer",
         "lint": "eslint src --max-warnings 0",
         "preview": "vite preview",
         "start": "vite --no-clearScreen",
         "test": "vitest run",
```

### Comparing `bowtie_json_schema-2024.6.4/frontend/pnpm-lock.yaml` & `bowtie_json_schema-2024.6.5/frontend/pnpm-lock.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -48,28 +48,28 @@
       '@types/react-test-renderer':
         specifier: ^18.3.0
         version: 18.3.0
       '@types/urijs':
         specifier: ^1.19.25
         version: 1.19.25
       '@typescript-eslint/eslint-plugin':
-        specifier: ^7.10.0
-        version: 7.10.0(@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.11.0
+        version: 7.11.0(@typescript-eslint/parser@7.11.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)
       '@typescript-eslint/parser':
-        specifier: ^7.10.0
-        version: 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+        specifier: ^7.11.0
+        version: 7.11.0(eslint@8.57.0)(typescript@5.4.5)
       '@vitejs/plugin-react':
         specifier: ^4.3.0
-        version: 4.3.0(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))
+        version: 4.3.0(vite@5.2.12(@types/node@20.11.5)(terser@5.27.0))
       eslint:
         specifier: 8.57.0
         version: 8.57.0
       eslint-plugin-react:
-        specifier: 7.34.1
-        version: 7.34.1(eslint@8.57.0)
+        specifier: 7.34.2
+        version: 7.34.2(eslint@8.57.0)
       eslint-plugin-react-hooks:
         specifier: 4.6.2
         version: 4.6.2(eslint@8.57.0)
       jsdom:
         specifier: ^24.1.0
         version: 24.1.0
       react-test-renderer:
@@ -81,16 +81,16 @@
       ts-node:
         specifier: ^10.9.2
         version: 10.9.2(@types/node@20.11.5)(typescript@5.4.5)
       typescript:
         specifier: ^5.4.5
         version: 5.4.5
       vite:
-        specifier: ^5.2.11
-        version: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
+        specifier: ^5.2.12
+        version: 5.2.12(@types/node@20.11.5)(terser@5.27.0)
       vite-bundle-visualizer:
         specifier: ^1.2.1
         version: 1.2.1(rollup@4.17.2)
       vitest:
         specifier: ^1.6.0
         version: 1.6.0(@types/node@20.11.5)(jsdom@24.1.0)(terser@5.27.0)
 
@@ -593,70 +593,70 @@
 
   '@types/urijs@1.19.25':
     resolution: {integrity: sha512-XOfUup9r3Y06nFAZh3WvO0rBU4OtlfPB/vgxpjg+NRdGU6CN6djdc6OEiH+PcqHCY6eFLo9Ista73uarf4gnBg==}
 
   '@types/warning@3.0.3':
     resolution: {integrity: sha512-D1XC7WK8K+zZEveUPY+cf4+kgauk8N4eHr/XIHXGlGYkHLud6hK9lYfZk1ry1TNh798cZUCgb6MqGEG8DkJt6Q==}
 
-  '@typescript-eslint/eslint-plugin@7.10.0':
-    resolution: {integrity: sha512-PzCr+a/KAef5ZawX7nbyNwBDtM1HdLIT53aSA2DDlxmxMngZ43O8SIePOeX8H5S+FHXeI6t97mTt/dDdzY4Fyw==}
+  '@typescript-eslint/eslint-plugin@7.11.0':
+    resolution: {integrity: sha512-P+qEahbgeHW4JQ/87FuItjBj8O3MYv5gELDzr8QaQ7fsll1gSMTYb6j87MYyxwf3DtD7uGFB9ShwgmCJB5KmaQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       '@typescript-eslint/parser': ^7.0.0
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/parser@7.10.0':
-    resolution: {integrity: sha512-2EjZMA0LUW5V5tGQiaa2Gys+nKdfrn2xiTIBLR4fxmPmVSvgPcKNW+AE/ln9k0A4zDUti0J/GZXMDupQoI+e1w==}
+  '@typescript-eslint/parser@7.11.0':
+    resolution: {integrity: sha512-yimw99teuaXVWsBcPO1Ais02kwJ1jmNA1KxE7ng0aT7ndr1pT1wqj0OJnsYVGKKlc4QJai86l/025L6z8CljOg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/scope-manager@7.10.0':
-    resolution: {integrity: sha512-7L01/K8W/VGl7noe2mgH0K7BE29Sq6KAbVmxurj8GGaPDZXPr8EEQ2seOeAS+mEV9DnzxBQB6ax6qQQ5C6P4xg==}
+  '@typescript-eslint/scope-manager@7.11.0':
+    resolution: {integrity: sha512-27tGdVEiutD4POirLZX4YzT180vevUURJl4wJGmm6TrQoiYwuxTIY98PBp6L2oN+JQxzE0URvYlzJaBHIekXAw==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/type-utils@7.10.0':
-    resolution: {integrity: sha512-D7tS4WDkJWrVkuzgm90qYw9RdgBcrWmbbRkrLA4d7Pg3w0ttVGDsvYGV19SH8gPR5L7OtcN5J1hTtyenO9xE9g==}
+  '@typescript-eslint/type-utils@7.11.0':
+    resolution: {integrity: sha512-WmppUEgYy+y1NTseNMJ6mCFxt03/7jTOy08bcg7bxJJdsM4nuhnchyBbE8vryveaJUf62noH7LodPSo5Z0WUCg==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/types@7.10.0':
-    resolution: {integrity: sha512-7fNj+Ya35aNyhuqrA1E/VayQX9Elwr8NKZ4WueClR3KwJ7Xx9jcCdOrLW04h51de/+gNbyFMs+IDxh5xIwfbNg==}
+  '@typescript-eslint/types@7.11.0':
+    resolution: {integrity: sha512-MPEsDRZTyCiXkD4vd3zywDCifi7tatc4K37KqTprCvaXptP7Xlpdw0NR2hRJTetG5TxbWDB79Ys4kLmHliEo/w==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
-  '@typescript-eslint/typescript-estree@7.10.0':
-    resolution: {integrity: sha512-LXFnQJjL9XIcxeVfqmNj60YhatpRLt6UhdlFwAkjNc6jSUlK8zQOl1oktAP8PlWFzPQC1jny/8Bai3/HPuvN5g==}
+  '@typescript-eslint/typescript-estree@7.11.0':
+    resolution: {integrity: sha512-cxkhZ2C/iyi3/6U9EPc5y+a6csqHItndvN/CzbNXTNrsC3/ASoYQZEt9uMaEp+xFNjasqQyszp5TumAVKKvJeQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       typescript: '*'
     peerDependenciesMeta:
       typescript:
         optional: true
 
-  '@typescript-eslint/utils@7.10.0':
-    resolution: {integrity: sha512-olzif1Fuo8R8m/qKkzJqT7qwy16CzPRWBvERS0uvyc+DHd8AKbO4Jb7kpAvVzMmZm8TrHnI7hvjN4I05zow+tg==}
+  '@typescript-eslint/utils@7.11.0':
+    resolution: {integrity: sha512-xlAWwPleNRHwF37AhrZurOxA1wyXowW4PqVXZVUNCLjB48CqdPJoJWkrpH2nij9Q3Lb7rtWindtoXwxjxlKKCA==}
     engines: {node: ^18.18.0 || >=20.0.0}
     peerDependencies:
       eslint: ^8.56.0
 
-  '@typescript-eslint/visitor-keys@7.10.0':
-    resolution: {integrity: sha512-9ntIVgsi6gg6FIq9xjEO4VQJvwOqA3jaBFQJ/6TK5AvEup2+cECI6Fh7QiBxmfMHXU0V0J4RyPeOU1VDNzl9cg==}
+  '@typescript-eslint/visitor-keys@7.11.0':
+    resolution: {integrity: sha512-7syYk4MzjxTEk0g/w3iqtgxnFQspDJfn6QKD36xMuuhTzjcxY7F8EmBLnALjVyaOF1/bVocu3bS/2/F7rXrveQ==}
     engines: {node: ^18.18.0 || >=20.0.0}
 
   '@ungap/structured-clone@1.2.0':
     resolution: {integrity: sha512-zuVdFrMJiuCDQUMCzQaD6KL28MjnqqN8XnAqiEq9PNm/hCPTSGfrXCOfwj1ow4LFb/tNymJPwsNbVePc1xFqrQ==}
 
   '@vitejs/plugin-react@4.3.0':
     resolution: {integrity: sha512-KcEbMsn4Dpk+LIbHMj7gDPRKaTMStxxWRkRmxsg/jVdFdJCZWt1SchZcf0M4t8lIKdwwMsEyzhrcOXRrDPtOBw==}
@@ -1097,16 +1097,16 @@
 
   eslint-plugin-react-hooks@4.6.2:
     resolution: {integrity: sha512-QzliNJq4GinDBcD8gPB5v0wh6g8q3SUi6EFF0x8N/BL9PoVs0atuGc47ozMRyOWAKdwaZ5OnbOEa3WR+dSGKuQ==}
     engines: {node: '>=10'}
     peerDependencies:
       eslint: ^3.0.0 || ^4.0.0 || ^5.0.0 || ^6.0.0 || ^7.0.0 || ^8.0.0-0
 
-  eslint-plugin-react@7.34.1:
-    resolution: {integrity: sha512-N97CxlouPT1AHt8Jn0mhhN2RrADlUAsk1/atcT2KyA/l9Q/E6ll7OIGwNumFmWfZ9skV3XXccYS19h80rHtgkw==}
+  eslint-plugin-react@7.34.2:
+    resolution: {integrity: sha512-2HCmrU+/JNigDN6tg55cRDKCQWicYAPB38JGSFDQt95jDm8rrvSUo7YPkOIm5l6ts1j1zCvysNcasvfTMQzUOw==}
     engines: {node: '>=4'}
     peerDependencies:
       eslint: ^3 || ^4 || ^5 || ^6 || ^7 || ^8
 
   eslint-scope@5.1.1:
     resolution: {integrity: sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==}
     engines: {node: '>=8.0.0'}
@@ -2278,16 +2278,16 @@
     hasBin: true
 
   vite-node@1.6.0:
     resolution: {integrity: sha512-de6HJgzC+TFzOu0NTC4RAIsyf/DY/ibWDYQUcuEA84EMHhcefTUGkjFHKKEJhQN4A+6I0u++kr3l36ZF2d7XRw==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
 
-  vite@5.2.11:
-    resolution: {integrity: sha512-HndV31LWW05i1BLPMUCE1B9E9GFbOu1MbenhS58FuK6owSO5qHm7GiCotrNY1YE5rMeQSFBGmT5ZaLEjFizgiQ==}
+  vite@5.2.12:
+    resolution: {integrity: sha512-/gC8GxzxMK5ntBwb48pR32GGhENnjtY30G4A0jemunsBkiEZFw60s8InGpN8gkhHEkjnRK1aSAxeQgwvFhUHAA==}
     engines: {node: ^18.0.0 || >=20.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': ^18.0.0 || >=20.0.0
       less: '*'
       lightningcss: ^1.21.0
       sass: '*'
@@ -2923,105 +2923,105 @@
 
   '@types/unist@2.0.10': {}
 
   '@types/urijs@1.19.25': {}
 
   '@types/warning@3.0.3': {}
 
-  '@typescript-eslint/eslint-plugin@7.10.0(@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/eslint-plugin@7.11.0(@typescript-eslint/parser@7.11.0(eslint@8.57.0)(typescript@5.4.5))(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/regexpp': 4.10.0
-      '@typescript-eslint/parser': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/scope-manager': 7.10.0
-      '@typescript-eslint/type-utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.10.0
+      '@typescript-eslint/parser': 7.11.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.11.0
+      '@typescript-eslint/type-utils': 7.11.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.11.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.11.0
       eslint: 8.57.0
       graphemer: 1.4.0
       ignore: 5.3.1
       natural-compare: 1.4.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/parser@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/parser@7.11.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/scope-manager': 7.10.0
-      '@typescript-eslint/types': 7.10.0
-      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
-      '@typescript-eslint/visitor-keys': 7.10.0
+      '@typescript-eslint/scope-manager': 7.11.0
+      '@typescript-eslint/types': 7.11.0
+      '@typescript-eslint/typescript-estree': 7.11.0(typescript@5.4.5)
+      '@typescript-eslint/visitor-keys': 7.11.0
       debug: 4.3.4
       eslint: 8.57.0
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/scope-manager@7.10.0':
+  '@typescript-eslint/scope-manager@7.11.0':
     dependencies:
-      '@typescript-eslint/types': 7.10.0
-      '@typescript-eslint/visitor-keys': 7.10.0
+      '@typescript-eslint/types': 7.11.0
+      '@typescript-eslint/visitor-keys': 7.11.0
 
-  '@typescript-eslint/type-utils@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/type-utils@7.11.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
-      '@typescript-eslint/utils': 7.10.0(eslint@8.57.0)(typescript@5.4.5)
+      '@typescript-eslint/typescript-estree': 7.11.0(typescript@5.4.5)
+      '@typescript-eslint/utils': 7.11.0(eslint@8.57.0)(typescript@5.4.5)
       debug: 4.3.4
       eslint: 8.57.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/types@7.10.0': {}
+  '@typescript-eslint/types@7.11.0': {}
 
-  '@typescript-eslint/typescript-estree@7.10.0(typescript@5.4.5)':
+  '@typescript-eslint/typescript-estree@7.11.0(typescript@5.4.5)':
     dependencies:
-      '@typescript-eslint/types': 7.10.0
-      '@typescript-eslint/visitor-keys': 7.10.0
+      '@typescript-eslint/types': 7.11.0
+      '@typescript-eslint/visitor-keys': 7.11.0
       debug: 4.3.4
       globby: 11.1.0
       is-glob: 4.0.3
       minimatch: 9.0.4
       semver: 7.6.0
       ts-api-utils: 1.3.0(typescript@5.4.5)
     optionalDependencies:
       typescript: 5.4.5
     transitivePeerDependencies:
       - supports-color
 
-  '@typescript-eslint/utils@7.10.0(eslint@8.57.0)(typescript@5.4.5)':
+  '@typescript-eslint/utils@7.11.0(eslint@8.57.0)(typescript@5.4.5)':
     dependencies:
       '@eslint-community/eslint-utils': 4.4.0(eslint@8.57.0)
-      '@typescript-eslint/scope-manager': 7.10.0
-      '@typescript-eslint/types': 7.10.0
-      '@typescript-eslint/typescript-estree': 7.10.0(typescript@5.4.5)
+      '@typescript-eslint/scope-manager': 7.11.0
+      '@typescript-eslint/types': 7.11.0
+      '@typescript-eslint/typescript-estree': 7.11.0(typescript@5.4.5)
       eslint: 8.57.0
     transitivePeerDependencies:
       - supports-color
       - typescript
 
-  '@typescript-eslint/visitor-keys@7.10.0':
+  '@typescript-eslint/visitor-keys@7.11.0':
     dependencies:
-      '@typescript-eslint/types': 7.10.0
+      '@typescript-eslint/types': 7.11.0
       eslint-visitor-keys: 3.4.3
 
   '@ungap/structured-clone@1.2.0': {}
 
-  '@vitejs/plugin-react@4.3.0(vite@5.2.11(@types/node@20.11.5)(terser@5.27.0))':
+  '@vitejs/plugin-react@4.3.0(vite@5.2.12(@types/node@20.11.5)(terser@5.27.0))':
     dependencies:
       '@babel/core': 7.24.5
       '@babel/plugin-transform-react-jsx-self': 7.24.5(@babel/core@7.24.5)
       '@babel/plugin-transform-react-jsx-source': 7.24.1(@babel/core@7.24.5)
       '@types/babel__core': 7.20.5
       react-refresh: 0.14.2
-      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.12(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
       - supports-color
 
   '@vitest/expect@1.6.0':
     dependencies:
       '@vitest/spy': 1.6.0
       '@vitest/utils': 1.6.0
@@ -3584,15 +3584,15 @@
 
   escape-string-regexp@4.0.0: {}
 
   eslint-plugin-react-hooks@4.6.2(eslint@8.57.0):
     dependencies:
       eslint: 8.57.0
 
-  eslint-plugin-react@7.34.1(eslint@8.57.0):
+  eslint-plugin-react@7.34.2(eslint@8.57.0):
     dependencies:
       array-includes: 3.1.8
       array.prototype.findlast: 1.2.5
       array.prototype.flatmap: 1.3.2
       array.prototype.toreversed: 1.1.2
       array.prototype.tosorted: 1.1.3
       doctrine: 2.1.0
@@ -4890,26 +4890,26 @@
 
   vite-node@1.6.0(@types/node@20.11.5)(terser@5.27.0):
     dependencies:
       cac: 6.7.14
       debug: 4.3.4
       pathe: 1.1.2
       picocolors: 1.0.0
-      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.12(@types/node@20.11.5)(terser@5.27.0)
     transitivePeerDependencies:
       - '@types/node'
       - less
       - lightningcss
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
 
-  vite@5.2.11(@types/node@20.11.5)(terser@5.27.0):
+  vite@5.2.12(@types/node@20.11.5)(terser@5.27.0):
     dependencies:
       esbuild: 0.20.2
       postcss: 8.4.38
       rollup: 4.17.2
     optionalDependencies:
       '@types/node': 20.11.5
       fsevents: 2.3.3
@@ -4930,15 +4930,15 @@
       magic-string: 0.30.10
       pathe: 1.1.2
       picocolors: 1.0.0
       std-env: 3.7.0
       strip-literal: 2.1.0
       tinybench: 2.8.0
       tinypool: 0.8.4
-      vite: 5.2.11(@types/node@20.11.5)(terser@5.27.0)
+      vite: 5.2.12(@types/node@20.11.5)(terser@5.27.0)
       vite-node: 1.6.0(@types/node@20.11.5)(terser@5.27.0)
       why-is-node-running: 2.2.2
     optionalDependencies:
       '@types/node': 20.11.5
       jsdom: 24.1.0
     transitivePeerDependencies:
       - less
```

### Comparing `bowtie_json_schema-2024.6.4/frontend/tsconfig.json` & `bowtie_json_schema-2024.6.5/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/public/favicon.svg` & `bowtie_json_schema-2024.6.5/frontend/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/DialectReportView.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/DialectReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/ReportDataHandler.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/ReportDataHandler.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/index.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/index.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/assets/landscape-logo.svg` & `bowtie_json_schema-2024.6.5/frontend/src/assets/landscape-logo.svg`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/CopyToClipboard.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/CopyToClipboard.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/FilterSection.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/FilterSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/NavBar.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/NavBar.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/OtherImplementations.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/OtherImplementations.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/BowtieInfo/BowtieInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseItem.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseItem.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseResultSvg.test.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseResultSvg.test.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CaseResultSvg.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CaseResultSvg.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Cases/CasesSection.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Cases/CasesSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Cases/SchemaDisplay.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Cases/SchemaDisplay.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/DragAndDrop/DragAndDrop.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/DragAndDrop/DragAndDrop.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/DialectCompliance.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/DialectCompliance.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/EmbedBadges.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/EmbedBadges.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/ImplementationReportView/ImplementationReportView.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Modals/DetailsButtonModal.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Modals/DetailsButtonModal.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/RunInfo/RunInfoSection.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/RunInfo/RunInfoSection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Summary/ImplementationRow.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Summary/ImplementationRow.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-import "./ImplementationRow.css";
 import { useContext, useState } from "react";
+import { useNavigate } from "react-router-dom";
+import Col from "react-bootstrap/Col";
+import Container from "react-bootstrap/Container";
+import OverlayTrigger from "react-bootstrap/OverlayTrigger";
+import Popover from "react-bootstrap/Popover";
+import Row from "react-bootstrap/Row";
+
 import { DetailsButtonModal } from "../Modals/DetailsButtonModal";
 import { mapLanguage } from "../../data/mapLanguage";
-import { useNavigate } from "react-router-dom";
 import {
   Case,
   Implementation,
   ImplementationResults,
 } from "../../data/parseReportData";
 import { ThemeContext } from "../../context/ThemeContext";
 
@@ -26,17 +31,18 @@
   const { isDarkMode } = useContext(ThemeContext);
   const [showDetails, setShowDetails] = useState(false);
   const navigate = useNavigate();
 
   return (
     <tr>
       <th
-        className="table-implementation-name align-middle p-0"
-        onClick={() => navigate(`/implementations/${id}`)}
         scope="row"
+        style={{ cursor: "pointer" }}
+        className="align-middle p-0"
+        onClick={() => navigate(`/implementations/${id}`)}
       >
         <span
           className={`text-decoration-underline ${
             isDarkMode ? "text-primary-emphasis" : "text-primary"
           }`}
         >
           {implementation.name}
@@ -47,34 +53,59 @@
       </th>
       <td className="align-middle d-none d-sm-table-cell">
         <small className="font-monospace text-muted">
           {implementation.version ?? ""}
         </small>
       </td>
 
-      <td className="text-center align-middle">
-        {implementationResults.totals.erroredCases}
-      </td>
-      <td className="text-center align-middle">
-        {implementationResults.totals.skippedTests}
-      </td>
-      <td className="text-center align-middle details-required">
-        {implementationResults.totals.failedTests! +
-          implementationResults.totals.erroredTests!}
-        <div className="hover-details text-center">
-          <p>
-            <b>failed</b>: &nbsp;{implementationResults.totals.failedTests}
-          </p>
-          <p>
-            <b>errored</b>: &nbsp;{implementationResults.totals.erroredTests}
-          </p>
-        </div>
-      </td>
+      <OverlayTrigger
+        placement="left-end"
+        overlay={
+          <Popover style={{ border: "1px solid var(--bs-primary)" }}>
+            <Popover.Body>
+              <Container className="p-0">
+                <Row className="d-flex flex-column gap-2">
+                  <Col>
+                    <h6 className="fw-bold mb-0">
+                      failed:&nbsp;
+                      <span className="fw-normal">
+                        {implementationResults.totals.failedTests}
+                      </span>
+                    </h6>
+                  </Col>
+                  <Col>
+                    <h6 className="fw-bold mb-0">
+                      errored:&nbsp;
+                      <span className="fw-normal">
+                        {implementationResults.totals.erroredTests}
+                      </span>
+                    </h6>
+                  </Col>
+                  <Col>
+                    <h6 className="fw-bold mb-0">
+                      skipped:&nbsp;
+                      <span className="fw-normal">
+                        {implementationResults.totals.skippedTests}
+                      </span>
+                    </h6>
+                  </Col>
+                </Row>
+              </Container>
+            </Popover.Body>
+          </Popover>
+        }
+      >
+        <td scope="row" colSpan={4} className="text-center">
+          {implementationResults.totals.failedTests! +
+            implementationResults.totals.erroredTests! +
+            implementationResults.totals.skippedTests!}
+        </td>
+      </OverlayTrigger>
 
-      <td className="align-middle p-0">
+      <td scope="row" colSpan={4} className="align-middle p-0">
         {implementationResults.totals.failedTests! +
           implementationResults.totals.erroredTests! +
           implementationResults.totals.skippedTests! >
           0 && (
           <button
             type="button"
             className="btn btn-sm btn-primary"
```

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/components/Summary/SummarySection.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/components/Summary/SummarySection.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/context/BowtieVersionContext.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/context/BowtieVersionContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/context/ThemeContext.tsx` & `bowtie_json_schema-2024.6.5/frontend/src/context/ThemeContext.tsx`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/Badge.test.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/Badge.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/Badge.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/Badge.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/Dialect.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/Dialect.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/Site.test.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/Site.test.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/parseReportData.test.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/parseReportData.test.ts`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,14 @@
         {},
       ),
       implementationsResults: new Map([
         [
           tag("envsonschema"),
           {
             totals: {
-              erroredCases: 0,
               erroredTests: 0,
               skippedTests: 0,
               failedTests: 1,
             },
             caseResults: new Map([[1, [{ state: "failed", valid: false }]]]),
           },
         ],
@@ -225,15 +224,14 @@
         {},
       ),
       implementationsResults: new Map([
         [
           tag("envsonschema"),
           {
             totals: {
-              erroredCases: 0,
               erroredTests: 0,
               skippedTests: 0,
               failedTests: 4,
             },
             caseResults: new Map([
               [
                 1,
```

### Comparing `bowtie_json_schema-2024.6.4/frontend/src/data/parseReportData.ts` & `bowtie_json_schema-2024.6.5/frontend/src/data/parseReportData.ts`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,14 @@
   const runMetadata = RunMetadata.fromRecord(lines[0] as unknown as Header);
 
   const implementationsResultsMap = new Map<string, ImplementationResults>();
   for (const id of runMetadata.implementations.keys()) {
     implementationsResultsMap.set(id, {
       caseResults: new Map(),
       totals: {
-        erroredCases: 0,
         skippedTests: 0,
         failedTests: 0,
         erroredTests: 0,
       },
     });
   }
 
@@ -91,15 +90,14 @@
       const implementationResults = implementationsResultsMap.get(
         line.implementation as string,
       )!;
       if (line.caught !== undefined) {
         const context = line.context as Record<string, unknown>;
         const errorMessage: string = (context?.message ??
           context?.stderr) as string;
-        implementationResults.totals.erroredCases!++;
         implementationResults.totals.erroredTests! += caseData.tests.length;
         implementationResults.caseResults.set(
           line.seq as number,
           new Array<CaseResult>(caseData.tests.length).fill({
             state: "errored",
             message: errorMessage,
           }),
@@ -232,22 +230,20 @@
   const totalTests = Array.from(data.cases.values()).reduce(
     (prev, curr) => prev + curr.tests.length,
     0,
   );
   return Array.from(data.implementationsResults.values()).reduce(
     (prev, curr) => ({
       totalTests,
-      erroredCases: prev.erroredCases + curr.totals.erroredCases!,
       skippedTests: prev.skippedTests + curr.totals.skippedTests!,
       failedTests: prev.failedTests + curr.totals.failedTests!,
       erroredTests: prev.erroredTests + curr.totals.erroredTests!,
     }),
     {
       totalTests: totalTests,
-      erroredCases: 0,
       skippedTests: 0,
       failedTests: 0,
       erroredTests: 0,
     },
   );
 };
 
@@ -261,15 +257,14 @@
   metadata: Record<string, unknown>;
   implementations: Record<string, ImplementationData>;
   started: number;
 }
 
 export interface Totals {
   totalTests: number;
-  erroredCases: number;
   skippedTests: number;
   failedTests: number;
   erroredTests: number;
 }
 
 export interface ReportData {
   runMetadata: RunMetadata;
```

### Comparing `bowtie_json_schema-2024.6.4/implementations/.java-implementations-pmd-ruleset.xml` & `bowtie_json_schema-2024.6.5/implementations/.java-implementations-pmd-ruleset.xml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/clojure-json-schema/Dockerfile` & `bowtie_json_schema-2024.6.5/implementations/clojure-json-schema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj` & `bowtie_json_schema-2024.6.5/implementations/clojure-json-schema/src/bowtie_json_schema/core.clj`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/cpp-valijson/bowtie_valijson.cpp` & `bowtie_json_schema-2024.6.5/implementations/cpp-valijson/bowtie_valijson.cpp`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/.editorconfig` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/.editorconfig`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/.gitignore` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/Program.cs` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/bowtie_corvus_jsonschema.csproj`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
   <ItemGroup>
     <PackageReference Include="Corvus.Json.CodeGeneration.201909" Version="3.0.25" />
     <PackageReference Include="Corvus.Json.CodeGeneration.202012" Version="3.0.25" />
     <PackageReference Include="Corvus.Json.CodeGeneration.4" Version="3.0.25" />
     <PackageReference Include="Corvus.Json.CodeGeneration.6" Version="3.0.25" />
     <PackageReference Include="Corvus.Json.CodeGeneration.7" Version="3.0.25" />
-    <PackageReference Include="Corvus.Json.ExtendedTypes" Version="3.0.25" />
+    <PackageReference Include="Corvus.Json.ExtendedTypes" Version="3.0.26" />
     <PackageReference Include="Microsoft.Extensions.Configuration.Json" Version="8.0.0" />
     <PackageReference Include="Microsoft.CodeAnalysis.CSharp" Version="4.9.2" />
     <PackageReference Include="Microsoft.Extensions.DependencyModel" Version="8.0.0" />
 
   </ItemGroup>
 
   <ItemGroup>
```

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/core.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2019-09/meta/validation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/applicator.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/core.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/hyper-schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/meta-data.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft2020-12/meta/validation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft4/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft6/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json` & `bowtie_json_schema-2024.6.5/implementations/dotnet-corvus-jsonschema/metaschema/draft7/schema.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/.gitignore` & `bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/dotnet-jsonschema-net/Program.cs` & `bowtie_json_schema-2024.6.5/implementations/dotnet-jsonschema-net/Program.cs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/bowtie_gojsonschema.go` & `bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/bowtie_gojsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/go-gojsonschema/go.sum` & `bowtie_json_schema-2024.6.5/implementations/go-gojsonschema/go.sum`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/go-jsonschema/bowtie_jsonschema.go` & `bowtie_json_schema-2024.6.5/implementations/go-jsonschema/bowtie_jsonschema.go`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-json-schema/BowtieJsonSchema.java` & `bowtie_json_schema-2024.6.5/implementations/java-json-schema/BowtieJsonSchema.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-json-schema/build.gradle` & `bowtie_json_schema-2024.6.5/implementations/java-json-schema/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.5/implementations/java-json-tools-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-json-tools-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.5/implementations/java-json-tools-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java` & `bowtie_json_schema-2024.6.5/implementations/java-jsonschemafriend/BowtieJsonSchemaFriend.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-jsonschemafriend/build.gradle` & `bowtie_json_schema-2024.6.5/implementations/java-jsonschemafriend/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java` & `bowtie_json_schema-2024.6.5/implementations/java-networknt-json-schema-validator/BowtieJsonSchemaValidator.java`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-networknt-json-schema-validator/build.gradle` & `bowtie_json_schema-2024.6.5/implementations/java-networknt-json-schema-validator/build.gradle`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/build.gradle.kts` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/justfile` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/justfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/gradle/libs.versions.toml` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/gradle/libs.versions.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/Runner.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/Support.kt` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/Support.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/Request.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/RunCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt` & `bowtie_json_schema-2024.6.5/implementations/java-openapiprocessor/src/main/kotlin/commands/StartCmd.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-ajv/bowtie_ajv.js` & `bowtie_json_schema-2024.6.5/implementations/js-ajv/bowtie_ajv.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-ajv/package-lock.json` & `bowtie_json_schema-2024.6.5/implementations/js-ajv/package-lock.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-hyperjump/bowtie_hyperjump.js` & `bowtie_json_schema-2024.6.5/implementations/js-hyperjump/bowtie_hyperjump.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-json-schema/bowtie_json_schema.js` & `bowtie_json_schema-2024.6.5/implementations/js-json-schema/bowtie_json_schema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-jsonschema/bowtie_jsonschema.js` & `bowtie_json_schema-2024.6.5/implementations/js-jsonschema/bowtie_jsonschema.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/js-schemasafe/bowtie_schemasafe.js` & `bowtie_json_schema-2024.6.5/implementations/js-schemasafe/bowtie_schemasafe.js`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts` & `bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/build.gradle.kts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt` & `bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/BowtieSampsonSchemaValidatorLauncher.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt` & `bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Commands.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt` & `bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/Responses.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt` & `bowtie_json_schema-2024.6.5/implementations/kotlin-kmp-json-schema-validator/src/main/kotlin/TestFilters.kt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/bowtie_jsonschema.lua` & `bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/bowtie_jsonschema.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/lua-jsonschema/json.lua` & `bowtie_json_schema-2024.6.5/implementations/lua-jsonschema/json.lua`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/php-opis-json-schema/bowtieJsonSchema.php` & `bowtie_json_schema-2024.6.5/implementations/php-opis-json-schema/bowtieJsonSchema.php`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/python-fastjsonschema/bowtie_fastjsonschema.py` & `bowtie_json_schema-2024.6.5/implementations/python-fastjsonschema/bowtie_fastjsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/python-jschon/bowtie_jschon.py` & `bowtie_json_schema-2024.6.5/implementations/python-jschon/bowtie_jschon.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/python-jsonschema/bowtie_jsonschema.py` & `bowtie_json_schema-2024.6.5/implementations/python-jsonschema/bowtie_jsonschema.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/ruby-json_schemer/bowtie_json_schemer.rb` & `bowtie_json_schema-2024.6.5/implementations/ruby-json_schemer/bowtie_json_schemer.rb`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-boon/Cargo.lock` & `bowtie_json_schema-2024.6.5/implementations/rust-boon/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-boon/Dockerfile` & `bowtie_json_schema-2024.6.5/implementations/rust-boon/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-boon/src/main.rs` & `bowtie_json_schema-2024.6.5/implementations/rust-boon/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/Cargo.lock` & `bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/Cargo.lock`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/Dockerfile` & `bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/Dockerfile`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/rust-jsonschema/src/main.rs` & `bowtie_json_schema-2024.6.5/implementations/rust-jsonschema/src/main.rs`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/Harness.scala` & `bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/scala-mjs-validator/build.sbt` & `bowtie_json_schema-2024.6.5/implementations/scala-mjs-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/Harness.scala` & `bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/Harness.scala`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/scala-rc-circe-json-validator/build.sbt` & `bowtie_json_schema-2024.6.5/implementations/scala-rc-circe-json-validator/build.sbt`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts` & `bowtie_json_schema-2024.6.5/implementations/ts-vscode-json-languageservice/bowtie_jsonls.ts`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_cli.py` & `bowtie_json_schema-2024.6.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_connectables.py` & `bowtie_json_schema-2024.6.5/tests/test_connectables.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from bowtie._connectables import Connectable, UnknownConnector
 from bowtie._containers import (
     IMAGE_REPOSITORY,
     ConnectableContainer,
     ConnectableImage,
 )
 from bowtie._core import validator_registry
-from bowtie._direct_connectable import Direct
+from bowtie._direct_connectable import Direct, NoDirectConnection
 
 validator = validator_registry().for_uri(
     "tag:bowtie.report,2024:connectables",
 )
 
 
 def test_explicit_image_with_repository():
@@ -123,22 +123,22 @@
     connectable = Connectable.from_str(id)
     assert connectable == Connectable(
         id=id,
         connector=ConnectableContainer(id="c7895a98f49d"),
     )
 
 
-def test_direct_connectable_jsonschema():
-    id = "direct:jsonschema"
+def test_direct_connectable_python_jsonschema():
+    id = "direct:python-jsonschema"
     validator.validate(id)
     connectable = Connectable.from_str(id)
     assert connectable == Connectable(
         id=id,
-        connector=Direct(id="jsonschema"),
+        connector=Direct(id="python-jsonschema"),
     )
 
 
 def test_direct_connectable_unknown():
     id = "direct:foobar"
     validator.validate(id)
-    with pytest.raises(ValueError, match="'jsonschema'"):
+    with pytest.raises(NoDirectConnection, match="'foobar'"):
         Connectable.from_str(id)
```

### Comparing `bowtie_json_schema-2024.6.4/tests/test_github.py` & `bowtie_json_schema-2024.6.5/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_hypothesis.py` & `bowtie_json_schema-2024.6.5/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_integration.py` & `bowtie_json_schema-2024.6.5/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2448,21 +2448,26 @@
 async def test_direct_connectable_python_jsonschema(tmp_path):
     tmp_path.joinpath("schema.json").write_text("{}")
     tmp_path.joinpath("instance.json").write_text("12")
 
     stdout, stderr = await bowtie(
         "validate",
         "-i",
-        "direct:jsonschema",
+        "direct:python-jsonschema",
         tmp_path / "schema.json",
         tmp_path / "instance.json",
         exit_code=0,
     )
     assert stderr == ""
 
     report = Report.from_serialized(stdout.splitlines())
     assert [
         [test_results for _, test_results in results]
         for _, results in report.cases_with_results()
     ] == [
-        [{"direct:jsonschema": TestResult.VALID}],
+        [{"direct:python-jsonschema": TestResult.VALID}],
     ], stderr
+
+
+@pytest.mark.asyncio
+async def test_smoke_direct_connectable_jsonschema():
+    await bowtie("smoke", "-i", "direct:python-jsonschema", exit_code=0)
```

### Comparing `bowtie_json_schema-2024.6.4/tests/test_registry.py` & `bowtie_json_schema-2024.6.5/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_report.py` & `bowtie_json_schema-2024.6.5/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/test_schemas.py` & `bowtie_json_schema-2024.6.5/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/envsonschema/envsonschema` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/envsonschema/envsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/lintsonschema` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/lintsonschema`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/connectables.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/connectables.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/report.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/report.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/info.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/info.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/smoke.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/statistics.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/cli/summary.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/v1.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/v1.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/run.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/io/commands/start.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/dialect.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/group.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/group.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/implementation.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/tests/fauxmplementations/lintsonschema/schemas/models/test.json` & `bowtie_json_schema-2024.6.5/tests/fauxmplementations/lintsonschema/schemas/models/test.json`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/.gitignore` & `bowtie_json_schema-2024.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/LICENSE` & `bowtie_json_schema-2024.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/README.rst` & `bowtie_json_schema-2024.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/hatch_build.py` & `bowtie_json_schema-2024.6.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/pyproject.toml` & `bowtie_json_schema-2024.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bowtie_json_schema-2024.6.4/PKG-INFO` & `bowtie_json_schema-2024.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bowtie-json-schema
-Version: 2024.6.4
+Version: 2024.6.5
 Summary: A meta-validator for the JSON Schema specification.
 Project-URL: Documentation, https://docs.bowtie.report/
 Project-URL: Homepage, https://bowtie.report/
 Project-URL: Issues, https://github.com/bowtie-json-schema/bowtie/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/bowtie-json-schema/bowtie
 Author-email: Julian Berman <Julian+bowtie@GrayVines.com>
```

