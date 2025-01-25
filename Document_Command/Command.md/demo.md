####################################
#######Step-1:Install Apache2#######
####################################
yes|sudo apt update
yes|sudo apt install apache2

#######################################
#######Step-2:Install Docker###########
#######################################

#Add Docker offical GPG Key:
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install-m 0755 -d /etc/apt/keyrings
curl-fsSL https://download.docker.com/linux/ubuntu/gpg|sudo gpg-dearmor
-o/etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

#Add the repository to Apt sources