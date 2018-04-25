### VIM 配置

Use [vim-pathogen](https://github.com/tpope/vim-pathogen) to manage the vim plugins

**vim-pathogen** 将 vim 插件组织在 `~/.vim/bundle` 下，并在运行时加载，比如要安装某插件，只要把该插件拷贝到 `~/.vim/bundle` 下，如果要删除某插件，只需要将`~/.vim/bundle` 下对应的插件删除。配合 GitHub 可以更方便的管理插件，比如：直接在 `~/.vim/bundle` 下 `git clone` 某个插件，更新的时候直接使用 `git pull`
