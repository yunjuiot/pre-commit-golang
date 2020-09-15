# pre-commit-golang

Golang pre-commit hooks for https://pre-commit.com

## HOWTO

1. Install pre-commit

```
brew install pre-commit
# Or pip install pre-commit
```

2. Add a file named `.pre-commit-config.yaml` into the root directory of your repository.

```yaml
repos:
  - repo: https://github.com/yunjuiot/pre-commit-golang
    rev: v1.0.0
    hooks:
      - id: go-imports
      - id: go-vet
      - id: go-lint
      - id: go-unit-tests
      - id: go-mod-tidy
      - id: golangci-lint # requires github.com/golangci/golangci-lint
```

2. Install pre-commit into your git repo

```
pre-commit install
```

## Credits

This repo is inspired by [`Bahjat/pre-commit-golang`](https://github.com/Bahjat/pre-commit-golang)
