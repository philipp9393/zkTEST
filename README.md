
* official guides ZkSync era : https://era.zksync.io/docs/dev/building-on-zksync/hello-world.html and https://era.zksync.io/docs/api/hardhat/getting-started.html#learn-more
* Goerli faucet: https://goerlifaucet.com/ ;
* ZkSync PRC: https://era.zksync.io/docs/dev/troubleshooting/important-links.html ;
* bridge to/from zksync era : https://portal.zksync.io/bridge ;
* explorer : https://goerli.explorer.zksync.io/ ;

# wat do :
1) download Visual Studio Code : https://code.visualstudio.com/ 
2) add extensions to VSC ( Solidity, npm Intellisense ), if Visual Studio Code spits out errors and offers to downloaded needed extensions in a pop up window - accept it and download. could be things like ( yarn, node.js etc. ) install mually ( there are a bunch of guides on how to do it available on the world wide web )
3) add link to this repo to Visual Studio Code : https://github.com/philipp9393/zkTEST
4) prepare betamask : add ZkSync Era Testnet via https://chainlist.org/?testnets=true&search=zksync+era+testnet or manually
5) request Goerli eth: https://goerlifaucet.com/
6) bridge Goerli ETH to ZkSync Era Testnet via https://portal.zksync.io/bridge (make sure it says ZkSync Era Goerli in the bottom right corner)
7) go back to Visual Studio Code terminal and type this command :  ```yarn init -y``` or ```npm init -y``` 
8) then type this : ```sudo npm i -D typescript ts-node ethers@^5.7.2 zksync-web3@^0.13.1 hardhat @matterlabs/hardhat-zksync-solc @matterlabs/hardhat-zksync-deploy```
9) then this : ```yarn hardhat compile```        or     ```npx hardhat compile```
10) add you betamask private key to ```deploy.ts``` 
11) and finally type : ```yarn hardhat deploy-zksync``` or ```npx hardhat deploy-zksync```then wait for the contract to be deployed
12) verify your contract on explorer
13) interact with your smart contract
