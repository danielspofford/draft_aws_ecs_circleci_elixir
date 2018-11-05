# Draft AWS ECS CircleCI Elixir

A [Draft](https://github.com/danielspofford/draft) template for a CircleCI
config for an Elixir project that will be deployed to AWS ECS.

## Related

- [draft_aws_ecs](https://github.com/danielspofford/draft_aws_ecs)

## Usage

### Template execution

Install the `draft` mix archive if you haven't already:

```
mix archive.install github danielspofford/draft
```

Execute this template:

```
mix draft.github danielspofford/draft_aws_ecs_circleci_elixir \
  --app-name=your_app_name \
  --production-image=your_production_image \
  --cluster=your_cluster_name \
  --service=your_service_name \
  --task=your_task_definition_name \
  --slack_build_channel=your_slack_channel \
  --slack_hook=your_slack_hook
```

`--app-name` may only contain letters, numbers, and underscores.
`--production-image` should not include a `:tag` suffix.
