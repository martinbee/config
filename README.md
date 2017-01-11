# General Guidelines
- Install homebrew
- Check if vim with lua is installed (if not install via homebrew)
- Follow spf13 vim installation instructions
- Disable spell (remove set spell line in .spf13-vim-3/.vimrc)
- Clone this repo and run install.sh to get fonts: https://github.com/vim-airline/vim-airline/issues/142
- Set up OhMyZsh: https://github.com/robbyrussell/oh-my-zshZsh
- gem install tmuxinator
- add the default.yml to .tmuxinator/
- Add custom airline theme seoul256

## Typescript Specific
- add the snippet below before syntax = on in .vimrc after spf13 installation to get ts highlighting
```
"Typescript
    Plugin 'leafgarland/typescript-vim'
```



