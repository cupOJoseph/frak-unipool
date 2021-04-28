# FRAK Unipool LP mining

#### FRAK Token: TBD - to be deployed

#### FRAK Uniswap Exchange: TBD

### Run tests

1) Install all dependencies in the root directory execute:
```
$ npm install
```

2) Run tests with:
```
$ npm run test
```

### Deploy to a network

1) Install all dependencies if not already installed:
```
$ npm install
```

2) Update the gas price to whatever is currently being accepted by the network in the `truffle-config.js` file.

3) Deploy to xDai. Set your private key mnemonic in the `MNEMONIC` environment variable.

```
$ npx truffle deploy --network mainnet
```

### Create a reward (will be spread across 30 days)

1) Approve the Unipool contract address to take reward amount. If the contract is verified on Etherscan you can
use MetaMask and their contract interface to do this. Otherwise use your preferred method for interacting with contracts.

2) Add a reward amount by going to the Etherscan UI at the Unipool contract address, connecting the MetaMask account 
and excuting `notifyRewardAmount(amount)` with the amount to reward. Remember the amount is padded with 18 zeros. Eg a reward
of 1000 HNY tokens would be 1000000000000000000000. 




