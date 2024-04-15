
# ERC-4907 Deployment Tutorial

[ERC-4907](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-4907.md) is an extension of [ERC-721](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-721.md). It proposes an additional role (`user`) which can be granted to addresses, and a time where the role is automatically revoked (`expires`). The `user` role represents permission to "use" the NFT, but not the ability to transfer it or set users.

This is the beginner guide to creating and deploying a simple ERC-4907 smart contract using ChainIDE, MetaMask, and Solidity.

If you have any questions, feel free to join [ChainIDE Discord!](https://discord.gg/QpGq4hjWrh)


Following are the steps to deploy an ERC-4907 smart contract:

1. Setting up a Wallet

2. Write down an ERC-4907 smart contract

3. Compile, deploy and Verify

4. List on test.double.one   

### 1. Setting up a Wallet

#### 1.1. Install MetaMask

When we deploy a smart contract to the blockchain or make a transaction to the deployed smart contract,
we need to pay the gas fee, and for that, we need to have a Web3 wallet, which is MetaMask. 
So, first of all, we'll install MetaMask. Please click [here](https://metamask.io/) to install MetaMask.

#### 1.2. Add the Mumbai Test Network to MetaMask
Click on the "Connect wallet" in the upper right corner, select the "Injected Web3 Provider" button, and then select on MetaMask to connect to the MetaMask wallet (Polygon Mainnet is the main network, and Mumbai is the test network - connect to Mumbai).

![image-20230114120433122](https://d3gvnlbntpm4ho.cloudfront.net/ERC721_Deployment_on_Mumbai_Polygon/image-20230114120433122.png)


#### 1.3. Obtaining Testnet Matic
Once Mumbai has been added to MetaMask, navigate to the [Polygon Faucet](https://faucet.polygon.technology/) to receive test tokens. On the faucet page, choose Mumbai as the network, MATIC as the token, and paste your MetaMask wallet address. Then, click submit, and the faucet will send you some test MATIC within a minute.

<img src="https://d3gvnlbntpm4ho.cloudfront.net/ERC+721+Deployment+on++Mumbai/Polygon_PR_get_tokens.png" width="100%" height="100%" />

### 2. Write down an ERC-4907 Smart contract

You need to write down all the required functions that you want to implement in your ERC-4907 smart contract. A general ERC-4907 smart contract has the following functions.

-   `setUser()`: set the user and expires of the NFT

-   `userOf()`: returns the user address of the NFT

-   `userExpires()`: returns the user expires of the NFT


ChainIDE team has prepared the complete ERC-4907 showcase including all the required functions, you may use that built-in template **ERC4907.sol**  and add/delete functions according to your requirements.

### 3. Compile, deploy and verify
These steps are the same as the ERC-721 Showcase.


### 4. List on test.double.one
Auto-Deployment is a powerful tool on Double Protocol that enables NFT Projects or anyone to instantly deploy ‘NFT collections’ on Double Protocol to enable Rental Service for such NFTs.

Click [here](https://docs.double.one/for-developers/integration-tutorials/nft-rental-auto-deployment) for details.
