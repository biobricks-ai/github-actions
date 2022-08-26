# github-actions
A repository for github actions used across biobricks

Use the below for your bricktools check action

```yaml
name: bricktools-check
on: [push]
jobs:
  bricktools-check:
    runs-on: ubuntu-latest
    container: insilica/biobricks:latest
    env:
      GITHUB_PAT: ${{ secrets.GITHUB_TOKEN }}
    steps:
    - name: Check out repository code
      uses: actions/checkout@v3

    - name: bricktools check
      run: bricktools::check(".")
      shell: Rscript {0}
```