# publish tutorial

## Copy
[/.vscode/settings.json](https://github.com/ngnam/supper-extension-software-develop/blob/master/settings.json)
```
{
    "workbench.iconTheme": "material-icon-theme",
    "peacock.favoriteColors": [
        {
            "name": "Angular Red",
            "value": "#b52e31"
        },
        {
            "name": "JavaScript Yellow",
            "value": "#f9e64f"
        },
        {
            "name": "Node JS",
            "value": "#1857a4"
        },
        {
            "name": "Dot net core",
            "value": "#215732"
        },
        {
            "name": "React Blue",
            "value": "#00b3e6"
        },
        {
            "name": "Java",
            "value": "#832561"
        },
        {
            "name": "Vue Green",
            "value": "#42b883"
        }
    ],
    "editor.formatOnPaste": true,
    "editor.fontFamily": "Consolas, 'Fira Code', monospace",
    "workbench.editor.highlightModifiedTabs": true,
    "files.autoSave": "afterDelay",
    "files.autoSaveDelay": 60000,
    "explorer.sortOrder": "type",
    "editor.cursorStyle": "line-thin",
    "editor.cursorBlinking": "smooth",
    "terminal.integrated.cursorBlinking": true,
    "files.trimFinalNewlines": true,
    "editor.acceptSuggestionOnEnter": "smart",
    "editor.renderWhitespace": "all",
    "prettier.tabWidth": 4,
    "editor.codeActionsOnSave": {
        "source.organizeImports": false
    },
    "editor.codeLens": false,
    "editor.cursorSmoothCaretAnimation": true,
    "editor.fontLigatures": true,
    "editor.formatOnType": false,
    "editor.letterSpacing": 1,
    "editor.lineHeight": 25,
    "editor.minimap.enabled": false,
    "editor.tabCompletion": "on",
    "editor.tabSize": 4,
    "editor.detectIndentation": true,
    "editor.wordWrap": "off",
    "sonarlint.ls.javaHome": "C:\\Program Files\\Java\\jdk-12.0.1",
    "[typescript]": {
        "editor.defaultFormatter": "esbenp.prettier-vscode",
        "editor.codeActionsOnSave": {
            "source.organizeImports": false
        },
        "editor.codeLens": false,
        "editor.cursorSmoothCaretAnimation": true,
        "editor.fontLigatures": true,
        "editor.formatOnType": false,
        "editor.letterSpacing": 1,
        "editor.lineHeight": 25,
        "editor.minimap.enabled": false,
        "editor.tabCompletion": "on",
        "editor.tabSize": 4,
        "editor.detectIndentation": true,
        "editor.wordWrap": "off",
    },
    "git.ignoreLimitWarning": true,
    "files.exclude": {
        "**/.git": true,
        "**/.DS_Store": true,
        "**/*.js": {
            "when": "$(basename).ts"
        },
        "**/*.js.map": {
            "when": "$(basename)"
        },
        "**/.classpath": true,
        "**/.project": true,
        "**/.settings": true,
        "**/.factorypath": true
    },
    "files.hotExit": "onExit",
    "files.defaultLanguage": "typescript",
    "files.trimTrailingWhitespace": true,
    "prettier.singleQuote": true,
    "workbench.colorCustomizations": {
        "activityBar.background": "#fbed80",
        "activityBar.foreground": "#15202b",
        "activityBar.inactiveForeground": "#15202b99",
        "activityBarBadge.background": "#06b9a5",
        "activityBarBadge.foreground": "#15202b",
        "titleBar.activeBackground": "#f9e64f",
        "titleBar.inactiveBackground": "#f9e64f99",
        "titleBar.activeForeground": "#15202b",
        "titleBar.inactiveForeground": "#15202b99",
        "statusBar.background": "#f9e64f",
        "statusBarItem.hoverBackground": "#f7df1e",
        "statusBar.foreground": "#15202b"
    },
}
```

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