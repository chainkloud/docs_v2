# Stake, Delegate and Withdraw

The requirement to become a Mix chain validator is having a stake of at least 100,000 MIX tokens.

The stake amount is the sum of the address's staked and delegated Mix tokens. This guide walks through the process of using MEW (MyEtherWallet.com) in the Mix network Roadmap - Those functionalities will be built into our Studio and will not require any technical knowledge in the future.

## Stake <a href="#stake" id="stake"></a>

There are two options to stake (both should be called from the address which would be the validator)

1. 1\. Send Mix tokens to the [consensus contract](https://miexs.com/address/0x1c7DFFd9313A0f3f20518E88735932D02bef4F28) - 0x1c7DFFd9313A0f3f20518E88735932D02bef4F28 on the Mix Network.
2. 2\. Call the \`stake\` function on the [consensus contract](https://miexs.com/address/0x1c7DFFd9313A0f3f20518E88735932D02bef4F28) - 0x1c7DFFd9313A0f3f20518E88735932D02bef4F28 on the Mix Network.

## Delegate <a href="#delegate" id="delegate"></a>

Mix token holders who don't want to run a node alone but still wish to participate in governing the network can delegate any amount to one of the validators. Delegating is done by calling the \`delegate\` function on the [consensus contract](https://miexs.com/address/0x1c7DFFd9313A0f3f20518E88735932D02bef4F28) with the validator address as data (see the screenshot from MEW).

![delegate](https://3886961007-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MQROvzQPC4eD8u5AQhv%2Fuploads%2FfW2bi43f3TMgmwzi7wSZ%2Fimage.png?alt=media\&token=f30eb8a1-ff40-4f1e-9f73-89466ea2c83e)

## Withdraw <a href="#withdraw" id="withdraw"></a>

Both stakers and validators can withdraw their Mix tokens, up to the staked/delegated amount, at any time. The withdrawn amount will be deducted from the validator stake amount. If the stake amount falls below the minimum, the validator will be removed from the Mix chain validators list. There are two options to withdraw:

1. 1\. Call the \`withdraw\` function on the [consensus contract](https://miexs.com/address/0x1c7DFFd9313A0f3f20518E88735932D02bef4F28) with one parameter - the amount to withdraw. This call is for stakers and will reduce the stake amount of the sender address.
2. 2\. Call the \`withdraw\` function on the [consensus contract](https://miexs.com/address/0x1c7DFFd9313A0f3f20518E88735932D02bef4F28) with two parameters - validator address and amount to withdraw. This call is for both stakers (who can use their address as the parameter) and for delegators to withdraw their delegated stake on a specific validator.

![withdraw option no. 1](https://3886961007-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MQROvzQPC4eD8u5AQhv%2Fuploads%2FyBpFV4W9N9vgpGyFEr76%2Fimage.png?alt=media\&token=0f715110-4b8d-4a35-81a6-93383d903f42)

![withdraw option no. 2](https://3886961007-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F-MQROvzQPC4eD8u5AQhv%2Fuploads%2FTGmteQzEhEXuDVbibfVt%2Fimage.png?alt=media\&token=84a4f2a6-3c5e-41d7-b427-a845db9f82d2)
