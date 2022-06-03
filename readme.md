<!-- ABOUT THE PROJECT -->

## About The Project

ERC721S, or ERC721 SoulBound, is an implementation for SoulBound Token (SBT) coined by Vitalik Buterin in a [blog post](https://vitalik.ca/general/2022/01/26/soulbound.html).

### Features

- Non-transferable: SoulBound Token is not transferrable.
- Community recovery: during emergency conditions (i.e. lost private key), the ERC721S token owner can approve his token to community multisig address and apply to transfer to a new wallet.
- Gas saving: we take advantage of ERC721A standard for gas optimization.
