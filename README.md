# Custom Token Swap Marketplace (Uniswap Exchange) DApp

Building a Custom Token Swap Marketplace (Uniswap Exchange) using Next.js, Solidity, and React.js Build your Uniswap Token Marketplace start-up, in which you can provide users to Swap any ERC20 token, and allow them to buy tokens.

## Project Overview

![alt text](https://www.daulathussain.com/wp-content/uploads/2023/08/uniswap-token-marketplace.jpg)

## Instruction

Kindly follow the following Instructions to run the project in your system and install the necessary requirements

- [Final Source Code](https://www.theblockchaincoders.com/sourceCode/uniswap-token-marketplace-dapp)

#### Setup Video

- [Final Code Setup video](https://youtu.be/2gqvaEAVCM4?si=b_XykDWVP1hzCBkY)

```
   URL: https://youtu.be/2gqvaEAVCM4?si=b_XykDWVP1hzCBkY
   WATCH: Setup & Demo Of Project
```

#### Install Vs Code Editor

```
  URL: https://code.visualstudio.com/download
  GET: VsCode Editor
```

#### NodeJs & NPM Version

```
  URL: https://nodejs.org/en/download
  NodeJs: v18.12.1
  NPM: 8.19.2
```

#### Clone Starter File

```
  URL:https://github.com/daulathussain/uniswap-tokem-marketplace-starter-file
  GET: Project Starter File Download
```

All you need to follow the complete project and follow the instructions which are explained in the tutorial by Daulat

## Final Code Instruction

If you download the final source code then you can follow the following instructions to run the Dapp successfully

#### Setup Video

```
   URL: https://youtu.be/UHjJwa8TiQs?si=EzdPof1eUA37Nhtt
   WATCH: Setup & Demo Of Project
```

#### Final Source Code

```
   FINAL SOURCE CODE: https://www.theblockchaincoders.com/sourceCode/uniswap-token-marketplace-dapp
   ALL SOURCE CODE: https://www.theblockchaincoders.com/SourceCode
   Download the Final Source Code
```

#### Install Vs Code Editor

```
  URL: https://code.visualstudio.com/download
  GET: VsCode Editor
```

#### NodeJs & NPM Version

```
  URL: https://nodejs.org/en/download
  NodeJs: v18.12.1
  NPM: 8.19.2
```

#### WAGMI WALLET

```
  URL CHAINS: https://wagmi.sh/react/api/chains
  WEBSITE: https://wagmi.sh/
  DOC: https://wagmi.sh/react/getting-started
```

#### Test Faucets

Google will provide you with some free test faucets which you can transfer to your wallet address for deploying the contract

```
  URL: https://cloud.google.com/application/web3/faucet
  Get: Free Test Faucets
```

#### RemixID

We are using RemixID for deploying the contract and generation of the ABI in the project, but you can use any other tools like Hardhat, etc.

```
  URL: https://remix-project.org
  OPEN: RemixID
```

## Important Links

- [Get Pro Blockchain Developer Course](https://www.theblockchaincoders.com/pro-nft-marketplace)
- [Support Creator](https://bit.ly/Support-Creator)
- [All Projects Source Code](https://www.theblockchaincoders.com/SourceCode)

## Authors

- [@theblockchaincoders.com](https://www.theblockchaincoders.com/)
- [@consultancy](https://www.theblockchaincoders.com/consultancy)
- [@youtube](https://www.youtube.com/@daulathussain)

#### ENVIROMENT VARIABLES

```
  NEXT_PUBLIC_MARKETPLACE_ADDRESS = 0xd55fffb30a6af39A6705e52d172eAf77baC73aA2

  # SEPOLIA RPC URL
  NEXT_PUBLIC_SEPOLIA_URL = https://rpc.ankr.com/eth_sepolia

  # HOLESKY RPC URL
  NEXT_PUBLIC_HOLESKY_RPC_URL = https://rpc.ankr.com/eth_holesky
```

#### HOLESKY NETWORK

```
  const { chains, provider } = configureChains(
  [
    {
      id: 17000,
      name: "Holesky",
      network: "holesky",
      nativeCurrency: {
        name: "Holesky Ether",
        symbol: "ETH",
        decimals: 18,
      },
      rpcUrls: {
        default: {
          http: [`${HOLESKY}`],
        },
        public: {
          http: [`${HOLESKY}`],
        },
      },
      blockExplorers: {
        default: {
          name: "Holescan",
          url: "https://holesky.etherscan.io/",
        },
      },
      testnet: true,
    },
  ],
  [
    jsonRpcProvider({
      rpc: (chain) => {
        if (chain.id === 17000) {
          return { http: `${HOLESKY}` };
        }
        return null;
      },
      priority: 1,
    }),
  ]
);
```

#### SEPOLIA NETWORK

```
 const { chains, provider } = configureChains(
  [
    {
      id: 11155111,
      name: "Sepolia",
      network: "sepolia",
      nativeCurrency: {
        name: "Sepolia Ether",
        symbol: "ETH",
        decimals: 18,
      },
      rpcUrls: {
        default: {
          http: [`${SEPOLIA}`],
        },
        public: {
          http: [`${SEPOLIA}`],
        },
      },
      blockExplorers: {
        default: {
          name: "Etherscan",
          url: "https://sepolia.etherscan.io",
        },
      },
      testnet: true,
    },
  ],
  [
    jsonRpcProvider({
      rpc: (chain) => {
        if (chain.id === 11155111) {
          return { http: `${SEPOLIA}` };
        }
        return null;
      },
      priority: 1,
    }),
  ]
);
```
