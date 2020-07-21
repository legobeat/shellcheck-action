# Shellcheck Action

## Usage

Add the following to your GIthub Actions workflows:

```yaml
name: shellcheck

on: [push]

jobs:
  lint:
    name: lint
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@master
      - name: ShellCheck Action
        uses: fearphage/shellcheck-action@master
        env:
          GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
```

## Acknowledgements:

* Shellcheck - https://github.com/koalaman/shellcheck
