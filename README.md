# check-if-merged GH Action

## Uses:

create at your repo root path: .github/workflows/check_if_merged.yml with:

```
name: Check if branch is merged to staging
on:
  push:
    branches-ignore:
      - 'master'
      - 'staging'
jobs:
  check-if-merged:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v1
    - uses: CareMessagePlatform/check-if-merged@v1
```
