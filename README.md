# pre-commit-flutter

[pre-commit](https://pre-commit.com/) hooks for [Flutter](https://flutter.dev/)

---

To use the hooks:
```yaml
# .pre-commit-config.yaml
repos:
  - repo: https://github.com/intellitect/pre-commit-flutter
    rev: 70e63d4b1a3a3262bedbdf53a03dadae302b99a0
    hooks:
      - id: flutter-lint
```

To update to the latest version of the hook:
```shell
pre-commit autoupdate --bleeding-edge --repo https://github.com/intellitect/pre-commit-flutter
```

## Development

To test a hook in this repo:
```shell
pre-commit try-repo --all-files . flutter-lint
```

To test all the hooks, remove the hook ID:
```shell
pre-commit try-repo --all-files .
```
