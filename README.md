# @opinionated-ts/package-template

An experimental TypeScript project template for distributable packages, CLI tools, SDKs, libraries, and other projects that need to be built and packaged for distribution.

It is built on top of [`@opinionated-ts/template`](https://github.com/opinionated-ts/template) and provides the same tooling foundation, with additional structure and defaults for package development and distribution.

> [!WARNING]
>
> This template is currently experimental and under active development.
>
> The underlying TypeScript tooling foundation is established, but the package development and build approach is still being explored and has not yet been fully validated. The packaging structure, build configuration, and related defaults may change as the approach is refined.
>
> It is not ready for general use or production projects.

## When to use this template?

Use this template when developing a TypeScript project that needs to be built and packaged for distribution.

It is intended for projects such as:

- npm packages and libraries
- CLI tools
- SDKs
- reusable TypeScript modules
- other distributable projects that require a build and packaging step

It provides:

- A package-focused starting point built on [`@opinionated-ts/template`](https://github.com/opinionated-ts/template)
- Opinionated defaults for performance, code quality, and developer experience
- A modern Bun-first development environment
- A foundation for building and distributing TypeScript packages
- Consistent tooling across Opinionated TS package projects

The package-specific layer is experimental and may evolve significantly as the approach is validated.

## Getting started

For development and experimentation, clone the repository directly:

```bash
git clone https://github.com/opinionated-ts/package-template.git my-project

cd my-project

rm -rf .git
git init
```

### Install dependencies

```bash
bun install
```

### Install git hooks

```bash
bun hooks:install
```

### Configure package metadata

Update `package.json` for your project and repository:

```json
{
  "name": "your-package-name",
  "repository": {
    "type": "git",
    "url": "git+https://github.com/your-username/your-repo.git"
  }
}
```

At minimum, update:

- `name` — your package name
- `repository.url` — your repository URL

Additional package metadata may be required depending on how the project is distributed.

## What's included

### TypeScript tooling foundation

The package template inherits the tooling, conventions, and project foundation provided by [`@opinionated-ts/template`](https://github.com/opinionated-ts/template).

### Package development foundation

On top of the base template, it adds the structure and defaults currently being explored for building and distributing TypeScript projects.

This includes the foundation required for projects that need compilation, bundling, and package-oriented output.

The package-specific parts are experimental and subject to change as the approach is validated.

## Related projects

- [`@opinionated-ts/template`](https://github.com/opinionated-ts/template) — base TypeScript project template
- [`@opinionated-ts/config`](https://github.com/opinionated-ts/config) — shared tooling configuration used across Opinionated TS projects
