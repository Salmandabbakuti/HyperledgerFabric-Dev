## Manual Setup Of First-Nework

##### Work Flow

1. Configuring Network Organizations 

2. Certificates Generation

3. Configuring Gensis-states and Channel Transactions

4. Containerization of Orgs

5. Bringing Up Network 

6. Chaincode Installation and Instantiations

7.Invoking & Querying Chaincode on Peers

 #### 1. Configuring Network Organizations
 
 Pre-Configured ie. ```crypto-config.yaml``` and ```configtx.yaml```

#### 2. Certificates Generation

Export Your ```fabric-samles``` path

```
export PATH=<replace this with your path>/bin:$PATH
```

In your firstnetwork directory, 

```
../bin/cryptogen generate --config=./crypto-config.yaml
```

