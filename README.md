# ast-grep-pre-commit-mirror

[ast-grep](https://ast-grep.github.io/) pre-commit hook distributed via PyPI for seamless integration with Python projects.

## Usage

Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/PFCCLab/ast-grep-pre-commit-mirror
  rev: v0.39.1
  hooks:
    - id: ast-grep
```

### Auto-fix code issues

```yaml
- id: ast-grep
  args: ["--update-all"]
```

### Custom configuration

```yaml
- id: ast-grep
  args: ["--config", "ast-grep/sgconfig.yml"]
```

## Writing Rules

ast-grep uses AST pattern matching to search and rewrite code:

- [Documentation](https://ast-grep.github.io/guide/introduction.html) - Learn the fundamentals
- [Playground](https://ast-grep.github.io/playground.html) - Test patterns interactively
- [Rule Examples](https://ast-grep.github.io/catalog/) - Browse community rules
