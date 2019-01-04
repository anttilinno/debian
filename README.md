# debian
Debian related things

## preseed.txt
Debian stretch preseed file I found useful in VirtualBox to kickstart my K8s environment.

 - Locale en_US
 - keymap US
 - Automatic network configuration (have not found an easy way to disable ipv6 network check)
 - Add estonian debian mirror
 - Set up a root account with password *meh*
 - Timezone Europe/Tallinn, hardware clock set to UTC
 - NTP is used to sync time
 - Partition whole disk automatically (I usually make 20GB disk in VBox). **No SWAP!**
 - Add repositories for Docker and Kubernetes
 - Install ssh service
 - Setup grub to /dev/sda
 - Install docker-ce, docker-compose
 - Install kubelet, kubeadm, kubectl
 - Add user antti to group docker
 - Create user antti with password *meh*
