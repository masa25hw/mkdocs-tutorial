# Continouous Integration

## GitHub Pages

GitHub ActionsでYAMLを作成。

```YAML
name: CI

on:
  push:
    branches: main

jobs:
  Upload-gh-pages
  runs-on: [ self-hosted , Linux]
    - name: Checkout
      uses: actions/checkout@v2

    - name: Update GitHub Pages
      run: |
        mkdocs build --clean
        mkdocs gh-deploy
```
