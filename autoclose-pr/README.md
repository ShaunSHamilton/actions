# Auto-close PR

## Required Inputs and Outputs

## Optional Inputs and Outputs

## Secrets Used

## Environment Variables

## Example

```yml
name: GitHub - Autoclose Invalid PRs
on:
  pull_request_target:
    branches:
      - "main"
    paths:
      - ".gitignore"

jobs:
  autoclose:
    name: Auto-Close
    steps:
      - name: Run Action
        uses: freeCodeCamp/actions/autoclose-pr@main
```
