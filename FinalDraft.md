# Submission

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
    * Help PUSH token-holders to vote in EPNS governance proposals
    * All of the above [✅]


## What are Channels?
Any user who activates themselves as a service on the protocol to send notifications for its users can be considered a Channel.

In other words, any service, i.e., a dapp, protocol, or even a web2 service, that wants to send notifications out to its web3 users can choose to become a channel and establish an adequate communication bridge with its users.

The creation of a channel is just a one-time simple procedure. It must be noted that channel creation only happens on the Ethereum blockchain and one wallet address can only create one channel only the protocol.

> ***Note: Although channel creation only happens on the Ethereum blockchain, the protocol is designed to be chain-agnostic, i.e., channel owners can choose to send notification on any chain of their choice and not just Ethereum network***

A successfully created channel can send notifications to its subscribers, directly tied to their wallet addresses.

Once any user opts in and becomes a subscriber for a chanenel, he/she shall receive notifications from that channel directly in their inbox.
Users who are not a subscriber of a particular channel, receive notifications from that channel in their spam box.

> ***Opting In or Opting out of a Channel is a completely gasless transaction and requires no fees.***

## Questions
1. On which chain, does the channel creation happen?
    * Polygon
    * Ethereum [✅]
    * None of the above.

2. Can you send notifications only on Ethereum blockchain?
    * Yes, it’s restricted to the Ethereum blockchain only.
    * No, EPNS notifications are chain-agnostic and not tied only to Ethereum. [✅]

2. What happens if the user receives notifications from an unsubscribed channel?
    *  The User will not get that Notification.
    *  The User will receive the notification in the main inbox.
    *  The Notification will go to the Spam Box.[✅]

## Notifications

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

## Showrunners

The showrunners framework is a scaffold that developers can use to build out notifications for their use cases.

Showrunners framework provides the tools and helpers required for constructing the payload and sending the notification using the EPNS infrastructure.

Out-of-the-box showrunners provide the developer with a scheduling engine and libraries and helpers for easy access to blockchain data as well as web2 data sources.
