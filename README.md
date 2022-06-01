# Development env

- OS : `Windows 10`
- Node.js : `v16.13.1`
- Typescript : `^4.7.2`
- hardhat : `^2.9.7`
- solidity : `^0.8.0`

# :wrench: Installation

```shell
npm install
```

# :computer: Execution

```shell
# Run scripts with listening file change mode
npm run scripts <path>
# Run hardhat test
npm run test:local
npm run test:matic
# Test with coverage
npm run coverage:local
npm run coverage:matic
```

# Polygonscan verification

```shell
npx hardhat run --network matic scripts/deploy.ts
```

Copy the deployment address and paste it in to replace `DEPLOYED_CONTRACT_ADDRESS` in this command:

```shell
npx hardhat verify --network matic DEPLOYED_CONTRACT_ADDRESS "Hello, Hardhat!"
```
