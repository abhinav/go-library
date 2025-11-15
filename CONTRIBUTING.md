# Contributing

## Setup

Tooling for this project is managed with
[mise](https://mise.jdx.dev/).
It's easiest to set up mise to get the right versions of tools.

Short of that, look at mise.toml and mise.lock
and install the right versions of tools manually.

## Changelog

All significant user-facing changes should be added to the changelog.
We use [changie](https://changie.dev/) to manage the changelog.

Add new unreleased entries with `changie new`.

## Releasing a new version (maintainers only)

1. Batch together unreleased changes into a new version.

    ```bash
    # For minor releases:
    changie batch minor

    # If only fixing bugs:
    changie batch patch
    ```

2. Merge the new changes with the root CHANGELOG.md.

    ```bash
    changie merge
    ```

3. Commit these changes to a new branch.

    ```bash
    git checkout -b release-$(changie latest)
    git add .changes CHANGELOG.md
    git commit -m "Release $(changie latest)"
    ```

4. Submit a pull request and wait for it to be merged, and pull it.

    ```bash
    git checkout main
    git pull
    ```

5. Tag the new release

    ```bash
    gh release create $(changie latest) -F .changes/$(changie latest).md
    ```
