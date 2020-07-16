# Configuration

## Code editor

We use [Visual Studio Code](https://code.visualstudio.com/) for all our projects. You can use any code editor of your choice, but you have to maintain our standards.

## Plugins

To help you maintain our standards you can use the following plugins:

- [Prettier (Must use)](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Better comments (Must use)](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
- [Live Sass Compiler (Must use)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)
- [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2)

## VS Code configuration

You must use the following settings otherwise **Domino's Pizza** will have a lot of business from us (you 😉)

```javascript
{
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
 "editor.tabSize": 2,
 "prettier.printWidth": 90,
 "prettier.vueIndentScriptAndStyle": true,
 "prettier.trailingComma": "none",
 "prettier.singleQuote": true,
 "prettier.semi": false,
 "editor.formatOnSave": true,
 "javascript.preferences.quoteStyle": "single",
 "typescript.format.semicolons": "remove",
 "javascript.format.semicolons": "remove",
 "liveSassCompile.settings.formats": [
   {
     "format": "expanded",
      "extensionName": ".css",
      "savePath": "~/../css/"
    }
  ],
}
```
