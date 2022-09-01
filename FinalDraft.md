## What is EPNS

Ethereum Push Notification Service (EPNS) is the world’s first decentralized communication & notification protocol for Web3.

Using the protocol, any smart contract, dApp, or backend service can send on-chain or off-chain notifications tied to the wallet addresses of users in a gasless, multichain, open, and platform-agnostic way.

Being an open communication middleware, notifications can be integrated and shown on any crypto wallet, mobile app, browser extension, or dApps enabling a native communication layer for Web3.0


## Questions
1. What layer of web3 is EPNS?
    * Communication [✅]
    * Computation
    * Storage
    * Data relay

2. Does sending notification always require gas fees?
    * Yes, Always
    * No, (only for on-chain notifications) [✅]

3. What problem does EPNS aim to solve?
    * Enable communication between Web3 users
    * Protect users from spam and irregular communication and uphold user privacy
    * Enable web3 and web3 users to interact using their wallet addresses in a decentralized fashion
    * All of the above [✅]

---

# What are Channels?
Any user who activates themselves as a service on the protocol to send notifications for its users can be considered a Channel.

In other words, any service, i.e., a dapp, protocol, or even a web2 service, that wants to send notifications out to its web3 users can choose to become a channel and establish an adequate communication bridge with its users.

The creation of a channel is just a one-time simple procedure. It must be noted that channel creation only happens on the Ethereum blockchain and one wallet address can only create one channel only the protocol.

> ***Note: Although channel creation only happens on the Ethereum blockchain, the protocol is designed to be chain-agnostic, i.e., channel owners can choose to send notification on any chain of their choice and not just Ethereum network***

A successfully created channel can send notifications to its subscribers, directly tied to their wallet addresses.

Once any user opts in and becomes a subscriber for a channel, he/she shall receive notifications from that channel directly in their inbox.
Users who are not a subscriber of a particular channel, receive notifications from that channel in their spam box.

> ***Opting In or Opting out of a Channel is a completely gasless transaction and requires no fees.***

## What is Channel Alias?
In order to enable your channel to be blockchain-agnostic and allow multi-chain communication, we have introduced a new term called Channel Alias. This property is what enables your channel to send notifications on any other blockchain.

In simpler terms, a channel alias address is a native representation of your Ethereum channel on any other EVM or Non-EVM chain through which you wish to communicate with your subscribers.

This means that although channel creation must happen on the Ethereum blockchain itself, notifications or communications can be carried out on any other chain through the same channel if the channel has its alias address adequately configured for that particular chain.

You can communicate with your subscribers on Polygon, BSC, Solana, etc. using an Alias address that is compatible with that respective blockchain.

## How to set up Channel Alias?
Now that we understand channel alias, it's time to understand how one set up their channel alias address for any other chain.

In order to set-up channel alias address for any preferred chain, one has to go through 2 simple steps:
* Selecting the chain and providing the right alias address for the channel during channel creation itself.
* Verification of the alias Address on the selected chain.

## Questions
1. On which chain, does the channel creation happen?
    * Polygon
    * Ethereum [✅]
    * None of the above.

2. Can you send notifications only on Ethereum blockchain?
    * Yes, it’s restricted to the Ethereum blockchain only.
    * No, EPNS notifications are chain-agnostic and not tied only to Ethereum chain. [✅]

2. What happens if the user receives notifications from an unsubscribed channel?
    *  The User will not get that Notification.
    *  The User will receive the notification in his/her inbox.
    *  The Notification will go to the User's Spam Box. [✅]
---

# Notifications

Any successfully created channel, in its active state,  can send notifications to its subscribers about a wide range of things related to defi, governance proposals, web3 news, or any other crucial updates about their protocol/services.

Notifications land in the inbox of those users who are subscribed to the channel. Non-subscribers of a particular channel aren't alerted about notifications from that channel as they land in their spam box.

### Types of Notifications
1. **Broadcast Notifications**: This type of notification is basically broadcasted or sent to all the subscribers of a channel at once.

2. **Targeted Notifications**: As the name suggests, this type of notification allows channel owners to notify a specific wallet address.

3. **Subset Notifications**: Subset notifications are quite helpful when a particular group of subscribers of a channel is supposed to be notified.

## What are Delegated Notifications?

Delegated notifications is a feature that allows channel owners to delegate their power of sending notifications to any other wallet address or multiple wallets of their choice.

