# Pegasys Token Asset Registry

This repository is a comprehensive collection of token assets for pooled tokens on the Pegasys DEX.

Such a collection can be maintained only through a community effort, so _feel free to add your token!_

This repo is intended to be similar to Trust Wallet's asset repository. Token logos are stored according to their Syscoin address under the `tokens` directory. Logos are stored in the format `<token-address>/logo.png`.

Mainnet and testnet token registries are handled independently.

Please make sure to follow the guidelines as this speeds up our review process 😉

## Guidelines
To integrate your token into the Pegasys app you must submit a PR following these steps:
- [ ] Make sure to let us know of your interest through our [Discord channel](https://discord.gg/kAq3pAUAkE) by reaching out to anyone from our team over at the `Support -> 🌱│new-tokens` channel.
- [ ] Fork the Github repository, preferably to your team's Github organization.
- [ ] Create a new folder with the [_checksum formatted_](https://piyolab.github.io/sushiether/RunScrapboxCode/?web3=1.0.0-beta.33&code=https://scrapbox.io/api/code/sushiether/web3.js_-_Ethereum_のアドレスをチェックサム付きアドレスに変換する/demo.js) smart contract address of your token(mixed case `0xa5B6...` address).
- [ ] Tell your designer that token image must be in PNG format, preferably transparent background, recommended size 256x256px, with max file size of 100kB.
- [ ] Upload your logo with file named `logo.png` to previously created folder, i.e. `tokens/0x000000000000000000000000000000000000dEaD/logo.png`
- [ ] Create a `info.json` file with info about the token/project containing:
```json
{
    "name": "Token Name",
    "type": "ERC20", // Token type/extensions according to https://eips.ethereum.org/ | https://openzeppelin.com/contracts/
    "symbol": "TOKEN",
    "decimals": 18,
    "website": "https://token.finance",
    "description": "One-sentence summary of your project",
    "explorer": "https://syscan.io/token/0x000000000000000000000000000000000000dEaD",
    "status": "active",
    "id": "0x000000000000000000000000000000000000dEaD",
    "links": [
        {
            "name": "twitter",
            "url": "https://twitter.com/TokenName"
        },
        {
            "name": "telegram",
            "url": "https://t.me/joinchat/TokenLink"
        },
        {
            "name": "coingecko",
            "url": "https://coingecko.com/en/coins/token-name/"
        }
    ]
}
```
- [ ] Create a pull request to the main repo, preferably copying over the contents of `info.json` to the PR description

## Disclaimer
Pegasys team allows anyone to submit new assets to this repository. However, this does not mean that we are in direct partnership with all of the projects.

The Pegasys team will reject projects that are deemed as scam or fraudulent after careful review. We also reserve the right to change the terms of asset submissions at any time due to changing market conditions, risk of fraud, or any other factors we deem relevant. We hold no responsibility to add your token under any circumstances.

