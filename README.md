# Linux Commands
```
sudo grep -r '^psk=' /etc/NetworkManager/system-connections/            # Show Wi-Fi Passwords
cp -r path_to_source path_to_destination/                               # Copy the Directory

scp -v <file_name.extension> username@ip_address:                       # -v is for debug log on console
scp -v -r <folder_name> username@ip_address:                            # -r is recursively (complete) folder
scp remote_username@remote_ip:/remote/file /local/file                  # Copy data from remote machine to local machine
scp -v -i <key.pem> -r <folder_name> ec2_username@public_ip_address:    # copy dir to ec2 linux machine
scp -i <ssh pvt key> file/dir remote_user@ip_address:                   # Copy files from local system to gcp vm

rename 's/test_//g' *                                                   # rename by removing the test_ at the start of all  
sudo fuser -k port_number/tcp                                           # Kill already running port    
mkdir -p test_dir/{"a","b","c","d"}                                     # create nested directories

ssh-keygen -t rsa                                                       # generate ssh private and public key
ssh-copy-id username@ip_address                                         # copy public key to the ip_address host (to access it)
ls ~/.ssh/id_*                                                          # check existing ssh key
ssh-keygen -t rsa -b 4096 -C "your_email@domain.com"                    # Generate ssh key

sudo find / -iname <file or dir name>                                   # find the location of file or dir
du -shc *                                                               # List the files with size

grep "model name" /proc/cpuinfo | wc -l                                 # Number of CPUs available


# My Terminal Configuration:
1. .bashrc file
orange=$(tput setaf 166);
yellow=$(tput setaf 228);
green=$(tput setaf 71);
white=$(tput setaf 15);
bold=$(tput bold);
reset=$(tput sgr0);

PS1="\[${bold}\]\n";
PS1+="\[${orange}\]\u";   # username
PS1+="\[${white}\] at ";
PS1+="\[${yellow}\]\h";   # host
PS1+="\[${white}\] in ";
PS1+="\[${green}\]\W";     # working directory
PS1+="\n";
PS1+="\[${white}\]\$ \[${reset}\]";    # $ and reset color
export PS1;

2. .bash_profile file
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
source /usr/local/bin/virtualenvwrapper.sh
echo 'FROM BASH_PROFILE'

if [ -f ~/.bashrc ]; then 
    source ~/.bashrc
fi

```
