# Scripts Overview

## Contract Scripts

Below are npx scripts provided by `Starknet-Scaffold` for your smart contract development.

### Build Contract

To build your contracts:
```
npm run build-contracts
```

### Format contracts
Leverage `Scarb’s` native formatting capabilities by running:
```
npm run format-contracts
```

#### Verify contracts

To verify your smart contracts, from the base repository run:

```
npm run verify-contracts --contract-address=<CONTRACT_ADDRESS> --contract-name=<CONTRACT_NAME> --network=<NETWORK>
```

### Test contracts
To run your Starknet Foundry tests:
```
npm run test-contracts
```

### Run custom `starknet-foundry` scripts
To run a custom starknet foundry deploy/declare/invoke script:
```
npm run contract-scripts <SCRIPT_NAME> --url=<RPC_URL>
```

### Generate an SRC-5 interface ID for your contracts
To generate an `SRC-5 interface ID`, run:
```
npm run generate-interface <PATH_TO_INTERFACE>
```

### Prepare Account for deployment
To prepare your account for deployment, run:
```
npm run prepare-account --url=<RPC_URL> --name=<ACCOUNT_NAME> <PROFILE_NAME>
```
generates a profile which is added to scarb.toml and can be passed to other commands.

### Deploy Account
To deploy an account:
```
npm run deploy-account --profile=<MY_PROFILE> --name=<ACCOUNT_NAME> --feetoken=<FEE_TOKEN> --maxfee=<MAX_FEE>
```
where the profile is gotten from `snfoundry.toml`, name is the prepared account and maxfee is the specified max fee.

### Delete Account
To delete an account:
```
npm run delete-account --profile=<MY_PROFILE> --accountfile=<PATH_TO_ACCOUNT_FILE> --name=<ACCOUNT_NAME> --network=<alpha-mainnet | alpha-goerli>
```

### Declare Contract
To declare a Starknet contract:
```
npm run declare-contract --profile=<MY_PROFILE> --contract=<CONTRACT_NAME> --feetoken=<FEE_TOKEN>
```

### Deploy Contract
To deploy a contract:
```
npm run deploy-contract --profile=<MY_PROFILE> --feetoken=<FEE_TOKEN> --class=<CONTRACT_CLASSHASH>
```

###  Starknet-Devnet
Confirm that Docker is installed and running to use starknet-devnet. To run devnet:
```
npm run devnet
```


## Dojo Scripts
The `contracts` folder contains all the tools needed to write, build, test and deploy dojo projects. It is built with sozo and katana. Here are common operations you can perform on your dojo contracts.

### Initialize Dojo Project
To initialize a dojo project, from the base repository:
```
npm run initialize-dojo --name=<PROJECT_NAME>
```

### Build Dojo Project
To build your dojo project, from the base repository run:
```
npm run build-dojo --name=<PROJECT_NAME>
```

### Deploy Katana
To build deploy katana, from the base repository run:
```
npm run deploy-dojo-katana --name=<PROJECT_NAME>
``` 

### Migrate Dojo Project
To migrate your dojo project, from the base repository run:
```
npm run migrate-dojo --name=<PROJECT_NAME>
```


## User Interface Scripts

The following are scripts from `Starknet-Scaffold` for handling the user interface.

### Run Frontend
To run UI, from the base repository:
```
npm run start
```

### Run Frontend
To build your frontend, from the base repository run:
```
npm run build-ui
```

