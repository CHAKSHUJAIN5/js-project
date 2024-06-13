# Creating NFT
In this project we will learn about NFT  and create some (not original)

## Description
The code initializes an empty `NFTs` array to store minted NFTs. The `mintNFT` function creates and adds an NFT object with `name`, `color`, and `rarity` to the array. The `listNFTs` function logs the metadata of all NFTs, and the `getTotalSupply` function logs the total count of minted NFTs.

## Getting Started

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program


1. Initialize NFTs array: An empty array to store minted NFTs.
2. Minting function: Creates and adds an NFT object with name, color, and rarity to the array.
3. Listing function: Logs metadata of all NFTs in the array.
4. Total supply function: Logs the total count of minted NFTs.

```javascript
// create a variable to hold your NFTs
const NFTs = []

// this function will take in some values as parameters, create an
// NFT object using the parameters passed to it for its metadata, 
// and store it in the variable above.
function mintNFT(name, color, rarity) {
    const NFT = {
        "name": name,
        "color": color,
        "rarity": rarity,   
    }
    NFTs.push(NFT);
}

// create a "loop" that will go through an "array" of NFTs
// and print their metadata with console.log()
function listNFTs() {
    for (let i = 0; i < NFTs.length; i++) {
        console.log("\nName:   " + NFTs[i].name);
        console.log("Color:  " + NFTs[i].color);
        console.log("Rarity: " + NFTs[i].rarity);
        console.log("\n");
    }
}

// print the total number of NFTs we have minted to the console
function getTotalSupply() {
    console.log("\nNumber of NFTs minted are: " + NFTs.length);
}

// call your functions below this line
mintNFT("Dragon", "Red", "Epic");
mintNFT("Phoenix", "Orange", "Legendary");
mintNFT("Unicorn", "White", "Rare");
listNFTs();
getTotalSupply();
```

To run the code on Gitpod, start by navigating to [Gitpod](https://gitpod.io/) and signing in with your GitHub account. Create a new workspace by clicking "New Workspace" and entering the URL of your GitHub repository. If you don't have a repository, you can create a new one on GitHub and use its URL. Gitpod will automatically clone the repository for you. Once inside the workspace, create a new file named `nft.js` and paste your code into it. Open the terminal in Gitpod by selecting "Terminal" from the top menu and choosing "New Terminal." Gitpod usually comes with Node.js pre-installed, but if it's not, you can install it by running `sudo apt-get update` followed by `sudo apt-get install -y nodejs npm`. Finally, run your script by executing `node nft.js` in the terminal. This will mint the NFTs, list their metadata, and display the total number of minted NFTs.

## Authors
Chakshu jain

```
