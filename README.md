# Basic Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, a sample script that deploys that contract, and an example of a task implementation, which simply lists the available accounts.

```
/contracts: it has all the solidity contracts
/scripts: contains the deploying script
/test:  contains the test-script
```
# Creating a Hardhat Project
Run the below commands
```shell
mkdir my-wave-portal
cd my-wave-portal
npm init -y
npm install --save-dev hardhat
```
Choose the option to create a sample project. Say yes to everything.

```shell
npx hardhat accounts #will list out all the accounts
```

# Compile the project
Run the below commands
```shell
npx hardhat compile
npx hardhat test
```

# Output
<img src="https://i.imgur.com/gn8Qqbf.png">

# Run the contract with the scripts in /scripts
Run the below commands
```shell
npx hardhat run scripts/run.js
```

# Output
<img src="https://i.imgur.com/gZgLmdF.png">

# Deploy the contract locally
Note: hardhat always creates a new ethereum blockchain and destroys it once the script is complete and it does this for every contracs. Its good as its like refereshing the server which helps in debugging the errors fast

Head to your terminal and create a new window. In this window, cd back to your my-wave-portal project. Then, in here go ahead and run
```shell
npx hardhat node
```

Open another terminal and run
```shell
npx hardhat run scripts/deploy.js --network localhost
```

# Output
Check the terminal
<img src="https://i.imgur.com/INuFQgX.png">

Check the first terminal where we created the local blockchain
<img src="https://i.imgur.com/zyyLsNH.png">

# What's Next?
We will be using ReactJs to deploy it for the users to use