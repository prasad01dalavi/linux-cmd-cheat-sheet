# Linux Commands
```
sudo grep -r '^psk=' /etc/NetworkManager/system-connections/            # Show Wi-Fi Passwords
cp -r path_to_source path_to_destination/                               # Copy the Directory

scp -v <file_name.extension> username@ip_address:                       # -v is for debug log on console
scp -v -r <folder_name> username@ip_address:                            # -r is recursively (complete) folder
scp remote_username@remote_ip:/remote/file /local/file                  # Copy data from remote machine to local machine
scp -v -i <key.pem> -r <folder_name> ec2_username@public_ip_address:    # copy dir to ec2 linux machine

rename 's/test_//g' *                                                   # rename by removing the test_ at the start of all  
sudo fuser -k port_number/tcp                                           # Kill already running port    
mkdir -p test_dir/{"a","b","c","d"}                                     # create nested directories

ls ~/.ssh/id_*                                                          # check existing ssh key
ssh-keygen -t rsa -b 4096 -C "your_email@domain.com"                    # Generate ssh key





```
