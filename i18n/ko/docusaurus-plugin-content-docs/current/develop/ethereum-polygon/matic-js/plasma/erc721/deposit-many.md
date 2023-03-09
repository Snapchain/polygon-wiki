---
id: deposit-many
title: deplasmaitMany
keywords:
- 'plasma client, erc721, deplasmaitMany, polygon, sdk'
description: '이더리움에서 Polygon 체인으로 복수의 토큰을 입금합니다.'
---

`deplasmaitMany` 메서드를 사용해 이더리움에서 Polygon 체인으로 복수의 토큰을 입금할 수 있습니다.

```
const erc721RootToken = plasmaClient.erc721(<root token address>, true);

const result = await erc721RootToken.deplasmaitMany([<token id1>,<token id2>], <user address>);

const txHash = await result.getTransactionHash();

const txReceipt = await result.getReceipt();

```