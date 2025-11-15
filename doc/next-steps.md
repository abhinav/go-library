# Next steps (delete me)

Now that the project has been scaffolded,
take the following steps to start working on it:

1. **Update the repository and import path**

    Update all references to the placeholder
    repository path (abhinav/go-library)
    and import path (go.abhg.dev/library)
    to the actual import path of your project.

    ```bash
    REPOSITORY_PATH="..."  # e.g. "abhinav/foo-go"
    IMPORT_PATH="..."      # e.g. "go.abhg.dev/foo"
    git ls-files |
      xargs perl -p -i \
        -e "s{go.abhg.dev/library}{$IMPORT_PATH}g; \
            s{abhinav/go-library}{$REPOSITORY_PATH}g"
    ```

2. **Update the package name**

    doc.go is the only file where the package name is defined.
    Update it.

3. **Delete this file**

    ```bash
    git rm doc/next-steps.md
    ```

4. **Write documentation**

    When you're ready, update doc/README.md and accompanying files.
