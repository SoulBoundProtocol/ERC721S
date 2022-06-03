<!-- ABOUT THE PROJECT -->

## About The Project

ERC721S, **S for SoulBound**, is an implementation for SoulBound (non-transferable) NFT coined by Vitalik Buterin in a [blog post](https://vitalik.ca/general/2022/01/26/soulbound.html).

## Features

- Non-transferable: SoulBound
- Community recovery: at extreme condition (lost private key), community multisig (contract owner) can transfer the token to the new wallet under the approvement of the token holder.
- Gas saving: reuse the code in ERC721A
- Sybil identification: each address is associated with an `isSybil` variable for projects to identify Sybil/bot.
- Soul power: each address is associated with an `isSybil` variable, a score that measures the soul power associated with the addresss (e.g. the contribution score to the project).
