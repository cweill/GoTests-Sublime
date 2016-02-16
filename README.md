# GoTests-Sublime [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/cweill/GoTests-Sublime/blob/master/LICENSE)

`GoTests-Sublime` is an IDE plugin for Sublime Text 3 for automatically generating [table driven tests](https://github.com/golang/go/wiki/TableDrivenTests). It uses [`gotests`](https://github.com/cweill/gotests) to generate missing tests based on its target source files' function and method signatures. Any new dependencies in the test files are automatically imported.

## Demo

![demo](/gotests.gif)

## Installation

__Prequisite:__ Use [`go get`](https://golang.org/cmd/go/#hdr-Download_and_install_packages_and_dependencies) to install and update the `gotests` tool:
```sh
$ go get -u github.com/cweill/gotests/...
```
Next, install the `GoTests-Sublime` plugin:

With [Package Control](http://wbond.net/sublime_packages/package_control):

1. Run “Package Control: Install Package” command, find and install `GoTests` plugin.
2. Restart Sublime Text (if required)

Manually:

1. Clone this repo into your [Packages folder](https://www.sublimetext.com/docs/3/packages.html)
2. Restart Sublime Text (if required)

Finally, open `Preferences > Package Settings > GoTests > Settings - User`. In the newly created file, add the absolute path to the `gotests` binary (`$ which gotests`):

```js
// GoTests.sublime-settings
{
    // Add path to gotests here.
	"gotests_cmd": "/absolute/path/to/gotests",
}
```

## Usage

Select some functions, right-click, and select `Generate Go tests`. This appends missing tests to an existing test file, or creates a new test file with them.

## License

`GoTests-Sublime` is released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
