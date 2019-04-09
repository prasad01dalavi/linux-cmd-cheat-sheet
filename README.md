# Linux Commands
```
# Show Wi-Fi Passwords:
sudo grep -r '^psk=' /etc/NetworkManager/system-connections/

cp -r path_to_source path_to_destination/           # Copy the Directory

# Transfer files/folders using SCP
scp -v <file_name.extension> username@ip_address:   # -v is for debug log on console
scp -v -r <folder_name> username@ip_address:        # -r is recursively (complete) folder


```
