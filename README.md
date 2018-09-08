# Token Subscriptions

Publishers (service providers) deploy a smart contract on Ethereum with parameters for a subscription including destination address, token address, token amount, and period of recurrence. The publisher then supplies a link to the subscriber that is presented with the terms of the subscription to sign an off-chain meta transaction that is replayed on the defined period. The subscriber controls the flow of the tokens (starting, stopping, pausing, etc) using the ERC20 standard approve() function.

Created for the [#wyominghackathon](https://wyominghackathon.devpost.com/).

Usually a nonce is used for replay protection, but the heart of the trick with tokensubscriptions.com is a replay-able nonce that works on a defined schedule. In combination with the ERC20 allowances and meta transactions an extremely simple token subscription service can be created.

Start accepting token subscriptions now! 