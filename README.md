<div align="center">

[![copier](https://img.shields.io/badge/copier-template-orange)](https://copier.readthedocs.io/)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![mise](https://mise-versions.jdx.dev/badge.svg)](https://mise.jdx.dev)
[![bun](https://img.shields.io/badge/bun-toolkit-yellow)](https://bun.sh)


# bun-ts-vite copier template
</div>

This Copier template bootstraps repository for projects that leverage `bun`, `TypeScript`, and `Vite`. It is intentionally small: the goal is to give every new repository a consistent starting point for line endings, ignore rules, and local quality checks.

## What It Adds

The generated repository includes:

- `.gitignore` with GitHub's `macOS` and `mise` templates
- `.gitattributes` rendered from `.gitattributes.jinja` to normalize text files and mark common binaries
- `.pre-commit-config.yaml` with basic repository safety and shell linting hooks
- `mise.toml` to pin the tools used to maintain the template and generated repositories

## Included Tooling

Tool versions are managed with `mise`.

- `git-cliff` for changelog generation
- `pre-commit` for local hook execution
- `bun` for running scripts and managing dependencies of the web projects

## Usage

Create a new repository from this template with Copier:

```bash
copier copy gh:copier-templates/bun-ts-vite path/to/new-repo
```

After generation, install the managed tools and run the configured checks:

```bash
mise install
mise run check
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Credits
When using this template, refer to [copier-templates/bun-ts-vite](https://github.com/copier-templates/bun-ts-vite).
