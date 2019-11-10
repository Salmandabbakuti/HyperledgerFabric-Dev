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
sudo apt install docker-compose

***Go-lang**

wget https://dl.google.com/go/go1.12.6.linux-amd64.tar.gz

sudo tar -xvf go1.12.6.linux-amd64.tar.gz
sudo mv go /usr/local
export GOROOT=/usr/local/go
export GOPATH=$HOME/go  #choose your prferred work directory path
export PATH=$GOPATH/bin:$GOROOT/bin:$PATH

***Node.js and Npm***
 
 curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash - 
 sudo apt-get install -y nodejs  #node v12.xx

***Fabric-samples Docker images***

curl -sSL http://bit.ly/2ysbOFE | bash -s


```

Build your Network

```
cd fabric-samples/first-network 
sudo ./byfn.sh generate       #Generates Certificates for network
sudo ./byfn.sh up             #Creates Genesis state and starts network

sudo ./byfn.sh down           #Stops Network

```

#### Creating Personalized Network

##### Work Flow

1. Configuring Network Organizations
2. Certificates Generation
3. Configuring Gensis-states and Channel Transactions
4. Containerization of Orgs
5. Bringing Up Network
