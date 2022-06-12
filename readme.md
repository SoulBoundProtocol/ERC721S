<!-- ABOUT THE PROJECT -->

## About The Project

ERC721S (**SoulBound**), is a standard for SoulBound Token (non-transferable NFT) coined by Vitalik Buterin in a [blog post](https://vitalik.ca/general/2022/01/26/soulbound.html).

<!-- FEATURES -->

## Features

- **Non-transferable**: SoulBound
- **Community Recovery**: at extreme condition (losing private key), community multisig (contract owner) can transfer the token to the new wallet under the approvement of the token holder.
- **Gas Saving**: learn from ERC721A
- **Sybil Identification** :each address is associated with an `isSybil` variable for projects to identify Sybil/bot.
- **Soul Power**: each address is associated with an `soulPower` variable, a score that measures the soul power associated with the addresss (e.g. the contribution score to the project).


<!-- USAGE -->

## Usage

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.4;

import "https://github.com/SoulBoundProtocol/ERC721S/contracts/ERC721S.sol";

contract SBT is ERC721S {
    constructor() ERC721S("SBT", "SBT") {}

    function mint() external payable {
        // `_mint`'s second argument now takes in a `quantity`, not a `tokenId`.
        _mint(msg.sender, 1);
    }
}
```
