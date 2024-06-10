# EVM Facuet dApp

This is a showcase project that combines a facuet contract and corresponding UI that can be launched on any EVM chain through [Drew Package Manager](https://www.npmjs.com/package/@drewpackages/cli). The setup creates a new ERC-20 token with the name of your choosing and creates a faucet UI that helps anyone mint the token they might need for testing purposes

To launch a new dApp instance (including new contracts deployment) it:
```shell
npm i -g @drewpackages/cli
drew deploy drinkius/faucet  --params "{\"name\": \"Test Token\", \"symbol\": \"TT\", \"totalSupply\": 100000000000000 }"
```

## Development
```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.ts
```