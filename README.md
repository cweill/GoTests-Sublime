# GoTests-Sublime [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/cweill/GoTests-Sublime/blob/master/LICENSE)

`GoTests-Sublime` makes writing better Go tests easy. It is an IDE plugin for Sublime Text 3 that uses [`gotests`](https://github.com/cweill/gotests) to generate [table driven tests](https://github.com/golang/go/wiki/TableDrivenTests) from selected function and method signatures. Any new dependencies in the test files are automatically imported.

## Demo

![demo](/gotests.gif)

## Installation

__Prequisite:__ Use [`go get`](https://golang.org/cmd/go/#hdr-Download_and_install_packages_and_dependencies) to install and update the `gotests` tool:
```sh
$ go get -u github.com/cweill/gotests/...
```
Next, install the `GoTests-Sublime` plugin:

With [Package Control](http://wbond.net/sublime_packages/package_control):

1. Run the `Package Control: Install Package` command
1. Find and install `GoTests`
1. Restart Sublime Text (if required)

Manually:

1. Clone this repo into your [Packages folder](http://docs.sublimetext.info/en/sublime-text-3/basic_concepts.html#the-data-directory)
1. Restart Sublime Text (if required)

Finally, open `Preferences > Package Settings > GoTests > Settings - User`. In the newly created file, set your `$GOPATH`:

```js
// GoTests.sublime-settings
{
	// Add your GOPATH here.
	"GOPATH": "/absolute/go/path/",
}
```

## Usage

Select some functions, right-click, and select `Generate Go tests`. This appends missing tests to an existing test file, or creates a new test file with them.

## License

`GoTests-Sublime` is released under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0).
