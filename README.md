# Wotan pre-commit

This repository contains a [pre-commit hook](https://pre-commit.com/#pre-commit-configyaml---hooks) that runs [Wotan](https://github.com/fimbullinter/wotan) on staged TypeScript and Vue files.

## Usage

Ensure that [pre-commit is installed](https://pre-commit.com/#install), then add this repo to your project's `.pre-commit-config.yaml` file:

```yaml
repos:
  - repo: https://github.com/johnfraney/wotan-pre-commit
    rev: v0.1.0
    hooks:
      - id: wotan
        language: node
        types: [vue, ts]
```
