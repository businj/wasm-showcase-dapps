# Astar WASM showcase dApps
This repository contains examples of ink! contracts and their respective UIs that can be deployed on Atar netwroks.
If you are looking for unaudited production ready dApps (ink! + UI) this repo is for you.

#### Contribute to this repository
contributions are welcome:
- If you find an issue or a refactor idea please open an issue
- If you want to add your own example open a Pull Request

## dApps
#### Uniswap-V2 - DEX
This folder contains the line by line implementation of [uniswap-v2 core](https://github.com/Uniswap/v2-core) + [uniswap-v2 periphery](https://github.com/Uniswap/v2-periphery) & its tests. It uses [ink! 3.3.0](https://github.com/paritytech/ink/tree/v3.3.0) & [Openbrush 2.2.0](https://github.com/Supercolony-net/openbrush-contracts/tree/v2.2.0)
The UI template is in active development and will be public in January 23

### Farming
A farming dApp line by line implementation of [ArthSwap master chef](https://github.com/ArthSwap/ArthSwap-MasterChef) adapted from 
[sushiswap](https://github.com/sushiswap/sushiswap/blob/archieve/canary/contracts/MasterChefV2.sol) 

### Fliper + UI 
This is an hello world! example with a basic flipper contract and an UI to interact with it.
The UI is a react app and uses polkadotjs to interact with the node

#### DAO
On Chain governance based on [Governor](https://github.com/OpenZeppelin/openzeppelin-contracts/tree/master/contracts/governance) contracts of OpenZeppelin

#### Tests
The test folder contains integration tests for the contracts.

**Runs the tests**
1. Run a local node \
   Last version of polkadot *v0.9.29* introduced WeightV2 and is not compatible with redspot \
   Please use [swanky-node v0.11](https://github.com/AstarNetwork/swanky-node/releases/tag/v0.11.0) 
2. The end-to-end test uses redspot as testing environment. Node version should be 14
```bash
yarn install
npx redspot test
```
