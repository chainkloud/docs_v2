---
description: >-
  Build of The Graph, we expose a GraphQL API to access the data on the Mix
  Network
---

# The Graph Hosted Service

## Deploying your own subgraph

The Graph is an indexing protocol for querying networks like Ethereum and IPFS. Anyone can build and publish open APIs, called subgraphs, making data easily accessible. The Graph is available on the Mix Network via the [Hosted Service ](https://thegraph.com/hosted-service)solution.

## To get Started

* [Get Started](https://thegraph.com/docs/en/) Guide
* [About The Graph](https://thegraph.com/docs/en/about/)
* What is [Hosted Service](https://thegraph.com/docs/en/deploying/hosted-service/)

## FAQ

* Is Hosted Service going to be sunset soon? - The [message](https://thegraph.com/docs/en/deploying/hosted-service/) refers to the Ethereum network solely. The Graph team [assured](https://thegraph.com/blog/sunsetting-hosted-service/) that:

> Note (added 8.9.2022): The end of Q1 2023 reflects the sunsetting timeline only for The Graph Network-supported chains. As non-mainnet chains become supported on The Graph Network, their hosted service equivalents will sunset gradually to ensure developers have time to migrate subgraphs to the decentralized network. Stay up to date on which chains are supported by The Graph Network here.

:point\_up: Meaning that the Mix Network is going to be supported either via the Hosted Service or with the decentralized protocol

## Integration Guide

* in `subgraph.yaml` put `fuse` as the network name
