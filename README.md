# Javascript Project Template

My personal basic project template using webpack and development packages that I use, along with the scripts I use on every project.

## What's included?

- All the packages listed in `package.json` are already setup and configured with general settings
- Webpack bundler already setup
- All files linked properly
- Build scripts that output into `./dist` folder and are configured to clean the folder before building
- Github Pages `./dist` folder branch and publishing script
- ESLint with Airbnb format enabled in `.eslintrc.json`
- ESLint and Prettier conflicts fixed with `eslint-plugin-prettier`
- Normalize.css imported in `index.js` (my preferred CSS reset)
- Inline source map devtool enabled in `webpack.config.js`

## Guide

### How to create a repository with this template

1. Click the green "Use This Template" on this page -> "Create a new repository"
1. Name the repository and clone it on your local machine
1. Navigate to the repository's local folder and open in your preferred code editor
1. **Install** all packages listed in `package.json` with `npm install`

### Included scripts

- **Build** the project using webpack with `npm run build`
- **Build** the project on save using webpack with `npm run build-watch`
- **Publish** a dist folder github pages branch with `npm run github-pages-deploy`
- **Lint** JS files in the src folder with `npm run lint`

## Optional if you use VSCode:

- `Prettier - Code Formatter` VSCode Plugin
- `ESLint VS Code Plugin` VSCode Plugin

- Add config below to your VSCode settings.json to automatically lint with ESLint and format with Prettier on save.

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
