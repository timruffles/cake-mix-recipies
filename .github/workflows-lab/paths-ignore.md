on:
  push:
    paths-ignore:
    - "docs/**"

jobs:
  pushOnMasterLab:
    runs-on: ubuntu-16.04
    name: "lab paths ignore"
    steps:
      - uses: actions/npm@master
        name: docker action
        with:
          args: --version
