# POLY-PROOF-AdvancedGenerate a 5-item collection using DALLE 2 or Midjourney

## Description
In this project, we will deploy a unique NFT collection on the Ethereum blockchain. To add an exciting twist, we will utilize advanced image generation tools such as DALLE 2 or Midjourney to create the artwork for our NFTs. Once the collection is generated, we will store the NFT images on IPFS using pinata.cloud.

Next, we will map the NFT collection to the Polygon network, which will enable faster and more cost-effective transactions. To achieve this, we will use the token mapper provided by Polygon.

Finally, we will transfer the NFT assets from the Ethereum blockchain to the Polygon network using the FxPortal Bridge. This will ensure that our NFTs can be accessed and traded efficiently on the Polygon network. By following these steps, we will have successfully combined cutting-edge image generation technology with blockchain innovation to create and transfer our unique NFT collection.
Store items on IPFS using pinata.cloud

## Project Aim ::
* Deploy an ERC721 or ERC1155 to the Goerli Ethereum Testnet

+ You should have a promptDescription function on the contract that returns the prompt you used to generate the images

- Map Your NFT Collection using Polygon network token mapper. Note: this isn’t necessary but helpful for visualization.

* Write a hardhat script to batch mint all NFTs. Hint: ERC721A is optimal here.

* Write a hardhat script to batch transfer all NFTs from Ethereum to Polygon Mumbai using the FxPortal Bridge

+ Approve the NFTs to be transferred

- Deposit the NFTs to the Bridge

* Test balanceOf on Mumbai

## Steps ::
Prequisites; 
Generate a collection of 5 unique items using DALLE2, Midjourney, or Gencraft (a free source). Upload the generated images to pinata.cloud and store their URLs.

1. Clone the project repository.

2. For this project, we'll be working with the sepolia testnet and the Mumbai Testnet. To ensure proper execution, acquire test ethers for your Ethereum account from https://sepoliafaucet.com/. Keep the private key associated with the account that has test ethers in your hardhat configuration.

3. Execute the following command to deploy the NFT contract on the sepolia testnet: npx hardhat run scripts/deploy.js --network sepolia. After a successful deployment, copy the deployed contract address and paste it in the batchMint.js and approvedDeposit.js files.

4. Next, run the batch minting script using this command: npx hardhat run scripts/batchMint.js --network sepolia. This will create and mint the NFTs in the sepolia testnet.

5. Now, execute the approved deposit script with the command: npx hardhat run scripts/approvedDeposit.js --network sepolia. This will approve the NFTs to be transferred to the Polygon network.

6. Proceed to transfer the NFT assets from the Ethereum blockchain to the Polygon Mumbai network using the FxPortal Bridge.

7. Finally, test the balanceOf function on the Mumbai network to confirm the successful transfer and receive the output indicating the Mumbai testnet balance for the number of NFTs received from the sepolia testnet.

8. By following these steps, you will have successfully deployed an NFT collection on the Ethereum sepolia testnet, mapped it to the Polygon network, and transferred the NFT assets from Ethereum to Polygon using the FxPortal Bridge.

## Author
Vaishnavi Arora

## License
This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.
