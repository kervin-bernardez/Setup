# Setup
# Download setup github repo
```
git clone https://github.com/kervin-bernardez/Setup.git ~/Downloads/Setup
cd ~/Downloads/Setup && sudo cp Material-Black-Lime-Numix-FLAT /usr/share/icons
```

# Install updates and packages
```
sudo apt update -y && sudo apt upgrade -y
sudo apt install flameshot terraform bloodhound -y
```

# Install ohmyzsh
```
sh -c "$(wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh --no-check-certificate -O -)"
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
sudo cp ~/.zshrc ~/.zshrc-bak && sudo cp .zshrc ~/.zshrc
soruce ~/.zshrc
```

# Install sublime
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/sublimehq-archive.gpg > /dev/null
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```

# Download github repo
```
sudo git clone https://github.com/danielmiessler/SecLists.git /opt/Seclists
sudo git clone https://github.com/nicocha30/ligolo-ng.git /opt/ligolo
```

# Dowload linux tools
```
wget https://github.com/peass-ng/PEASS-ng/releases/download/20241205-c8c0c3e5/linpeas.sh --no-check-certificate
wget https://github.com/DominicBreuker/pspy/releases/download/v1.2.1/pspy64
wget https://github.com/DominicBreuker/pspy/releases/download/v1.2.1/pspy32
```

# Dowload windows tools
```
wget https://github.com/peass-ng/PEASS-ng/releases/download/20241205-c8c0c3e5/winPEASany.exe --no-check-certificate
wget https://raw.githubusercontent.com/ivan-sincek/powershell-reverse-tcp/refs/heads/master/src/invoke_expression/original/powershell_reverse_tcp.ps1 --no-check-certificate
wget https://raw.githubusercontent.com/ivan-sincek/powershell-reverse-tcp/refs/heads/master/src/invoke_expression/original/powershell_bind_tcp.ps1 --no-check-certificate
```

# Download dev tools
```
curl "https://awscli.amazonaws.com/awscli-exe-linux-aarch64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```
