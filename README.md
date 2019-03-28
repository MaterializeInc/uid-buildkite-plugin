# UID Buildkite Plugin

A [Buildkite plugin] that exposes the agent's UID and GID as environment
variables.

## Details

The user ID is exported as the `BUILDKITE_AGENT_UID` environment variable.
The group ID is exported as the `BUILDKITE_AGENT_GID` environment variable.

## Example

```yml
steps:
  - command: 'echo "My UID is: $$BUILDKITE_AGENT_UID"'
    plugins:
      - timelydata/uid#1.0.0: ~
```

[Buildkite plugin]: https://buildkite.com/docs/agent/v3/plugins
