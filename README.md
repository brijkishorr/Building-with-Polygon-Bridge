# Building-with-Polygon-Bridge

This project showcases the creation and deployment of an NFT collection using a variety of tools and platforms. The project includes generating images with AI, storing them on IPFS, deploying an ERC721 or ERC1155 smart contract, and transferring the NFTs between Ethereum and Polygon networks.

## Tools Used

- **Hardhat**: A development environment for Ethereum software.
- **Foundry (optionally)**: A blazing fast, portable, and modular toolkit for Ethereum application development written in Rust.

## Project Rubric

To successfully complete the Final Challenge, your project should meet the following criteria:

1. **Generate a 5-item collection using DALLE 2 or Midjourney**: Use one of these AI tools to create a set of five unique images for your NFT collection.
   
2. **Store items on IPFS using pinata.cloud**: Upload the generated images to IPFS (InterPlanetary File System) using the Pinata service for decentralized storage.
   
3. **Deploy an ERC721 or ERC1155 to the sepolia Ethereum Testnet**: Choose and deploy either an ERC721 or ERC1155 smart contract to the sepolia Testnet, which will represent your NFT collection.
   
4. **Prompt Description Function**: Implement a function called `promptDescription` in your smart contract that returns the prompt used to generate the images.
   
5. **Map Your NFT Collection using Polygon network token mapper** (optional but recommended): Use the Polygon network token mapper for better visualization of your NFT collection on the Polygon network.
   
6. **Write a Hardhat Script to Batch Mint All NFTs**: Create a script using Hardhat to batch mint all the NFTs in your collection. Using the `ERC721A` standard is optimal for this purpose.
   
7. **Write a Hardhat Script to Batch Transfer All NFTs from Ethereum to Polygon amoy using the FxPortal Bridge**: Develop a script to transfer all minted NFTs from the Ethereum network to the Polygon amoy testnet using the FxPortal Bridge.

## Getting Started

### Prerequisites

- Node.js and npm installed
- Hardhat installed
- Pinata.cloud account
- sepolia Testnet faucet for test Ether
- Polygon amoy Testnet faucet for test MATIC

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/nft-collection-project.git
   cd nft-collection-project
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

### Usage

1. **Generate Images**: Use DALLE 2 or Midjourney to create your 5-item NFT collection. Save the images locally.

2. **Upload to IPFS**: Use Pinata to upload your images to IPFS. Note the IPFS hash for each image.

3. **Deploy Smart Contract**:
   - Compile the contract:
     ```sh
     npx hardhat compile
     ```
   - Deploy the contract to sepolia Testnet:
     ```sh
     npx hardhat run scripts/deploy.js --network sepolia
     ```

4. **Mint NFTs**: Use the batch minting script to mint your NFTs.
   ```sh
   npx hardhat run scripts/batchMint.js --network sepolia
   ```

5. **Transfer to Polygon**: Transfer your NFTs to Polygon amoy using the batch transfer script.
   ```sh
   npx hardhat run scripts/batchTransfer.js --network amoy
   ```

## Scripts

- `scripts/deploy.js`: Script to deploy the smart contract.
- `scripts/batchMint.js`: Script to batch mint NFTs.
- `scripts/batchTransfer.js`: Script to batch transfer NFTs from Ethereum to Polygon.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.

---

By following this guide, you will be able to create, deploy, and transfer your NFT collection across different networks. Enjoy building your project!
