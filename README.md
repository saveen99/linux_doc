


# linux_doc

***

### Java Installation

`
sudo apt update
`

`
sudo apt install default-jre
`

`
sudo apt install default-jdk
`



***

### Install Fish Shell in Ubuntu

`
sudo apt install fish -y
`

### Install Ohmyposh

`
sudo wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/posh-linux-amd64 -O /usr/local/bin/oh-my-posh
`

`
sudo chmod +x /usr/local/bin/oh-my-posh
`

### Download and Install Firacode Nerd Fonts

`
mkdir -p $HOME/.local/share/fonts
`

`
wget https://github.com/ryanoasis/nerd-fonts/releases/download/v3.2.1/FiraCode.zip -O $HOME/Downloads/firacode.zip
`

`
unzip $HOME/Downloads/firacode.zip -d $HOME/.local/share/fonts
`

`
fc-cache -f -v
`

`
sudo apt install gnome-tweaks -y
`

### Download & Install Ohmyposh Themes

`
mkdir ~/.poshthemes
`

`
wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/themes.zip -O ~/.poshthemes/themes.zip
`

`
unzip ~/.poshthemes/themes.zip -d ~/.poshthemes
`

`
chmod u+rw ~/.poshthemes/*.json
`

`
rm ~/.poshthemes/themes.zip
`

### Add Ohmyposh Theme to Fish Config

`
gnome-text-editor $HOME/.config/fish/config.fish
`

Paste the code line top of the file

`
oh-my-posh init fish --config $HOME/.poshthemes/montys.omp.json | source
`

### Change Terminal Color Scheme

`
bash -c  "$(wget -qO- https://git.io/vQgMr)" 
`
