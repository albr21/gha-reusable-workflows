# gha-reusable-workflows

GitHub Actions workflows for CI/CD across repositories.

## Usage

```yaml
name: <workflow-name>

on:
  workflow_dispatch:

jobs:
  python-ci:
    uses: albr21/gha-reusable-workflows/.github/workflows/reusable-build-and-push-docker-image-on-ghcr.yml
    with:
      name: <name>
      tag: <tag>
      dockerfile: <dockerfile>
      context: <context>
    secrets: inherit
```

## Available Workflows

- [🧩 Reusable Build and Push Docker Image on GHCR](./workflows/reusable-build-and-push-docker-image-on-ghcr.yml)

## Contributing

Check out the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
