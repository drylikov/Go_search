


































































































































# Go_search.

 [Godoc.org](http://godoc.org) via the command-line.

 ![godoc command-line search]

## Installation

```
$ go get github.com/drylikov/Go_search
```

## Usage

- Add an alias: `alias gos=Go_search`
- Help text:
    ```sh
    $ Go_search --help
    Usage:
        Go_search <query>... [--top] [--count n] [--open]
        Go_search -h | --help
        Go_search --version

      Options:
        -n, --count n    number of results [default: 5]
        -t, --top        top-level packages only
        -o, --open       open godoc.org search results in default browser
        -h, --help       output help information
        -v, --version    output version
    ```
- Examples:
    ```sh
    $ Go_search UUID

        github.com/pborman/uuid
        godoc.org/pkg/github.com/pborman/uuid
        The uuid package generates and inspects UUIDs.

        github.com/satori/go.uuid
        godoc.org/pkg/github.com/satori/go.uuid
        Package uuid provides implementation of Universally Unique
        Identifier (UUID).

        github.com/nu7hatch/gouuid
        godoc.org/pkg/github.com/nu7hatch/gouuid
        This package provides immutable UUID structs and the
        functions NewV3, NewV4, NewV5 and Parse() for generating
        versions 3, 4 and 5 UUIDs as specified in RFC 4122.

        github.com/twinj/uuid
        godoc.org/pkg/github.com/twinj/uuid
        This package provides RFC4122 and DCE 1.1 UUIDs.

        github.com/docker/distribution/uuid
        godoc.org/pkg/github.com/docker/distribution/uuid
        Package uuid provides simple UUID generation.
    ```
    ```sh
    $ Go_search UUID --open
    # opens godoc.org search results in default browser
    ```
