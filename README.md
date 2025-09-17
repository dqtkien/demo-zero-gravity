# Mainnet0G Foundry Starter

This repository is a minimal Foundry setup pre-configured for the 0G mainnet RPC.

## Install Dependencies

```sh
forge install foundry-rs/forge-std@v1.10.0 \
  OpenZeppelin/openzeppelin-contracts@v4.9.6 \
  OpenZeppelin/openzeppelin-contracts-upgradeable@v4.9.6
```

## Build smart contract

```sh
forge build
```

## Verify contract

```sh
forge verify-contract 0xbCFB30bfD6C7D1eE2388C2E39CA7c917e9eaE11b src/orocle-v2/OrocleV2.sol:OrocleV2 \
  --chain-id 16661 \
  --compiler-version 0.8.19+commit.7dd6d404 \
  --verifier custom \
  --verifier-api-key 123 \
  --verifier-url https://chainscan.0g.ai/open
```
