## Command Line

sudo apt-get update

sudo apt-get upgrade

sudo apt-get install vim, git, transmission, filezilla, vlc, steam, zsh

sudo add-apt-repository ppa:stebbins/handbrake-releases

sudo apt-get update

sudo apt-get install handbrake-gtk

### Node
curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -

sudo apt-get install -y nodejs

### ZSH
zsh --version

chsh -s $(which zsh)

npm install --global pure-prompt

vim ~/.zshrc

add > ZSH_THEME="pure"

### PIA
[Link - PIA Forum](https://helpdesk.privateinternetaccess.com/hc/en-us/articles/219438217-Installing-the-PIA-App-on-Linux)

### MakeMKV
[Link - MakeMKV Forum](http://www.makemkv.com/forum2/viewtopic.php?f=3&t=224)

- Install required packages on Ubuntu
sudo apt-get install build-essential libc6-dev libssl-dev libgl1-mesa-dev libqt4-dev

- Download Files
wget http://www.makemkv.com/download/makemkv_v1.5.6_beta_oss.tar.gz
wget http://www.makemkv.com/download/makemkv_v1.5.6_beta_bin.tar.gz

- Unzip Files and Remove tarballs
tar -xvvf makemkv_v1.5.6_beta_oss.tar.gz
tar -xvvf makemkv_v1.5.6_beta_bin.tar.gz
rm makemkv_v1.5.6_beta_oss.tar.gz
rm makemkv_v1.5.6_beta_bin.tar.gz

- Build OSS and BIN
cd makemkv_v1.5.6_beta_oss/

make -f makefile.linux

sudo make -f makefile.linux install

cd ../makemkv_v1.5.6_beta_bin/

make -f makefile.linux

sudo make -f makefile.linux install

cd ..

- Remove Directories
sudo rm -r makemkv_v1.5.6_beta_oss/

sudo rm -r makemkv_v1.5.6_beta_bin/
