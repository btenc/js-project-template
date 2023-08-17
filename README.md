# Javascript Project Template

My personal basic project template using webpack and development packages that I use, along with the scripts I use on every project.

## What's included?

- Webpack bundler already setup
- All files linked properly
- Build scripts that output into `./dist` folder and configured to clean the folder before building
- Github Pages `./dist` folder branch and publishing script
- ESLint with Airbnb format enabled in `.eslintrc.json`
- ESLint and Prettier conflicts fixed with `eslint-plugin-prettier`
- Normalize.css imported in `index.js` (my preferred CSS reset)
- Inline source map devtool enabled in `webpack.config.js`
- HtmlWebpackPlugin already configured in `webpack.config.js`
- style-loader and css-loader configured in `webpack.config.js`

## Guide

- **Install** all packages with `npm install`
- **Build** the project using webpack with `npm run build`
- **Build** the project on save using webpack with `npm run build-watch`
- **Publish** a dist folder github pages branch with `npm run github-pages-deploy`
- **Lint** JS files in the src folder with `npm run lint`

## Optional if you use VSCode:

- `Prettier - Code Formatter` VSCode Plugin
- `ESLint VS Code Plugin` VSCode Plugin

- Add config below to your VSCode settings.json to automatically lint and format on save.

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
