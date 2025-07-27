# MegaLinter Custom Flavor

Demo Custom Flavor

## Embedded linters

  - BASH_SHELLCHECK
  - BASH_SHFMT
  - CSS_STYLELINT
  - HTML_DJLINT
  - JSON_V8R
  - YAML_V8R

## How to generate the flavor

Create a GitHub release on your repo, it will generate and publish your custom flavor using the MegaLinter custom Flavor Builder matching the tag name of your release (example: `9.0.0`)

You can also generate a custom flavor using MegaLinter Custom Flavor by pushing on any branch or manually run the workflow `megalinter-custom-flavor-builder.yml`.

## How to use the custom flavor

Follow [MegaLinter installation guide](https://megalinter.io/latest/install-assisted/), and replace related elements in the workflow.

- GitHub Action: On MegaLinter step in .github/workflows/mega-linter.yml, define `uses: nvuillam/megalinter-custom-flavor-demo@main`
- Docker image: Replace official MegaLinter image by `ghcr.io/nvuillam/megalinter-custom-flavor-demo/megalinter-custom-flavor:latest`