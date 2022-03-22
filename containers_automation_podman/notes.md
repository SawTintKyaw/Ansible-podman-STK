
ansible all -m raw -a "show version"
ansible all -m raw -a "show ip interface brief"
ansible all -m raw -a "show ip interface brief" -c ssh


ansible all -m ios_command -a "commands='show ip int brief'" -c network_cli
ansible all -m ios_ping -a "dest=192.168.122.1"



ansible all -m ios_ping -a "dest=192.168.122.1" -c network_cli


ansible all -m ping -c network_cli
ansible all -m ping -c local



