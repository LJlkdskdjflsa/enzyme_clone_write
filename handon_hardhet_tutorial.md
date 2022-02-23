```
npm init
npm install hardhat -D
npx hardhat
npm install -D @nomiclabs/hardhat-ethers ethers @nomiclabs/hardhat-waffle ethereum-waffle chai
```

寫合約

```
npx hardhat compile
```
寫test 
```
npx hardhat test
```
通過後debug合約
用hardhat console在智能合約中加入js的code
再跑一次
```
npx hardhat test
```
會顯示出console.log 的資訊

### Deploy Smart Contract
1. local
2. testnet
3. mainnet

local:
寫script.deploy.js

deploy to kovan
```
npx hardhat run scripts/deploy.js
``` 
->success

deploy to rinkeby
把alchemy資訊加入 config
```
npx hardhat run scripts/deploy.js --network rinkeby
``` 