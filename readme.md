# publish tutorial
* https://code.visualstudio.com/api/working-with-extensions/publishing-extension#publishing-extensions

# Installation
Make sure you have Node.js installed. Then run:

`npm install -g vsce`

# Usage
You can use vsce to easily package and publish your extensions:
```
    $ cd myExtension
    $ vsce package
    # myExtension.vsix generated
    $ vsce publish
    # <publisherID>.myExtension published to VS Code MarketPlace

    vsce create-publisher (publisher name)
    vsce login (publisher name)
    vsce publish -p <token>

```
* update extension `vsce publish minor`

# auto-changelog
Command line tool for generating a changelog from git tags and commit history
Latest npm version Build Status Test Coverage

## Installation

* Run `npm install -g auto-changelog`

## Usage

*Run `auto-changelog -p -v 1.0.0 -o CHANGELOG.md`

## isue when published
* https://github.com/Microsoft/vscode-vsce/issues/11