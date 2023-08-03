# POLY-PROOF-AdvancedGenerate a 5-item collection using DALLE 2 or Midjourney

## Description
In this project, we will deploy a unique NFT collection on the Ethereum blockchain. To add an exciting twist, we will utilize advanced image generation tools such as DALLE 2 or Midjourney to create the artwork for our NFTs. Once the collection is generated, we will store the NFT images on IPFS using pinata.cloud.

Next, we will map the NFT collection to the Polygon network, which will enable faster and more cost-effective transactions. To achieve this, we will use the token mapper provided by Polygon.

Finally, we will transfer the NFT assets from the Ethereum blockchain to the Polygon network using the FxPortal Bridge. This will ensure that our NFTs can be accessed and traded efficiently on the Polygon network. By following these steps, we will have successfully combined cutting-edge image generation technology with blockchain innovation to create and transfer our unique NFT collection.
Store items on IPFS using pinata.cloud

## Steps::
* Deploy an ERC721 or ERC1155 to the Goerli Ethereum Testnet

+ You should have a promptDescription function on the contract that returns the prompt you used to generate the images

- Map Your NFT Collection using Polygon network token mapper. Note: this isn’t necessary but helpful for visualization.

* Write a hardhat script to batch mint all NFTs. Hint: ERC721A is optimal here.

* Write a hardhat script to batch transfer all NFTs from Ethereum to Polygon Mumbai using the FxPortal Bridge

+ Approve the NFTs to be transferred

- Deposit the NFTs to the Bridge

* Test balanceOf on Mumbai

## Author
Vaishnavi Arora

## License
This contract is licensed under the MIT License. SPDX-License-Identifier: MIT.
