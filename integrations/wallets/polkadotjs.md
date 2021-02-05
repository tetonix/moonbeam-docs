---
title: Polkadot JS Apps
description: Follow this quick tutorial to learn how to use Moonbeam’s Ethereum-standard H160 addresses with Substrate-based apps like Polkadot JS.
---
# Polkadot JS Apps

![Intro diagram](/images/polkadotjs/polkadotjs-banner.png)

## Introduction
With the [release of the v3 upgrade](https://www.purestake.com/news/moonbeam-network-upgrades-account-structure-to-match-ethereum/) for the Moonbase Alpha TestNet, we have made significant updates to the underlying account system on Moonbeam, replacing the default Substrate-style accounts and keys with Ethereum-style accounts and keys.

The Polkadot JS Apps interface was updated as well so that it natively supports H160 addresses and ECDSA keys. So, in this tutorial lets check this new integration of Ethereum-based accounts on the Polkadot JS Apps site.

## Connecting to Moonbase Alpha
First, we need to connect it to the Moonbase Alpha TestNet by clicking the top left corner logo and selecting Moonbase Alpha under Test Networks.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app1.png)

After switching, the Polkadot JS site will not only connect to Moonbase Alpha, but it will also change its styling, to make a perfect match.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app2.png)

## Importing an H160 Account
Let's see how we can import an already existing MetaMask account to Polkadot JS Apps. First, navigate to the accounts section, and click in the add account button.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app3.png)

This will open a wizard pop-up that will guide you through the process of adding an account to the Polkadot JS Apps interface. Make sure you click on the drop-down menu and change from Mnemonic to Raw seed, this allows you to add an account through a private key. 

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app4.png)

Next, enter your private key that you can export from MetaMask, in this case we are importing the following account:

- Private key: `28194e8ddb4a2f2b110ee69eaba1ee1f35e88da2222b5a7d6e3afa14cf7a3347`
- Public address: `0x44236223aB4291b93EEd10E4B511B37a398DEE55` 

Make sure to include the prefix in the private key, that is `0x`. If you entered the information correctly, the corresponding public address should appear in the upper left corner of the window.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app5.png)

Click next and finish the wizard by setting an account name and password. After a confirmation message, you should see in the main Accounts tab the address with the corresponding balance, in our case Bob's. Moreover, we can overlay the MetaMask extension to see that both balances are the same.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app6.png)

## Sending a Transaction Through Substrate's API
Now, let's demonstrate the potential of Moonbeam's Unified Accounts scheme by making a transfer through the Substrate API using the Polkadot JS Apps. Remember that we are talking about interacting with Substrate using an Ethereum-style H160 address. To do so, we've imported another account, named Charley with 5 `DEV` tokens.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app7.png)

Next, let's click on Bob's send button, which opens another wizard that guides you through the process of sending a transaction. Set the send to address and the amount, which for our example is 5 DEV tokens. When ready click on the Make Transfer button.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app8.png)

After the transaction is signed using the password, Polkadot JS will display some messages on the top right corner while it's being processed. Once confirmed, you should see the balances updated for each account.

![Connect to Moonbase Alpha](/images/polkadotjs/polkadotjs-app8.png)

And that is it! We are super excited about being able to support H160 accounts in Polkadot JS Apps, as we believe this will greatly enhance the user experience in the Moonbeam Network and its Ethereum compatibility features.

## We Want to Hear From You
If you have any feedback regarding the Polkadot JS Apps, the Unified Accounts integration, or any other Moonbeam related topic, feel free to reach out through our official development [Discord server](https://discord.gg/PfpUATX).
