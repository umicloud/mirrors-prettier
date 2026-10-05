prettier mirror
===============

Mirror of prettier package for pre-commit.

For pre-commit: see https://github.com/pre-commit/pre-commit

For prettier: see https://github.com/prettier/prettier

### Using prettier with pre-commit

Add this to your `.pre-commit-config.yaml`:

```yaml
- repo: https://github.com/umicloud/mirrors-prettier
  rev: "" # Use the sha / tag you want to point at
  hooks:
    - id: prettier
```

_note_: only prettier versions >= 2.1.0 are supported

By default, all files are passed to `prettier`, if you want to limit the
file list, adjust `types` / `types_or` / `files`:

```yaml
- id: prettier
  types_or: [css, javascript]
```
