
## Step 1: Start IPFS locally

Open a terminal window and run the script `startipfs.sh` to start IPFS locally.

## Step 2: Ganache

Start Ganache as your development Ethereum node.

## Step 3: Import Ganache accounts

From Metamask, import private keys for at least 2 accounts including the first one.

## Step 4: Configure your project

Open the app project.

Edit your file `truffle-config.js` to set the port number used by Ganache.

## Step 5: Deploy the smart contract

Open a terminal window from your app folder.

Compile and migrate the smart contract (AssetContract) to Ganache:

```
$ truffle migrate --reset --compile-all --network ganache
```

## Step 6: Copy the contract settings

Your app project requires some settings from the deployed smart contract.

Run the following script from the app folder:

```
$ npm run contracts
```

## Step 7: Run APP

Run the Dapp from the app folder:

```
$ npm start
```

