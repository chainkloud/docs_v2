# Getting started as a validator on Mix Mainnet

## Pre-requirements

To be a Mix validator, you first must see that you meet the pre-requirements:

* You know what it means to be a Mix validator - How to become a validator
* You have at least 100K MIX tokens, or you will have an aggregated delegation of at least 100K MIX tokens.

## How to become a Mix validator

To quickly become a validator, follow this steps:

Read more at: [https://github.com/chainkloud/CoinNetwork/tree/master/node-example](https://github.com/chainkloud/CoinNetwork/tree/master/node-example)

#### Stake

To stake MIX tokens, all you should do is send your MIX tokens to the Mix Consensus contract address over the Mix network from the validator address.

{% hint style="success" %}
The Mix Consensus contract address: `0x1c7DFFd9313A0f3f20518E88735932D02bef4F28`
{% endhint %}

The easiest way is to import your private key or key-store file to your favorite wallet (for example, Metamask), switch the network to Mix, and send the MIX tokens (native tokens) to the Consensus contract address.

{% hint style="info" %}
You can find your key-store (containing your private key) and the password for the created account in:

`$HOME/nodes/keys/MIX/UTC--xxxx`

`$HOME/nodes/node.pwd`
{% endhint %}

#### Delegate

To delegate, send the MIX tokens from any address to the Consensus contract address with the data: `0x5c19a95c000000000000000000000000<address without 0x>`.

{% hint style="success" %}
Example:

For the address: `0xb8ce4a040e8aa33bbe2de62e92851b7d7afd52de`\
Use: `0x5c19a95c000000000000000000000000b8ce4a040e8aa33bbe2de62e92851b7d7afd52de` as the data.

`5c19a95c` is for the `delegate(address)` function signature.

`b8ce4a040e8aa33bbe2de62e92851b7d7afd52de`in this example, is an address you're delegating to (without the `0x` prefix)
{% endhint %}

### Step 6: Wait for one cycle (approximately 48 hours).

Wait until the next cycle is started.

{% hint style="success" %}
You can see that you are validating both in the [status](https://status.miexs.com/) and explorer sites.
{% endhint %}

For live support, contact us on [Telegram](https://t.me/) or [Discord](https://discord.gg). Good luck, and happy validating!
