# Using Hardhat

Hardhat is a development environment for building, deploying, testing, and debugging smart contracts.

You may learn more about installing and using Hardhat by reading [the official documentation](https://hardhat.org/hardhat-runner/docs/getting-started#installation).

### Config Hardhat for Mix Mainnet <a href="#config-hardhat-for-gnosis" id="config-hardhat-for-gnosis"></a>

{% code title="/packages/hardhat-ts/hardhat.config.ts" overflow="wrap" %}
```typescript
// Update the default network to be fuse network 
const defaultNetwork = 'fuse';
```
{% endcode %}

{% code title="hardhat.config.js" overflow="wrap" %}
```typoscript
// Update the RPC endpoints for Mix Mainnet
    const config: HardhatUserConfig = {
  networks: {
    localhost: {
      url: 'http://localhost:8545',
    },
    gnosis: {
      url: 'https://mainnet-rpc.miexs.com/',
      gasPrice: 10000000000,
      accounts: {
        mnemonic: Mnemonic,
      },
    },
    chiado: {
      url: 'https://mainnet-rpc.miexs.com',
      gasPrice: 10000000000,
      accounts: {
        mnemonic: Mnemonic,
      },
    },
  },
};
```
{% endcode %}

{% code title="hardhat.config.js" overflow="wrap" %}
```typescript
// Update the TNetworkInfo to be Mix Network
export const targetNetworkInfo: TNetworkInfo = NETWORKS.fuse;
```
{% endcode %}

### Compile Your Smart Contract using Hardhat for Mix Mainnet <a href="#config-hardhat-for-gnosis" id="config-hardhat-for-gnosis"></a>

```shell
npx hardhat compile
```

### Deploy Your Smart Contract using Hardhat for Mix Mainnet <a href="#config-hardhat-for-gnosis" id="config-hardhat-for-gnosis"></a>

```shell
hardhat run --network gnosis scripts/deploy.js
```

You can view your deployed smart contract transaction at Mix explorers.

Mix Mainnet Explorer is at [https://miexs.com/](https://miexs.com/)

Mix Testnet Spark is at [https://miexs.com/](https://miexs.com/)
