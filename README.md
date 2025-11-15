- [Next steps](#next-steps-delete-me)

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


# Go library template

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)


## Introduction

[![Go Reference](https://pkg.go.dev/badge/go.abhg.dev/library.svg)](https://pkg.go.dev/go.abhg.dev/library)
[![CI](https://github.com/abhinav/go-library/actions/workflows/ci.yml/badge.svg)](https://github.com/abhinav/go-library/actions/workflows/ci.yml)

<!--
Uncomment when repository is public
[![codecov](https://codecov.io/gh/abhinav/go-library/branch/main/graph/badge.svg?token=W98KYF8SPE)](https://codecov.io/gh/abhinav/go-library)
-->

library is a Go library that does things.

## Installation

Install the latest release with Go modules:

```bash
go get go.abhg.dev/library@latest
```

## Usage

To use library, import it:

```go
import "go.abhg.dev/library"
```

Then do stuff with it.

## License

This software is made available under the BSD-3 license.
See LICENSE for the full license text.
