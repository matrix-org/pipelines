# pipelines
Buildkite Pipelines for Matrix.org Projects.

## Testing a pipeline locally

See the intructions at
https://gitlab.matrix.org/new-vector/internal/-/wikis/BuildKite#testing-a-pipeline-locally.

This is an internal page. If you are not allowed to view this page, know that
the instructions effectively boil down to:

1. Install [buildkite-agent](https://github.com/buildkite/agent) and [buildkite-cli](https://github.com/buildkite/cli).
2. Change to the codebase directory of the project you'd like to test.
3. Run `bk local run /path/to/project/pipeline.yml`.

Note that `--debug` can be added to the above command to produce
some more helpful logs.
