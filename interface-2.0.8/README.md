# Dreamswap Frontend

[![Tests](https://github.com/Dreamswap/uniswap-frontend/workflows/Tests/badge.svg)](https://github.com/Dreamswap/uniswap-frontend/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for Dreamswap -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [uniswap.org](https://uniswap.org/)
- Docs: [uniswap.org/docs/](https://uniswap.org/docs/)
- Twitter: [@DreamswapProtocol](https://twitter.com/DreamswapProtocol)
- Reddit: [/r/Dreamswap](https://www.reddit.com/r/Dreamswap/)
- Email: [contact@uniswap.org](mailto:contact@uniswap.org)
- Discord: [Dreamswap](https://discord.gg/Y7TF6QA)
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Accessing the frontend

To access the front end, use an IPFS gateway link from the
[latest release](https://github.com/Dreamswap/uniswap-frontend/releases/latest)
or visit [uniswap.exchange](https://uniswap.exchange).

## Development

### Install Dependencies

```bash
yarn
```

### Configure Environment (optional)

Copy `.env` to `.env.local` and change the appropriate variables.

### Run

```bash
yarn start
```

To have the frontend default to a different network, make a copy of `.env` named `.env.local`, 
change `REACT_APP_NETWORK_ID` to `"{yourNetworkId}"`, and change `REACT_APP_NETWORK_URL` to e.g. 
`"https://{yourNetwork}.infura.io/v3/{yourKey}"`. 

Note that the front end only works properly on testnets where both 
[Dreamswap V2](https://uniswap.org/docs/v2/smart-contracts/factory/) and 
[eth-scan](https://github.com/MyCryptoHQ/eth-scan) are deployed.
The frontend will not work on other networks.

## Contributions

**Please open all pull requests against the `v2` branch.** 
CI checks will run against all PRs. 
