# BySwap

This repo contains the contracts for BySwap protocol, an AMM inspired by Solidly.

## Testing

This repo uses both Foundry (for Solidity testing) and Hardhat (for deployment).

Foundry Setup

```ml
forge init
forge build
forge test
```

Hardhat Setup

```ml
npm i
npx hardhat compile
```

## Deployment

This project's deployment process uses [Hardhat tasks](https://hardhat.org/guides/create-task.html). The scripts are found in `tasks/`.

Deployment contains 3 steps:

1. `npx hardhat deploy:op` which deploys the core contracts, along with RedemptionReceiver, to Optimism.

2. `npx hardhat deploy:ftm` which deploys the RedemptionSender contract to Fantom. The RedemptionReceiver address from Step 1 should be recorded in `deployed.ts` prior.

## Security

WIP

## Contracts

WIP
