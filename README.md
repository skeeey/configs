## VIM 配置

Use [vim-pathogen](https://github.com/tpope/vim-pathogen) to manage the vim plugins

**vim-pathogen** 将 vim 插件组织在 `~/.vim/bundle` 下，并在运行时加载，比如要安装某插件，只要把该插件拷贝到 `~/.vim/bundle` 下，如果要删除某插件，只需要将`~/.vim/bundle` 下对应的插件删除。配合 GitHub 可以更方便的管理插件，比如：直接在 `~/.vim/bundle` 下 `git clone` 某个插件，更新的时候直接使用 `git pull`

## VSCode 配置

### 设置
```json
{
    "workbench.editor.enablePreview": false,
    "workbench.editor.enablePreviewFromQuickOpen": false,
    "editor.minimap.enabled": false,
    "files.exclude": {
        ".vscode": true,
        "**/target": true,
        "**/.settings": true,
        "**/.classpath": true,
        "**/.project": true,
        "**/Chrome_*": true,
        "**/PhantomJS_*": true,
        "**/typings": true,
        "**/.jazzignore": true
    },
    "search.exclude": {}
}
```

### MAC 快捷键
```json
[
    { "key": "cmd+d",   "command": "editor.action.deleteLines",
                        "when": "editorTextFocus" },
    { "key": "shift+cmd+k",     "command": "editor.action.addSelectionToNextFindMatch",
                        "when": "editorFocus" },
    { "key": "shift+cmd+o",     "command": "workbench.action.files.openFileFolder" },
    { "key": "cmd+o",   "command": "workbench.action.gotoSymbol" },
    { "key": "alt+/",   "command": "editor.action.triggerSuggest",
                        "when": "editorHasCompletionItemProvider && editorTextFocus && !editorReadonly"  }
]
```

### Windows 换行
```
    "files.eol": "\n",
```

### Windows 终端（[cmder](http://cmder.net/)）
```
"terminal.integrated.shell.windows": "cmd.exe",
"terminal.integrated.shellArgs.windows": [
        "/k", "C:\\Tools\\cmder\\vendor\\init.bat"
    ]
```