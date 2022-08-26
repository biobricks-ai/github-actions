# github-actions
Biobricks github actions

## Run bricktools::check on this brick

```yaml
name: "Run bricktools check"
description: "Runs bricktools::check on the current brick"
runs:
  using: 'docker'
  image: 'docker://insilica/biobricks:latest'
  entrypoint: '/github-action-bricktools-check.sh'
```
