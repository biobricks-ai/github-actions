# github-actions
A repository for github actions used across biobricks

Use the below for your bricktools check action

```yaml
name: "Run bricktools check"
description: "Runs bricktools::check on the current brick"
runs:
  using: 'docker'
  image: 'docker://insilica/biobricks:latest'
  entrypoint: '/github-action-bricktools-check.sh'
```
