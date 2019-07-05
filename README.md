# Hyperledger-Dev
permissioned Blockchain development Environment
 
 ## First-network
 
 #### Pre-requisites
 
```
 ****Docker***
 
 sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
apt-cache policy docker-ce
sudo apt install docker-ce

***Go-lang**

wget https://dl.google.com/go/go1.12.6.linux-amd64.tar.gz

sudo tar -xvf go1.12.6.linux-amd64.tar.gz
sudo mv go /usr/local
export GOROOT=/usr/local/go
export GOPATH=$HOME/go  #choose your prferred work directory path
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

***Node.js and Npm***

sudo apt-get install nodejs
sudo apt-get install npm

***Fabric-samples Docker images***

curl -sSL http://bit.ly/2ysbOFE | bash -s 1.3.0

