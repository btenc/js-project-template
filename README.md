# Webpack JS Project Template

My personal project template using webpack and development packages that I use, along with the scripts I use on every project.

All the packages listed in `package.json` are already setup and configured with all-purpose settings. To see how things are configured specifically or to make changes check `webpack.config.js` and `.eslintrc.json`

## What's configured?

- Webpack (module bundler)
- Normalize.css (CSS Reset)
- ESLint (linter)
  - Setup with Airbnb style guide
- Prettier (code formatter)
  - Includes eslint-config-prettier to solve conflicts between ESLint and Prettier
- Jest for TDD
- css-loader and style-loader to bundle `.css` files
- html-webpack-plugin to bundle `.html` files
- Various development and hosting scripts

## Guide

### How to create a repository with this template

1. Click the green "Use This Template" on this page -> "Create a new repository"
1. Name the repository and clone it on your local machine
1. Navigate to the repository's local folder and open in your preferred code editor
1. **Install** all packages listed in `package.json` with `npm install`
1. Program in the `./src` folder, use included scripts to build your project, (output is in `./dist`)

### Included scripts

- **Build** the project to `./dist` using webpack with `npm run build`
- **Build** the project on save to `./dist` using webpack with `npm run build-watch`
- **Publish** a dist folder github pages branch with `npm run github-pages-deploy`
- **Lint** `.js` files in the `./src` folder with `npm run lint`

## Optional if you use VSCode:

- `Prettier - Code Formatter` VSCode Plugin
- `ESLint VS Code Plugin` VSCode Plugin

- Add config below to your VSCode `settings.json` (either for your workspace or user settings) to automatically lint with ESLint and format with Prettier on save.

```
"editor.formatOnSave": true,
"[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
},
"[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
},
"[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
},
"editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
},
"eslint.validate": ["javascript"]
```
