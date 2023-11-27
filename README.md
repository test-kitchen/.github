# Reusable Workflows

## Lint and Unit Test

- `.github/workflows/lint-unit.yml`

## Usage

Include the following in your workflow:

```yaml
jobs:
  lint-unit:
    uses: test-kitchen/.github/.github/workflows/lint-unit.yml@main
    with:
    bundle_with: "chefstyle"
    bundle_without: "development"
```

The options above are the default values, so you can omit them if you want.
