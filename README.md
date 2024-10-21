# setup-vtk

[![Continuous Integration](https://github.com/Quesys-tech/setup-vtk/actions/workflows/ci.yml/badge.svg)](https://github.com/Quesys-tech/setup-vtk/actions/workflows/ci.yml)
[![Lint Codebase](https://github.com/Quesys-tech/setup-vtk/actions/workflows/linter.yml/badge.svg)](https://github.com/Quesys-tech/setup-vtk/actions/workflows/linter.yml)

This action installs [Visualization Toolkit (VTK)](https://vtk.org/) onto the
runner.

## Usage

```yaml
name: Check Transpiled JavaScript
on:
  pull_request:

jobs:
  runs-on: ubuntu-latest # currently only supports ubuntu
  steps:
    # checkout your repository
    - uses: Quesys-tech/setup-vtk@v1
      with:
        vtk-version: '9.3.1' # `latest` tag is also available
    # build your project with VTK
```

## Roadmap

1. Develop a version that supports latest version of VTK on Ubuntu
2. Develop a version that supports latest version of VTK on Windows
3. Develop a version that supports latest version of VTK on MacOS
