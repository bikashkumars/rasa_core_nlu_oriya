## Install C and C++ in Ubuntu
sudo apt install gcc
sudo apt-get install g++

## Install Conda in Linux
Login to Linux and Open Terminal or SSH to your server and Execute following command

# download 
Download Mini Conda Shell Script File
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh

Execute Shell script
bash Miniconda3-latest-Linux-x86_64.sh

# Add Conda Path to Ubuntu/Linux Bash Path. So that Conda command will work every where
vm  ~/.profile

Press i
Add this line at the end
PATH=$PATH:$HOME/miniconda3/bin

To Exit VI - press ESC then ; and then wq (to save VI editor and Quit)

Exit VI editor and execute following command
source ~/.profile

Now fire this command, this should work
conda --version