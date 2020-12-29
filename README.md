# pipelines
Buildkite Pipelines for Matrix.org Projects.

## Testing a pipeline locally

If you would like to test a change to a pipeline before merging to this repo,
you can opt to run the pipeline on your local machine.

1. Install [buildkite-agent](https://github.com/buildkite/agent) and [buildkite-cli](https://github.com/buildkite/cli).
2. Login to buildkite with `bk configure buildkite`.
3. Create your own Buildkite organisation. This is to ensure separation of
   production agents from developer computers. Do so from the drop-down on
   https://buildkite.com once signed in.
4. Configure your buildkite agent token. This should be the agent token of
   the org you just created. You can find your organisation's agent token under
   https://buildkite.com/organizations/YOUR_ORG_NAME/agents.
5. Change to the directory of the project you'd like to test (e.g. `cd
   /path/to/synapse`) and do `bk run /path/to/pipelines-repo/PROJECT_NAME/pipeline.yml`.
