# Smithy for VS Code

This package is a Visual Studio Code extension to recognize and highlight the
Smithy interface definition language (IDL). It can also be used as a TextMate
bundle in TextMate and [IntelliJ using a third-party plugin](https://www.jetbrains.com/help/idea/importing-textmate-bundles.html).

## Features

This extension provides basic syntax highlighting of ".smithy" files.

Additionally, it provides [Snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets).

## Installation

### VS Code

This extension and the Smithy Language Server are not yet published. To use this extension, publish the Language Server locally before manually installing the Extension with the following steps:
* Clone the Language Server locally: `git clone https://github.com/awslabs/smithy-language-server.git && cd smithy-language-server`
* Build and publish it locally: `./gradlew build publishToMavenLocal`
* Clone the Extension: `git clone https://github.com/awslabs/smithy-vscode.git && cd smithy-vscode`
* Run npm commands to install:
`npm install && npm run install-plugin`

### IntelliJ

You can use this extension in IntelliJ by installing the
"TextMate bundle support" plugin and registering this repository as a bundle.
See the [IntelliJ documentation](https://www.jetbrains.com/help/idea/textmate.html)
for more details.

## Release Notes

### 0.3.0 - 2020-09-19

- Updated to work with Smithy 1.0 syntax.

### 0.2.0 - 2019-06-26

- Add support for use statements.
- Add support for documentation comments.

### 0.1.0

Initial release for Smithy IDL syntax highlighting.
