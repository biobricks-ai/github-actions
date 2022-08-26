# github-actions
Biobricks github actions

## Run bricktools::check on this brick
Add the below to .github/workflows/bricktools-check.yaml
```yaml
name: bricktools-check
on: [push]
jobs:
  bricktools-check:
    runs-on: ubuntu-latest
    steps:
      - name: bricktools check
        uses: biobricks-ai/github-actions/bricktools-check@main
```
