# Usage

My re-usable workflows

## Gradle

```yaml
name: Call Gradle CI

on: [workflow_dispatch, push, pull_request]

jobs:
  call-workflow:
    uses: tomasbjerre/.github/.github/workflows/gradle-ci.yml@master
```

## Draft releases

```yaml
name: Draft release

on: [workflow_dispatch, push]

jobs:
  call-workflow:
    uses: tomasbjerre/.github/.github/workflows/draft-release.yaml@master
```

## Publish release on push

```yaml
name: Publish release on tag push

on:
  workflow_dispatch:
  workflow_call:
  push:
    tags:
      - "*"

jobs:
  call-workflow:
    uses: tomasbjerre/.github/.github/workflows/publish-release-on-tag-push.yaml@master
```
