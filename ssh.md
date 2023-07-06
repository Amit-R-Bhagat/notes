What it does ? 
Connect and work on remote machine

ssh = ssh-client + ssh-daemon
authorized-keys is used by daemon o n remote machine

| command | explanation |
| --------------- | ----------- |
| ssh-keygen | generate key pair |
| ssh-keygen -b 4096 | generate key pair with 4096 bits (default 3072) |
| ssh-keygen -l | key pair fingerprint |
| ssh-copy-id | copy public key to remote |
| ssh remote_host | connect to remote_host with same user as local_machine |
| ssh username@remote_host | connect to remote_host with username user |
| ssh username@remote_host command | connect to remote and run command |
| /etc/ssh/sshd_config (file) | config file for daemon |
| ~/.ssh/config | config file for client (optional) |


``` man ssh_config ``` is useful for seeing all fields possible in the config.

Tunneling is a way to route your traffic via ssh connection.
Local Tunneling routes traffic from your local machine to remote host.
Remote Tunneling routes traffic from remote lost to local machine.