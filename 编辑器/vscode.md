# vscode 配置

## setting.json

```json
{
  "beautify.config": {
    "newline_between_rules": false,
    "selector_separator_newline": false
  },
  "files.eol": "\n",
  // 禁用默认验证。
  "javascript.validate.enable": false,
  "css.validate": false,
  "scss.validate": false,
  // 启用后，将在保存文件时剪裁尾随空格。
  "files.trimTrailingWhitespace": true,
  "git.autofetch": true,
  "editor.fontSize": 13,
  // vscode默认启用了根据文件类型自动设置tabsize的选项
  "editor.detectIndentation": false,
  "editor.tabSize": 2,
  "editor.lineHeight": 25,
  // #值设置为true时，每次保存的时候自动格式化；值设置为false时，代码格式化请按shift+alt+F
  "editor.formatOnSave": false,
  "files.associations": {
    "*.vue": "vue",
    "*.js": "javascriptreact"
  },
  "eslint.options": {
    "extensions": [
      ".js",
      ".vue"
    ]
  },
  "eslint.validate": [
    "javascript",
    "html",
    "javascriptreact",
    "vue"
  ],
  "search.exclude": {
    "**/node_modules": true,
    "**/bower_components": true,
    "**/dist": true
  },
  "emmet.syntaxProfiles": {
    "javascript": "jsx",
    "vue": "html",
    "vue-html": "html"
  },
  "git.confirmSync": false,
  "window.zoomLevel": 0,
  "editor.renderWhitespace": "boundary",
  "editor.cursorBlinking": "smooth",
  "editor.minimap.enabled": true,
  "editor.minimap.renderCharacters": false,
  "window.title": "${dirty}${activeEditorMedium}${separator}${rootName}",
  "editor.codeLens": true,
  "editor.snippetSuggestions": "top",
  "explorer.confirmDelete": false,
  //  #让函数(名)和后面的括号之间加个空格
  "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "files.autoSave": "afterDelay",
  "settingsSync.ignoredExtensions": [],
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Dracula",
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  },
  "editor.rulers": [],
  "editor.renderIndentGuides": false,
  "editor.highlightActiveIndentGuide": false,
  "editor.renameOnType": true
}
```

## 插件

[参考](https://segmentfault.com/a/1190000015157970)
[参考](https://segmentfault.com/a/1190000011779959?utm_source=sf-related)
