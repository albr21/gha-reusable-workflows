# gha-reusable-workflows

GitHub Actions workflows for CI/CD across repositories.

## Usage

```yaml
name: <workflow-name>

on:
  workflow_dispatch:

jobs:
  <job-name>:
    uses: albr21/gha-reusable-workflows/.github/workflows/<workflow-name>@main
    with:
      <inputs>
    secrets: inherit
```

## Available Workflows

- [🧩 Build and Push Docker Image on GHCR](./workflows/reusable-build-and-push-docker-image-on-ghcr.yml)
- [🧩 GHA Quality](./workflows/reusable-gha-quality.yml)
- [🧩 Perform GitHub Release](./workflows/reusable-perform-github-release.yml)
- [🧩 Python Quality](./workflows/reusable-python-quality.yml)

## Contributing

Check out the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute to this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
