# .github

### Currently used actions

* __version-check__ - action responsible for checking the version when modifying the code.
* __tests__ - action responsible for running the tests in python or typescript.
* __release action__ - action responsible for code distribution.

### Reusable workflows

* __semgrep-authz__ (`.github/workflows/semgrep-authz.yaml`) - scans for authorization
  paths that answer "allowed" when identity is unknown or the check itself failed.
  Report-only by default; see the header of that file before making it blocking.

For more information check the documentation.

Hero Labs

### Inputs 

| Name                    | Required | Description                             |
|-------------------------|----------|-----------------------------------------|
| WORKFLOW_SKIP_CHECKOUT  | no       | Skip checkout                           |
| WORKFLOW_USE_ARTIFACTS  | no       | Download artifacts from *artifacs* path |
| HL_GITHUB_TOKEN         | no       | If defined that GitHub Action will try to sync submodules |