# VSCODE SETTINGS SYNC
https://gist.github.com/martinbee/fd073ec33c8d1b08d508a48136f99391

^Update eslint.nodePath to point towards global node modules

# General Guidelines
- Use package manager (Homebrew, apt, etc.)
- For Mac we will use Homebrew

- Install Iterm2
  - https://www.iterm2.com/
  - In preferences/keys on the bottom right enable show/hide Iterm2 with system wide hotkey and hotkey toggles a dedicated profile
  - Import seoul color scheme for iterm2
- Install Homebrew
  - /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
- Install node/npm
  - brew install node
- Install vim with lua
  - brew install luajit
  - brew install vim --with-luajit
- Install spf13
  - Here for instructions (https://github.com/spf13/spf13-vim)
  - Current as of April 2017 curl: curl https://j.mp/spf13-vim3 -L > spf13-vim.sh && sh spf13-vim.sh
  - Remove Bundle 'amirh/HTML-AutoCloseTag' from .spf13-vim-3/.vimrc.bundles
  - Disable spell (remove set spell line in .spf13-vim-3/.vimrc)
- Install tmux
  - brew install tmux
- Install tmuxinator
  - sudo gem install tmuxinator
  - Copy .tmuxinator/ from config to your root
- Install the_silver_searcher
  - brew install the_silver_searcher
- Install reattach-to-user-namespace
  - brew install reattach-to-user-namespace
- Get powerline fonts
  - git clone https://github.com/powerline/fonts.git
  - cd into repo and run sh install.sh
  - Change fonts on iterm profile to a powerline font
- Install zsh
  - brew install zsh
- Install OhMyZsh: https://github.com/robbyrussell/oh-my-zshZsh
  - sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  - This should also set zsh to be default shell
- Install NVM (optional)
  - git clone https://github.com/lukechilds/zsh-nvm ~/.oh-my-zsh/custom/plugins/zsh-nvm into ~/.oh-my-zsh/custom/plugins/
  - Add zsh-nvm to plugins in .zshrc (i.e. plugins=(git) now plugins=(git zsh-nvm))
- Setup custom settings
  - Copy .tmux.conf, .vimrc.local, .zshrc, .czrc, and .gitconfig to ~/
  - Change .zshrc path export reference to use your path to .oh-my-zsh
  - Copy custom airline theme seoul256 to .vim/bundle/vim-airline-themes/autoload/airline/themes/
- Install Icdiff (https://github.com/jeffkaufman/icdiff) if desired
- Linting
  - npm i -g eslint eslint-config-airbnb eslint-plugin-import eslint-plugin-jsx eslint-plugin-react eslint-plugin-jsx-a11y eslint-plugin-mocha babel-eslint
  - eslint --init in your project
- Install esformatter
  - npm i -g esformatter
  - PluginInstall to ensure esformatter plugin is properly installed
  - Change esformatter presets
    - Go to (/usr/local/lib/node_modules/esformatter/lib/preset/);
    - Modify default-whitespace-after and default-whitespace-before so that
      ObjectPatternClosing or OpeningBrace have a 1 and not 0.
    - To use esformatter type ',fe' in vim in normal or visual mode
- Install commitizen
  - npm i -g commitizen
  - npm i -g cz-conventional-changelog
