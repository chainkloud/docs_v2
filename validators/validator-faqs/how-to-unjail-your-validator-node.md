---
description: When your validator is jailed, follow these instructions
---

# How to Unjail Your Validator Node

## **Prerequisites**

* Make sure your validator node is back to online
* Make sure your validator node is fully synced

## **Instructions**

1. Send an unjail request
2. Send a 0 MIX transaction to the consensus contract **0x1c7DFFd9313A0f3f20518E88735932D02bef4F28** from your validator wallet with the following data: **0x6eae5b11**
3. This will move the node to the pending list and it will be released at the start of the next cycle
