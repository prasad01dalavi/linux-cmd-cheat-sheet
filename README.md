# Linux Commands
```
sudo grep -r '^psk=' /etc/NetworkManager/system-connections/            # Show Wi-Fi Passwords
cp -r path_to_source path_to_destination/                               # Copy the Directory
scp -v <file_name.extension> username@ip_address:                       # -v is for debug log on console
scp -v -r <folder_name> username@ip_address:                            # -r is recursively (complete) folder
scp -v -i <key.pem> -r <folder_name> ec2_username@public_ip_address:    # copy dir to ec2 linux machine
rename 's/test_//g' *                                                   # rename by removing the test_ at the start of all  
sudo fuser -k port_number/tcp                                           # Kill already running port                                 

```
