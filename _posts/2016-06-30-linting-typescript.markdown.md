---
layout: post
title:  "Linting TypeScript - Getting Started with TSLint"
date:   2016-06-30 11:00:00
categories: typescript, visual studio code
author: Carlos R. Mendoza
<!-- permalink: -->
---

[TSLint](https://palantir.github.io/tslint/) is a popular TypeScript linting library. To integrate TSLint with a TypeScript project, follow the steps below.  

*Note: the commands below were tested to work with TSLint -v 3.12.1.*

### Installing TSLint
To get started, install the TSLint Command Line Interface (CLI).

`npm install tslint -g`

TypeScript is a peer dependency of TSLint, so make sure that you have it installed. If not, run the command below before installing TSLint.

`npm install typescript -g`

### Integrating TSLint in Your Project
Navigate to the root of your project, and run the command below.

`tslint --init` or `tslint -i`

This will generate a `tslint.json` config file in the root of your project. This files specifies the rules that are enabled and their options. To see which rules are available, visit [http://palantir.github.io/tslint/rules](http://palantir.github.io/tslint/rules).

### Running TSLint
To lint a file in your project, run the command below.

`tslint path/toFile.ts`

### Using TSLint with Visual Studio Code (VS Code)
If you are using VS Code, you can install the [TSLint extension](https://marketplace.visualstudio.com/items?itemName=eg2.tslint) by running the commands below inside of VS Code.

Launch VS Code Quick Open - `⌘+P`

Run - `ext install tslint`

If TSLint is correctly integrated with a project, VS Code should now lint project files as you type.