Once approved by the channel owner, a wallet address can send notifications on behalf of the channel to its subscribers. The channel owner can, however, revoke the approval at any given time.

This mechanism of sending delegated notifications is quite effective in providing value-added services to the channels. It also ensures the availability of mechanisms that can be used by EPNS or any other third-party infrastructure to send on-chain notifications on the channel’s behalf.

## Questions
1. Which one of these is false about EPNS Notifications?
    * They can be sent for Ethereum-based projects only [✅]
    * They come with a clickable Call-to-Action link
    * They take almost no time to trigger

2. What kind of notifications can you send through EPNS?
    * Subset
    * Broadcast
    * Targeted
    * All of the above [✅]

3. Which one of the following is false about Delegated Notifications?
    * Channel owner can delegate notification sending power to any Wallet address
    * The Delegated wallet address can send notification on behalf of the channels
    * Once approved, a delegated wallet address cannot be removed by channel owner. [✅]
    * Delegated notification are sent on the behalf of the channel address instead of the delegated wallet address.
---
# EPNS Smart Contracts

In order for the protocol to be chain-agnostic as well as truly decentralized, EPNS smart contracts play a major role.
The EPNS Protocol has now been divided into two different smart contracts, i.e., EPNS Core & EPNS Communicator.

**1. EPNS Core Contract:**
The EPNSCore protocol, as the name might indicate, is the main smart contract as it handles some of the most crucial features like Channel creation, governance, channel state changes as well as funds and incentive mechanisms, etc.
It’s very important to note, however, that the EPNS Core smart contract will only be deployed on the Ethereum blockchain and not on any other chain.

**2. EPNS Communicator Contract:**
Unlike the EPNS Core smart contract, the communicator protocol is designed to be deployed on multiple chains. This is also one of the imperative reasons behind the communicator contract being lightweight and not reliant on the core contract.

The EPNS Communicator protocol is comparatively quite simple. The communicator protocol includes features that allow users to subscribe to a channel, unsubscribe from a channel as well as the imperative one, i.e., sending notifications. As the communicator protocol can be deployed on various chains, it allows us to trigger notifications on multiple chains and not just the Ethereum blockchain.

## Questions
1. Which contract is responsible for governance as well as incentive mechanisms?
    * EPNS Core [✅]
    * EPNS Communicator
2. To what extent is EPNS Communicator contract dependent on EPNS Core?
    * Very heavily dependent.
    * Doesn't need to interact with core at all. [✅]

3. Which of the following is not true about EPNS Core contract
    * It can only be deployed on Ethereum
    * Core contract deals with creation of channels
    * Subscribing or unsubscribing features are built in the core contract.[✅]
    * None of the above.

---
## Push Nodes

Push Nodes are the central piece of the network that enables the blockchain of Web3 notifications to work. In essence, they are validators that can be run by anyone in the future with staking and slashing

![](https://i.imgur.com/zY9YqmS.png)

### 3 main tasks of Push Nodes
1. **Listening**: Push Nodes listens to EPNS Communicator smart contracts on every blockchain. They also enable off-chain or direct communication via API calls either from a backend or a dApp. This enables EPNS to support just about any Web3 service… ie: smart contracts, dApps, backends or direct payloads.

2. Validating and Governing: The communication which is driven by the EPNS Communicator layers require validation. This validation involves ensuring that whether or not the channel exists, the channel is not spamming, the channel is cross-chain verified.le governance and to verify the existence of the channel.
3. Admitting to Network / Dispatching: Lastly, the Push Nodes admit these notifications that are tied to wallet address in the network which can then be tapped into by any crypto frontend / wallet to display them. The dispatch functionality is also present in these nodes to allow bridging of Web3 notifications to be displayed in Web2 apps in case the wallet / frontend / software wants to enable that instead of handling direct socket connection.


## Questions
1. Which feature of Push Nodes enables EPNS protocol to support about any Web3 service?
    * Validating and Governing
    * Listneing to on-chain and off-chain communication [✅]
    * Dispatching
    * None of the above
2. Does Push Node listen to EPNS Communicator smart contract on Ethereum blockchain only?
    * Yes.
    * No. [✅]
3. How is **Dispatch functionality of Push Nodes**, helpful?
    * Enables Gasless notifications
    * Bridges the gap between Web3 notifications and Web3 apps [✅]
    * Enhances speed of notification delivery
    * All of the above.
---
