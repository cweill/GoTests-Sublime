# GoTests-Sublime [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/cweill/GoTests-Sublime/blob/master/LICENSE)

`GoTests-Sublime` is an IDE plugin for Sublime Text 3 for automatically generating [table driven tests](https://github.com/golang/go/wiki/TableDrivenTests). It uses [`gotests`](https://github.com/cweill/gotests) to generate missing tests based on its target source files' function and method signatures. Any new dependencies in the test files are automatically imported.

## Demo

![demo](/gotests.gif)

## Installation

First use [`go get`](https://golang.org/cmd/go/#hdr-Download_and_install_packages_and_dependencies) to install and update the `gotests` tool:
```sh
$ go get -u github.com/cweill/gotests/...
```

## License

`GoTests-Sublime` is released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
