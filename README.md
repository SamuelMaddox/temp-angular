# Probe Management <!-- omit in toc -->

- [Getting Started](#getting-started)
  - [Step 0 - Recommended IDE Setup](#step-0---recommended-ide-setup)
  - [Step 1 - Local Development Prerequisite](#step-1---local-development-prerequisite)
  - [Step 2 - Clone Repository](#step-2---clone-repository)
  - [Step 3 - Install Dependencies](#step-3---install-dependencies)
  - [Step 4 - Run VS Code Debugger](#step-4---run-vs-code-debugger)
- [Scripts](#scripts)
- [Pre-commit Hooks](#pre-commit-hooks)
- [Testing](#testing)
  - [Vue Testing Library](#vue-testing-library)
  - [Run Tests](#run-tests)
  - [View Test Coverage](#view-test-coverage)
- [CI/CD Pipeline Notes](#cicd-pipeline-notes)
- [File Structure](#file-structure)
  - [Sample File Structure](#sample-file-structure)
  - [File Structure Conventions](#file-structure-conventions)
- [ESLint and Prettier](#eslint-and-prettier)
  - [What is ESLint](#what-is-eslint)
  - [What Is Prettier](#what-is-prettier)
  - [Linting \& Prettier Disable Conventions](#linting--prettier-disable-conventions)
  - [Eslint Ignore Node](#eslint-ignore-node)
  - [Prettier Ignore Node](#prettier-ignore-node)
  - [Ignore root files or directories](#ignore-root-files-or-directories)
- [Type Support for `.vue` Imports in TS](#type-support-for-vue-imports-in-ts)
- [Customize configuration](#customize-configuration)
- [Project Setup](#project-setup)
  - [Compile and Hot-Reload for Development](#compile-and-hot-reload-for-development)
  - [Type-Check, Compile and Minify for Production](#type-check-compile-and-minify-for-production)
  - [Lint with ESLint](#lint-with-eslint)

This template should help get you started developing with Vue 3 in Vite.

## Getting Started

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### Step 0 - Recommended IDE Setup

- Install [VSCode](https://code.visualstudio.com/)
- Add these VSCode Extensions:

  - [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) - Syntax highlighting for Vue
  - [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) - Provides immediate linting when writing code.
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - Used to automatically format code files to a consistent style.
  - [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph) - View a Git Graph of your repository, and easily perform Git actions from the graph.
  - [Markdown All In One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one) - Useful for managing table of contents in markdown files. Also provides other useful features.
  - [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) - linting for markdown files to encourage standards and consistency for Markdown files.
  - [open in browser](https://marketplace.visualstudio.com/items?itemName=techer.open-in-browser) - Useful to quickly open [test coverage](#view-test-coverage) files in browser.

- Disable the VSCode Extension [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur) if you have it. This is for Vue v2 and we're using Vue v3.

### Step 1 - Local Development Prerequisite

- Install git using [these instructions](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
- Install Node 18+
  - **Mac/Linux**: [Node Version Manager](https://github.com/nvm-sh/nvm)
  - **Windows 10/11**: [Node Windows Installer](https://nodejs.org/en/)

### Step 2 - Clone Repository

### Step 3 - Install Dependencies

### Step 4 - Run VS Code Debugger

## Scripts

## Pre-commit Hooks

## Testing

### Vue Testing Library

### Run Tests

### View Test Coverage

## CI/CD Pipeline Notes

## File Structure

### Sample File Structure

```txt
📁 src
================================================================================
| 📁 API
| | 📁 FirstAPI
| | | 📄 index.ts
| | | 📄 Types.ts
================================================================================
| 📁 Components
| | 📁 Core
| | | 📁 FirstComponent
| | | | 📁 Assets
| | | | | 📄 icon.svg
| | | | 📁 Utils
| | | | | 📄 FirstUtil.ts
| | | 📄 index.vue
| | | 📄 index.test.ts
| | | 📄 Types.ts
================================================================================
| 📁 Config
| | 📁 FirstCategoryConfig
| | | 📄 index.ts
| | | 📄 Types.ts
================================================================================
| 📁 Font
| | 📁 FontName
| | | 📄 FontNameRegular.ttf
| | | 📄 FontNameItalic.ttf
| | | 📄 FontNameBold.ttf
| | | 📄 FontNameBoldItalic.ttf
| | 📄 FontName.css
================================================================================
| 📁 Layouts
| | 📁 MainLayout
| | | 📄 index.vue
| | | 📄 index.test.ts
| | | 📄 Types.ts
================================================================================
| 📁 Modules
| | 📁 Layout
| | | 📁 MainHeader
| | | | 📁 Assets
| | | | | 📄 pic.png
| | | | 📁 Components
| | | | | ...
| | | | 📁 Utils
| | | | | 📄 FirstUtil.ts
| | | | 📄 index.vue
| | | | 📄 index.test.ts
| | | | 📄 Types.ts
================================================================================
| 📁 Providers
| | 📁 FirstProvider
| | | 📄 index.ts
| | | 📄 Types.ts
================================================================================
| 📁 Router
| | 📄 index.ts
================================================================================
| 📁 SharedAssets
| | 📁 GroupOne
| | | 📄 pic.png
================================================================================
| 📁 Types
| | 📁 GroupOne
| | | 📁 Classes
| | | | 📄 FirstClassType.ts
| | | 📁 Enums
| | | | 📄 FirstEnumType.ts
| | | 📁 Interfaces
| | | | 📄 FirstInterfaceType.ts
================================================================================
| 📁 Utils
| | 📁 Core
| | | 📁 Constants
| | | | 📄 TimeConstants.ts
| | | 📁 FirstUtil.ts
| | | | 📄 FirstUtil.ts
| | | | 📄 index.ts
| | | | 📄 Types.ts
| | 📁 TestUtils
| | | 📄 RenderPage.ts
================================================================================
| 📁 Views
| | 📁 Core
| | | 📁 HomePage
| | | | 📁 Assets
| | | | | 📄 pic.png
| | | | 📁 Hooks
| | | | | 📄 UseFirstHook.ts
| | | | 📄 index.ts
| | | | 📄 index.test.ts
| | | | 📄 Styles.ts
| | | | 📄 Types.ts
================================================================================
| 📄 App.test.ts
| 📄 App.vue
| 📄 main.css
| 📄 main.ts
```

### File Structure Conventions

- Folders & Files in `/src` should use `PascalCase` for file names except for the following:

  - `/src/main.ts`
  - `/src/main.css`

- The top level `Components` folder should be for generic, used anywhere components (Like`HamburgerButton`, `SideNav`, `Input`). `Components` can have other `Components` as children.

- The top level `Modules` are really big (epic or feature level) components made up of smaller components. `Modules` can have other `Modules` and `Components` as children. The hope is that individual `Modules` are not be aware of other sibling `Modules`. The `src/API`, and `src/Providers` should help facilitate the communication across sibling `Modules`.

## ESLint and Prettier

### What is ESLint

[ESLint](https://eslint.org/) is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of making code more consistent and avoiding bugs.

Use the following command to run ESLint:

```terminal
npm run lint
```

Some parts of the code can be automatically fix. To automatically fix some ESLint errors run the following command:

```terminal
npm run lint:fix
```

### What Is Prettier

Prettier is used to format our code to conform to a consistent style.

### Linting & Prettier Disable Conventions

Please follow these 2 conventions When disabling a line or block of code:

**Convention 1** - Only disable the offending rule, not all of eslint. Example:

**Good** = `/* eslint disable no-console */`\
**Bad** = `/* eslint disable */`

**Convention 2** - Provide a note explaining why the rule is disabled

### Eslint Ignore Node

To disable a line of code do the following:

```js
// eslint-disable-next-line no-console
console.log("bar");
```

To disable a block of code do the following:

```js
/* eslint-disable no-console */

console.log("bar");

/* eslint-enable no-console */
```

### Prettier Ignore Node

In some cases prettier will reformat code that we don't want reformated. We can use `// prettier-ignore` to exclude the next node from formatting. For example:

```js
matrix(1, 0, 0, 0, 1, 0, 0, 0, 1);

// prettier-ignore
matrix(
  1, 0, 0,
  0, 1, 0,
  0, 0, 1
)
```

will be transformed to:

```js
matrix(1, 0, 0, 0, 1, 0, 0, 0, 1);

// prettier-ignore
matrix(
  1, 0, 0,
  0, 1, 0,
  0, 0, 1
)
```

### Ignore root files or directories

If a root file or directory needs to be ignored by ESLint or Prettier then add the file/directory name to the `.eslintignore` or `.prettierignore` files.

⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️
⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin) to make the TypeScript language service aware of `.vue` types.

If the standalone TypeScript plugin doesn't feel fast enough to you, Volar has also implemented a [Take Over Mode](https://github.com/johnsoncodehk/volar/discussions/471#discussioncomment-1361669) that is more performant. You can enable it by the following steps:

1. Disable the built-in TypeScript Extension
   1. Run `Extensions: Show Built-in Extensions` from VSCode's command palette
   2. Find `TypeScript and JavaScript Language Features`, right click and select `Disable (Workspace)`
2. Reload the VSCode window by running `Developer: Reload Window` from the command palette.

## Customize configuration

See [Vite Configuration Reference](https://vitejs.dev/config/).

## Project Setup

```sh
npm install
```

### Compile and Hot-Reload for Development

```sh
npm start
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
