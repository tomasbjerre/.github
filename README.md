# Usage

My re-usable workflows

## Gradle

```yml
name: Call Gradle CI

on: [workflow_dispatch, push, pull_request]

jobs:
  call-workflow:
    uses: tomasbjerre/.github/.github/workflows/gradle-ci.yml@master
```
