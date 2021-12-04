# Usage

My re-usable workflows

## Gradle

```yml
name: Call Gradle CI

on: [push, pull_request]

jobs:
  call-workflow:
    uses: tomasbjerre/.github/.github/workflows/gradle-ci.yml@master
```
