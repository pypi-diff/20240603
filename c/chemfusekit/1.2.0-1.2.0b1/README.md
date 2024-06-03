# Comparing `tmp/chemfusekit-1.2.0.tar.gz` & `tmp/chemfusekit-1.2.0b1.tar.gz`

## Comparing `chemfusekit-1.2.0.tar` & `chemfusekit-1.2.0b1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.python-version
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.releaserc.yml
--rw-r--r--   0        0        0    18131 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/requirements.lock
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.github/workflows/gh_pages.yml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.github/workflows/thesis.yml
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/__init__.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/__utils.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/knn.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/lda.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/lldf.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/lr.py
--rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/pca.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/plsda.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/chemfusekit/svm.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/babel.config.js
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docusaurus.config.js
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/package.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/sidebars.js
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versions.json
--rw-r--r--   0        0        0   427555 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/yarn.lock
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/complete-workflow.md
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/knn/knn.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lda/lda.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lda/ldasettings.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/_category_.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/index.mdx
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/lldf-class.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/lldfmodel.md
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/lldfsettings.md
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lldf/table.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lr/lr.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/pca/pca.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/plsda/plsda.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/svm/svm.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/svm/svmsettings.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/_category_.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/graphmode.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/graphoutput.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/printconfusionmatrix.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/printtable.md
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/docs/utils/runsplittests.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/css/custom.css
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/index.module.css
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/_category_.json
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/continuous-integration.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/index.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/process-model.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/project-philosophy.md
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/project-plan.md
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/requirements-specification.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/src/pages/project/use-cases.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/.nojekyll
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/colab-logo.svg
--rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/happy-woman.svg
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/logo.svg
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/static/img/magnifying-glass.svg
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/complete-workflow.md
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/knn/knn.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lda/lda.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lr/lr.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/pca/pca.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/plsda/plsda.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/svm/svm.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/svm/svmsettings.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/_category_.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/graphmode.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/graphoutput.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/printconfusionmatrix.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/printtable.md
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/runsplittests.md
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/complete-workflow.md
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/knn/knn.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lda/lda.md
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lr/lr.md
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/pca/pca.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/plsda/plsda.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/svm/svm.md
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/svm/svmsettings.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/_category_.json
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/graphmode.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/graphoutput.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/printconfusionmatrix.md
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/printtable.md
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/runsplittests.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_sidebars/version-1.1.3-sidebars.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/docs/versioned_sidebars/version-1.2-sidebars.json
--rw-r--r--   0        0        0   241944 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/examples/knn_notebook.ipynb
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/examples/pca_lda_notebook.ipynb
--rw-r--r--   0        0        0  1664192 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/examples/pca_lr_notebook.ipynb
--rw-r--r--   0        0        0   533669 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/examples/plsda_notebook.ipynb
--rw-r--r--   0        0        0   176363 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/examples/svm_notebook.ipynb
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Beartype.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Constructors.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Conventional Commits.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Kanban.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Logistic Regression.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/PCA-LR.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/PCA.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/PEP coding standards.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/SVM.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/To do.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Use Case Diagram.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/kNN.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/app.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/appearance.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/community-plugins.json
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/core-plugins.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/daily-notes.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/templates.json
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/workspace.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/calendar/data.json
--rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/calendar/main.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/calendar/manifest.json
--rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-kanban/main.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-kanban/manifest.json
--rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-kanban/styles.css
--rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-plantuml/main.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-plantuml/styles.css
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-04-19.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-04-20.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-04-22.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-04-23.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-06.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-07.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-08.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-09.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-17.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Devlog/2024-05-18.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/Templates/Daily devlog.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/UML/Components.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/UML/Process state machine.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/UML/Sequence.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/notes/UML/Use cases.md
--rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/qepas.xlsx
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/rt.xlsx
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_knn.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_lda.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_lldf.py
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_lr.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_pca.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_plsda.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/tests/test_svm.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/0-header.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/1-abstract.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/2-index.md.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/3-intro.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/999-ringraziamenti.md
--rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/thesis/logo-unibg.png
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/.gitignore
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/readme.md
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 chemfusekit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.python-version
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.releaserc.yml
+-rw-r--r--   0        0        0    14847 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/requirements-dev.lock
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/requirements.lock
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.github/workflows/gh_pages.yml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.github/workflows/thesis.yml
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/__utils.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/knn.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/lda.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/lldf.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/lr.py
+-rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/pca.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/plsda.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/chemfusekit/svm.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/babel.config.js
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docusaurus.config.js
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/package.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/sidebars.js
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versions.json
+-rw-r--r--   0        0        0   427555 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/yarn.lock
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/complete-workflow.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/knn/knn.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lda/lda.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lda/ldasettings.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/_category_.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/index.mdx
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/lldf-class.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/lldfmodel.md
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lldf/table.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lr/lr.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/pca/pca.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/plsda/plsda.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/svm/svm.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/svm/svmsettings.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/_category_.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/graphmode.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/graphoutput.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/printconfusionmatrix.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/printtable.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/docs/utils/runsplittests.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/_category_.json
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/continuous-integration.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/index.md
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/process-model.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/project-philosophy.md
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/project-plan.md
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/requirements-specification.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/src/pages/project/use-cases.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/.nojekyll
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/colab-logo.svg
+-rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/happy-woman.svg
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/static/img/magnifying-glass.svg
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/complete-workflow.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/knn/knn.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lda/lda.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lr/lr.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/pca/pca.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/plsda/plsda.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/svm/svm.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/svm/svmsettings.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/_category_.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/graphmode.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/graphoutput.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/printconfusionmatrix.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/printtable.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/runsplittests.md
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/complete-workflow.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/knn/knn.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lda/lda.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lr/lr.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/pca/pca.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/plsda/plsda.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/svm/svm.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/svm/svmsettings.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/_category_.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/graphmode.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/graphoutput.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/printconfusionmatrix.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/printtable.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/runsplittests.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_sidebars/version-1.1.3-sidebars.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/docs/versioned_sidebars/version-1.2-sidebars.json
+-rw-r--r--   0        0        0   241944 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/examples/knn_notebook.ipynb
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/examples/pca_lda_notebook.ipynb
+-rw-r--r--   0        0        0  1664192 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/examples/pca_lr_notebook.ipynb
+-rw-r--r--   0        0        0   533669 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/examples/plsda_notebook.ipynb
+-rw-r--r--   0        0        0   176363 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/examples/svm_notebook.ipynb
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Beartype.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Constructors.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Conventional Commits.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Kanban.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Logistic Regression.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/PCA-LR.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/PCA.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/PEP coding standards.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/SVM.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/To do.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Use Case Diagram.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/kNN.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/app.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/appearance.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/community-plugins.json
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/daily-notes.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/templates.json
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/workspace.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/calendar/data.json
+-rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/calendar/main.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/calendar/manifest.json
+-rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-kanban/main.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-kanban/manifest.json
+-rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-kanban/styles.css
+-rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-plantuml/main.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-04-19.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-04-20.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-04-22.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-04-23.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-06.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-07.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-08.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-09.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-17.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Devlog/2024-05-18.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/Templates/Daily devlog.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/UML/Components.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/UML/Process state machine.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/UML/Sequence.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/notes/UML/Use cases.md
+-rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/qepas.xlsx
+-rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/rt.xlsx
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_knn.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_lda.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_lldf.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_lr.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_pca.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_plsda.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/tests/test_svm.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/0-header.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/1-abstract.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/2-index.md.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/3-intro.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/999-ringraziamenti.md
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/thesis/logo-unibg.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/readme.md
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 chemfusekit-1.2.0b1/PKG-INFO
```

### Comparing `chemfusekit-1.2.0/.releaserc.yml` & `chemfusekit-1.2.0b1/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/CHANGELOG.md` & `chemfusekit-1.2.0b1/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,7 @@
-## [1.2.0](https://github.com/f-aguzzi/tesi/compare/v1.1.3...v1.2.0) (2024-06-03)
-
-
-### Features
-
-* graphing and multi-table in LLDF ([c450767](https://github.com/f-aguzzi/tesi/commit/c4507672fb502dfd5d9b0994ff461387ff5a3acc))
-
-
-### Bug Fixes
-
-* docs workflow, dependency clashes, demos ([a994940](https://github.com/f-aguzzi/tesi/commit/a994940a6bf115ea02054754fb3b237977a4e3aa)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* docs workflow, dependency clashes, demos ([6f72ec4](https://github.com/f-aguzzi/tesi/commit/6f72ec4a0c51902e05e468b6d6f79042a3bc73e5)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* gh pages workflow ([49c6bda](https://github.com/f-aguzzi/tesi/commit/49c6bdabf757073e87e0c7b0c98eb4d0ef843f78))
-
-
-### Docs
-
-* add documentation versioning [skip ci] ([ee0b7ab](https://github.com/f-aguzzi/tesi/commit/ee0b7ab915501d30d12ed6542535434265f0bd61))
-* added version 1.2 ([3fcd0cc](https://github.com/f-aguzzi/tesi/commit/3fcd0cc7abdb5daa201c74ba959340711506e1f0))
-
-
-### CI
-
-* **release:** 1.1.1-beta.2 [skip ci] ([a0519e7](https://github.com/f-aguzzi/tesi/commit/a0519e71d2bc75830ce027bdb11589a0762905a8)), closes [#25](https://github.com/f-aguzzi/tesi/issues/25)
-* **release:** 1.1.1-beta.3 [skip ci] ([4dc43c6](https://github.com/f-aguzzi/tesi/commit/4dc43c6f2e7ec6e34e6adfb5ad1b2aacaa3731e2)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* **release:** 1.1.2-beta.1 [skip ci] ([a903084](https://github.com/f-aguzzi/tesi/commit/a9030846e88a15dfd9ec8a9418e59098ef4e439c)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#25](https://github.com/f-aguzzi/tesi/issues/25) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* **release:** 1.1.2-beta.2 [skip ci] ([c23bcb0](https://github.com/f-aguzzi/tesi/commit/c23bcb0e833ed10ff7665f56edd82c0617152156)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* **release:** 1.1.2-beta.3 [skip ci] ([0bcdf85](https://github.com/f-aguzzi/tesi/commit/0bcdf851d60b16c3e4ced0f562149490d6bcbcbe))
-* **release:** 1.1.4-beta.1 [skip ci] ([d1e06cc](https://github.com/f-aguzzi/tesi/commit/d1e06cc4238c3e4f1b86ce4e8ab7e3eac6c5d1c6)), closes [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#25](https://github.com/f-aguzzi/tesi/issues/25) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#25](https://github.com/f-aguzzi/tesi/issues/25) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28) [#29](https://github.com/f-aguzzi/tesi/issues/29) [#28](https://github.com/f-aguzzi/tesi/issues/28)
-* **release:** 1.2.0-beta.1 [skip ci] ([b08fa39](https://github.com/f-aguzzi/tesi/commit/b08fa3970d537a19072b70edb2275488d160d69f))
-
 ## [1.2.0-beta.1](https://github.com/f-aguzzi/tesi/compare/v1.1.4-beta.1...v1.2.0-beta.1) (2024-06-03)
 
 
 ### Features
 
 * graphing and multi-table in LLDF ([c450767](https://github.com/f-aguzzi/tesi/commit/c4507672fb502dfd5d9b0994ff461387ff5a3acc))
```

### Comparing `chemfusekit-1.2.0/requirements-dev.lock` & `chemfusekit-1.2.0b1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/requirements.lock` & `chemfusekit-1.2.0b1/requirements.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/.github/workflows/gh_pages.yml` & `chemfusekit-1.2.0b1/.github/workflows/gh_pages.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/.github/workflows/pylint.yml` & `chemfusekit-1.2.0b1/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/.github/workflows/release.yml` & `chemfusekit-1.2.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/.github/workflows/thesis.yml` & `chemfusekit-1.2.0b1/.github/workflows/thesis.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/.github/workflows/unittest.yml` & `chemfusekit-1.2.0b1/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/__utils.py` & `chemfusekit-1.2.0b1/chemfusekit/__utils.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/knn.py` & `chemfusekit-1.2.0b1/chemfusekit/knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/lda.py` & `chemfusekit-1.2.0b1/chemfusekit/lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/lldf.py` & `chemfusekit-1.2.0b1/chemfusekit/lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/lr.py` & `chemfusekit-1.2.0b1/chemfusekit/lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/pca.py` & `chemfusekit-1.2.0b1/chemfusekit/pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/plsda.py` & `chemfusekit-1.2.0b1/chemfusekit/plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/chemfusekit/svm.py` & `chemfusekit-1.2.0b1/chemfusekit/svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/README.md` & `chemfusekit-1.2.0b1/docs/README.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docusaurus.config.js` & `chemfusekit-1.2.0b1/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/package.json` & `chemfusekit-1.2.0b1/docs/package.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/sidebars.js` & `chemfusekit-1.2.0b1/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/yarn.lock` & `chemfusekit-1.2.0b1/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/complete-workflow.md` & `chemfusekit-1.2.0b1/docs/docs/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/tutorial.md` & `chemfusekit-1.2.0b1/docs/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/knn/knn.md` & `chemfusekit-1.2.0b1/docs/docs/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/knn/knnsettings.md` & `chemfusekit-1.2.0b1/docs/docs/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lda/lda.md` & `chemfusekit-1.2.0b1/docs/docs/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lda/ldasettings.md` & `chemfusekit-1.2.0b1/docs/docs/lda/ldasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lldf/index.mdx` & `chemfusekit-1.2.0b1/docs/docs/lldf/index.mdx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lldf/lldf-class.md` & `chemfusekit-1.2.0b1/docs/docs/lldf/lldf-class.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lldf/table.md` & `chemfusekit-1.2.0b1/docs/docs/lldf/table.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lr/lr.md` & `chemfusekit-1.2.0b1/docs/docs/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/lr/lrsettings.md` & `chemfusekit-1.2.0b1/docs/docs/lr/lrsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/pca/pca.md` & `chemfusekit-1.2.0b1/docs/docs/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/pca/pcasettings.md` & `chemfusekit-1.2.0b1/docs/docs/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/plsda/plsda.md` & `chemfusekit-1.2.0b1/docs/docs/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/plsda/plsdasettings.md` & `chemfusekit-1.2.0b1/docs/docs/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/svm/svm.md` & `chemfusekit-1.2.0b1/docs/docs/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/svm/svmsettings.md` & `chemfusekit-1.2.0b1/docs/docs/svm/svmsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/docs/utils/graphoutput.md` & `chemfusekit-1.2.0b1/docs/docs/utils/graphoutput.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/components/HomepageFeatures/index.js` & `chemfusekit-1.2.0b1/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/css/custom.css` & `chemfusekit-1.2.0b1/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/index.js` & `chemfusekit-1.2.0b1/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/continuous-integration.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/continuous-integration.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/index.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/index.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/process-model.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/process-model.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/project-philosophy.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/project-philosophy.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/project-plan.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/project-plan.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/requirements-specification.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/requirements-specification.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/src/pages/project/use-cases.md` & `chemfusekit-1.2.0b1/docs/src/pages/project/use-cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/colab-logo.svg` & `chemfusekit-1.2.0b1/docs/static/img/colab-logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/docusaurus-social-card.jpg` & `chemfusekit-1.2.0b1/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/docusaurus.png` & `chemfusekit-1.2.0b1/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/favicon.ico` & `chemfusekit-1.2.0b1/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/happy-woman.svg` & `chemfusekit-1.2.0b1/docs/static/img/happy-woman.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/logo.svg` & `chemfusekit-1.2.0b1/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/static/img/magnifying-glass.svg` & `chemfusekit-1.2.0b1/docs/static/img/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/complete-workflow.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/tutorial.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/knn/knn.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/knn/knnsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lda/lda.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lda/ldasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lda/ldasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/lldf.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lldf/lldfsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lldf/lldfsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lr/lr.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/lr/lrsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/lr/lrsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/pca/pca.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/pca/pcasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/plsda/plsda.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/plsda/plsdasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/svm/svm.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/svm/svmsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/svm/svmsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.1.3/utils/graphoutput.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.1.3/utils/graphoutput.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/complete-workflow.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/tutorial.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/tutorial.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/knn/knn.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/knn/knnsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/knn/knnsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lda/lda.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lda/ldasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lda/ldasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/lldf.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lldf/lldfsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lldf/lldfsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lr/lr.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/lr/lrsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/lr/lrsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/pca/pca.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/pca/pcasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/pca/pcasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/plsda/plsda.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/plsda/plsdasettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/plsda/plsdasettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/svm/svm.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/svm/svmsettings.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/svm/svmsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/docs/versioned_docs/version-1.2/utils/graphoutput.md` & `chemfusekit-1.2.0b1/docs/versioned_docs/version-1.2/utils/graphoutput.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/examples/knn_notebook.ipynb` & `chemfusekit-1.2.0b1/examples/knn_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/examples/pca_lda_notebook.ipynb` & `chemfusekit-1.2.0b1/examples/pca_lda_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/examples/pca_lr_notebook.ipynb` & `chemfusekit-1.2.0b1/examples/pca_lr_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/examples/plsda_notebook.ipynb` & `chemfusekit-1.2.0b1/examples/plsda_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/examples/svm_notebook.ipynb` & `chemfusekit-1.2.0b1/examples/svm_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Beartype.md` & `chemfusekit-1.2.0b1/notes/Beartype.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Constructors.md` & `chemfusekit-1.2.0b1/notes/Constructors.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Conventional Commits.md` & `chemfusekit-1.2.0b1/notes/Conventional Commits.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Kanban.md` & `chemfusekit-1.2.0b1/notes/Kanban.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Use Case Diagram.md` & `chemfusekit-1.2.0b1/notes/Use Case Diagram.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/core-plugins-migration.json` & `chemfusekit-1.2.0b1/notes/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/workspace.json` & `chemfusekit-1.2.0b1/notes/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/plugins/calendar/main.js` & `chemfusekit-1.2.0b1/notes/.obsidian/plugins/calendar/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-kanban/main.js` & `chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-kanban/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-kanban/styles.css` & `chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-kanban/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-plantuml/main.js` & `chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-plantuml/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/.obsidian/plugins/obsidian-plantuml/styles.css` & `chemfusekit-1.2.0b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-04-19.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-04-19.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-04-20.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-04-20.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-04-22.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-04-22.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-04-23.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-04-23.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-06.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-06.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-07.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-07.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-08.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-08.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-09.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-09.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-17.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-17.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/Devlog/2024-05-18.md` & `chemfusekit-1.2.0b1/notes/Devlog/2024-05-18.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/UML/Process state machine.md` & `chemfusekit-1.2.0b1/notes/UML/Process state machine.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/UML/Sequence.md` & `chemfusekit-1.2.0b1/notes/UML/Sequence.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/notes/UML/Use cases.md` & `chemfusekit-1.2.0b1/notes/UML/Use cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/qepas.xlsx` & `chemfusekit-1.2.0b1/tests/qepas.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/rt.xlsx` & `chemfusekit-1.2.0b1/tests/rt.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_knn.py` & `chemfusekit-1.2.0b1/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_lda.py` & `chemfusekit-1.2.0b1/tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_lldf.py` & `chemfusekit-1.2.0b1/tests/test_lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_lr.py` & `chemfusekit-1.2.0b1/tests/test_lr.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_pca.py` & `chemfusekit-1.2.0b1/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_plsda.py` & `chemfusekit-1.2.0b1/tests/test_plsda.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/tests/test_svm.py` & `chemfusekit-1.2.0b1/tests/test_svm.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/thesis/0-header.md` & `chemfusekit-1.2.0b1/thesis/0-header.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/thesis/1-abstract.md` & `chemfusekit-1.2.0b1/thesis/1-abstract.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/thesis/logo-unibg.png` & `chemfusekit-1.2.0b1/thesis/logo-unibg.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/pyproject.toml` & `chemfusekit-1.2.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "chemfusekit"
-version = "1.2.0"
+version = "1.2.0b1"
 description = "A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis."
 authors = [
     { name = "Federico Aguzzi", email = "62149513+f-aguzzi@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy==1.25.0",
     "scipy>=1.13.0",
```

### Comparing `chemfusekit-1.2.0/readme.md` & `chemfusekit-1.2.0b1/readme.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.2.0/PKG-INFO` & `chemfusekit-1.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chemfusekit
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis.
 Author-email: Federico Aguzzi <62149513+f-aguzzi@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: nbformat>=4.2.0
 Requires-Dist: numpy==1.25.0
```

