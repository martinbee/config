# VSCODE SETTINGS SYNC
https://gist.github.com/martinbee/fd073ec33c8d1b08d508a48136f99391

^Update eslint.nodePath to point towards global node modules

# General Guidelines
- Use package manager (Homebrew, apt, etc.)
- For Mac we will use Homebrew

- Install VsCode and sign in using github
- Install Cursor and import VsCode Settings (https://cursor.sh/)
- Install Homebrew
  - /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
- Install spf13
  - Here for instructions (https://github.com/spf13/spf13-vim)
  - Current as of April 2017 curl: curl https://j.mp/spf13-vim3 -L > spf13-vim.sh && sh spf13-vim.sh
  - Remove Bundle 'amirh/HTML-AutoCloseTag' from .spf13-vim-3/.vimrc.bundles
  - Disable spell (remove set spell line in .spf13-vim-3/.vimrc)
- Install the_silver_searcher
  - brew install the_silver_searcher
- Install OhMyZsh: https://github.com/robbyrussell/oh-my-zshZsh
  - sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  - This should also set zsh to be default shell
  - Update .zshrc to point to correct .oh-my-zsh path
- Install NVM (we use zsh to keep this plugin up to date and seamless)
  - git clone https://github.com/lukechilds/zsh-nvm ~/.oh-my-zsh/custom/plugins/zsh-nvm
- Install git-open (we use zsh to keep this plugin up to date and seamless)
  - git clone https://github.com/paulirish/git-open.git $ZSH_CUSTOM/plugins/git-open
- Setup custom settings
  - Copy .vimrc.local, .zshrc, to ~/
  - Change .zshrc path export reference to use your path to .oh-my-zsh
  - Copy custom airline theme seoul256 to .vim/bundle/vim-airline-themes/autoload/airline/themes/
