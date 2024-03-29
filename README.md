[![N|Solid](https://eadn-wc04-4642508.nxedge.io/cdn/wp-content/themes/troontechnologies/assets/img/inner-logo.svg)](https://troontechnologies.com/)

# Blockchain coding assignments

This document will cover four weeks coding assignments, the assignments will focus mainly on Ethereum, solidity, web3 based development. At the end of each assignment, your code will be reviewed by a senior developer. 

> Note: Write your code while using solidity latest version (currently 0.8.9)

## Assignment # 1:
Create a custom erc20 token with the following details:
1. Token name: TroonToken
2. Token symbol: TRN
3. Decimal: 8
4. Max supply: 20 million

The token contract should use the safeMath library for all the arithmetic operations. The contract should be ownable and only the owner can mint new tokens. 

**Helping Material**
| Item | Link |
| ------ | ------ |
| ERC-20 standard official documentation | https://eips.ethereum.org/EIPS/eip-20 |
| Implementation example | https://github.com/OpenZeppelin/openzeppelin-contracts/blob/9b3710465583284b8c4c5d2245749246bb2e0094/contracts/token/ERC20/ERC20.sol |

> Note: Deploy the token contract on Rinkeby testnet and test all methods using Metamask wallet. 


## Assignment # 2:
**Problem Statment:**
Create a smart contract to sell NFTs. The total number of NFTs available will be 100 and each NFT costs 0.5 Ethers. A single user can not buy more than 10 NFTs.  All of the collected ETH tokens should be transferred to the admin wallet. 

**Additional Information**
1. Use ERC721 standard to create NFTs.
2. Use reentrancy guard on the payable functions. 
3. Contract should be ownable.
4. Use random images for NFT.
5. Use ipfs (pinata) for storing NFT metadata.

**Helping Material**
| Item | Link |
| ------ | ------ |
| ERC-721 standard official documentation | https://eips.ethereum.org/EIPS/eip-721 |
| NFT contract example | https://github.com/ProjectOpenSea/opensea-creatures/blob/master/contracts/ERC1155Tradable.sol |
| Metadata standard | https://docs.opensea.io/docs/metadata-standards |

> Note: Deploy the token contract on Rinkeby testnet and test all methods using Metamask wallet. 

## Asignment # 3
**Problem Statment:**
Create a lottery system where users can buy lottery tickets and can win a grand prize. Each lottery ticket costs 0.1 ETH. Once a ticket is bought it is not refundable nor the user can send it to anyone. A total of 100 tickets will be available in each lottery. Users can buy as many tickets as they want. Each lottery ticket will have a ticket id and the winning Id will be decided randomly. The reward for the winner will be 9.0 ETH and 1.0 ETH will go to the admin wallet. Once all the tickets are sold a new lottery will be started with the same reward. 

Create a function through which lottery winners can claim their reward. 

**Addidtional Information**
1. You can use chainlink oracle to generate random number.
2. Use reentrancy guard on the payable functions.
3. Contract should be ownable.

**Helping Material**
| Item | Link |
| ------ | ------ |
| Chain link VRF generator| https://docs.chain.link/docs/chainlink-vrf/#generate-random-numbers-in-your-smart-contracts |

## Asignment # 4
( Assignment 4 is a continuation of assignment 3)

Create a single-page user interface for the lottery system, where users can buy tickets using their Metamask wallet. Users can see how many tickets are left, the price of each ticket, the total prize for the lottery. A claim button for the winners through which they can claim their reward. And a collect funds option for the admin to collect his/her funds. 
You can use any javascript framework (react, angular, vuejs).

**Helping Material**
| Item | Link |
| ------ | ------ |
| Metamask integration tutorial | https://youtu.be/LzdMosLzj80 |
