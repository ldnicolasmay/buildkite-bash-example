# Buildkite Bash Example

## Trigger Build

Click the "New Build" button in the web UI for the `buildkite-bash-example-pipeline` pipeline.

Or you can use curl:

```shell
curl -H "Authorization: Bearer $TOKEN" \
  "https://api.buildkite.com/v2/organizations/test-org-ldnicolasmay/pipelines/buildkite-bash-example-pipeline/builds" \
  -X "POST" \
  -F "commit=HEAD" \
  -F "branch=master" \
  -F "message=First build :rocket:"
```
