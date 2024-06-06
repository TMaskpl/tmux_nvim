## Install NeoVim and Tmux

```
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux64.tar.gz

sudo rm -rf /opt/nvim

sudo tar -C /opt -xzf nvim-linux64.tar.gz

export PATH="$PATH:/opt/nvim-linux64/bin"

apt install -y tmux


## Install Lazyvim

```
mv ~/.config/nvim{,.bak}

mv ~/.local/share/nvim{,.bak}

mv ~/.local/state/nvim{,.bak}

mv ~/.cache/nvim{,.bak}

git clone https://github.com/LazyVim/starter ~/.config/nvim

rm -rf ~/.config/nvim/.git

nvim
