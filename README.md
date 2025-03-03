# tool-language-support README

This package provides TOOL language support for VSCode.

## To install this extension in vscode:
```
code --install-extension <replace-with-your-local-path-to-this-folder>\tool-language-support-0.0.2.vsix
```

## To improve and update the extension
If you don't already have node and npm installed, you will first need to [install them](https://medium.com/@imvinojanv/how-to-install-node-and-npm-on-your-local-machine-45fc0f2438a2).

To make changes, you will need VSCE installed to create vsix files. In terminal, run:

`npm install –g vsce`

At this point you should be set up to work on the extension.

1. make whatever improvements.  The language formatting is defined in `/syntaxes/tool.tmLanguage.json`. Code snippets for various TOOL language commands are defined in `/snippets/snippet.json`
2. After making your changes, run the command: `vsce package`  (you can ignore warnings about repository and license)
3. Commit your changes to this repository
4. re-run the command `code --install-extension <replace-with-your-local-path-to-this-folder>\tool-language-support-0.0.2.vsix`
5. notify your colleauges that you've made an improvement!
