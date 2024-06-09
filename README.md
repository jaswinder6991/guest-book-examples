# Guest Book Example via Relayer📖

This repo is an example based off the basic Guest Book Example but with a relayer twist.

[![](https://img.shields.io/badge/⋈%20Examples-Basics-green)](https://docs.near.org/tutorials/welcome)
[![](https://img.shields.io/badge/Contract-JS-yellow)](contract-ts)
[![](https://img.shields.io/badge/Contract-Rust-red)](contract-rs)
[![](https://img.shields.io/badge/Frontend-Next.js-blue)](frontend)

This repository contains example implementations of a Guest Book smart contract in both JavaScript and Rust, and an examples of a frontend interacting with a deployed Guest Book contract

## Important Notes
1. This repo uses a forked version of [wallet-selector](https://github.com/jaswinder6991/wallet-selector) which introduces signDelegateAction as a part of the wallet interface.
This is an attempt to make contributions to the wallet selector for enhanced functionality.

2. DON'T USE THIS FOR MAINNET
This repo uses a near private key in the frontend. You should use next js server to create an api end point /relay which uses near private key. Hence your private key won't be exposes in the browser.

## Pending steps
1. In the current forked wallet selector, even delegateActions with deposit gets signed with the function call. There should be a redirect to wallet page to sign delegateAction with deposit with a full access key instead.

Hence currently, if you attach a deposit, you get this error.
```
Error: {"index":0,"kind":{"index":0,"kind":{"DelegateActionAccessKeyError":"DepositWithFunctionCall”}}}
```

## Repositories

- [Guest Book TS Example](contract-ts)
- [Guest Book RS Example](contract-rs)
- [Guest Book Frontend Example](Frontend)

<br />

# What These Examples Show

1. How to store values for different users and handle Token transfers
2. How to interact with a smart contract on NEAR from a frontend

<br />

# Learn More
1. Learn more about the contract through its [README](./contract-ts/README.md).
2. Check [**our documentation**](https://docs.near.org/build/welcome).
