# Submission

# What is EPNS

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

---

# What are Channels?
Any user who activates themselves as a service on the protocol to send notifications for its users can be considered a Channel.

In other words, any service, i.e., a dapp, protocol, or even a web2 service, that wants to send notifications out to its web3 users can choose to become a channel and establish an adequate communication bridge with its users.

The creation of a channel is just a one-time simple procedure. It must be noted that channel creation only happens on the Ethereum blockchain and one wallet address can only create one channel only the protocol.

> ***Note: Although channel creation only happens on the Ethereum blockchain, the protocol is designed to be chain-agnostic, i.e., channel owners can choose to send notification on any chain of their choice and not just Ethereum network***

A successfully created channel can send notifications to its subscribers, directly tied to their wallet addresses.

Once any user opts in and becomes a subscriber for a chanenel, he/she shall receive notifications from that channel directly in their inbox.
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
    * Ethereum
    * None of the above.

2. Can you send notifications only on Ethereum blockchain?
    * Yes, it’s restricted to the Ethereum blockchain only.
    * No, EPNS notifications are chain-agnostic and not tied only to Ethereum.

2. What happens if the user receives notifications from an unsubscribed channel?
    *  The User will not get that Notification.
    *  The User will receive the notification in the main inbox.
    *  The Notification will go to the Spam Box.

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

---

# Push Nodes

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
    * EPNS Core
    * EPNS Communicator
2. To what exten is EPNS Commiuncator contract dependent on EPNS Core?
    * Very heavily dependent.
    * Doesn't need to interact with core at all.

3. Which of the following is not true about EPNS Core contract
    * It can only be deployed on Ethereum
    * Core contract deals with creation of channels
    * Subscribing or unsubscribing features are available on core contract.
    * None of the above.

---
# EPNS SDK

EPNS SDK is a growing Monorepo of packages that provide solutions for a wide range of development tasks one might come across while building on top of EPNS protocol.

It is a Javascript-based group of packages that helps developers to:
* Send notifications
* Subscribe (opt in) / Unsubscribe (opt out)
* Build EPNS features into their dApps
* Enable Access to Push Nodes APIs
* Render Default Notifications UI, etc


It is written in Typescript and supports React, React Native, Plain JS, and Node JS-based platforms. (We are adding support for more!).
It is also built on top of standard Web3 packages like *ethers, @web3-react*

## EPNS SDK Features

The SDK provides us with the following imperative features:
* Sending Notifications
* Opt-in to a Channel
* Opt-out from a channel
* Fetching notifications for a given user address
* Fetching Spam notifications for a given user address
* Fetching User subscriptions
* Fetching Channel Details
* Search for any particular channel
* Notification Components and view
* Embedded Notifications

---
## Showrunners

The showrunners framework is a scaffold that developers can use to build out notifications for their use cases.

Showrunners framework provides the tools and helpers required for constructing the payload and sending the notification using the EPNS infrastructure.

Out-of-the-box showrunners provide the developer with a scheduling engine and libraries and helpers for easy access to blockchain data as well as web2 data sources.

---

# Creating a Channel

Creating a channel is the very first step for sending notifications via EPNS.

Any wallet which activates itself on the EPNS Protocol to send a notification is called a Channel.

Using the EPNS dApp or our smart contracts, anyone with a wallet address on the Ethereum network can create their own channel. It can be deployed on;
* The Ethereum Mainnet (via[ Prod dApp](https://app.epns.io/)), or
* Kovan Test Network (via [Staging dApp](https://staging-app.epns.io/))

## Requirements for Setting Up a Channel
Ideally, there are 6 crucial requirements for creating a Channel.

1. A Channel Name
2. Channel Logo (an image of size 128px * 128px)
3. Alias Network (required for multi-chain, for example, if on Polygon, provide Polygon address of your contract, else can be left blank, currently supports only Polygon).

> *Important: This field needs to be provided at the very start in case you want to enable your channel on other blockchain networks, see  for guides and to understand the process.*

4. A brief Channel Description (250 Characters)
5. Channel CTA (Call To Action link)
6. An amount of 50 DAI in your Wallet (and some ETH )

> *If you are setting up a Channel on Staging dApp, you can get Free DAI and Kovan ETH from the dApp & online faucets. No need for real DAI/ETH on the Staging app 😁*

## Enabling Channel on Other Chain
As previously mentioned, although channel creation happens on Ethereum itself, the protocol is designed to enable the channel to send notification on any chain.

This is exactly where Channel Alias set-up plays a major role.

### How to set up Channel Alias?
In order to set-up channel alias address for any preferred chain, one has to go through 2 simple steps:

* Selecting the chain and providing the right alias address for the channel during channel creation itself.
* Verification of the alias Address on the selected chain.

---
# Sending Notifications

Who can Send Notifications?
As per the current design of the protocol, there can be 3 main actors who can send notifications:
1. **Channel Owners**: The owners of a particular channel can send notifications to their subscribers.

3. **Delegate Notification Senders**: Channel owners can allow any particular wallet address to send notifications on behalf of his/her channel. This feature is called delegated notifications and you can read more about it in this section 👉
4. **Notifications To Yourself**: The EPNS Communicator allows any address to send notifications to themselves 😃 It’s important to note, however, that the address sends the notification to themselves only.

> **Note:**
> *Sending notifications is a **gasless** transaction and therefore notification senders need not pay any gas fee while sending notifications via the Dapp.*
>
> *Gas Fees are only applicable when on-chain notifications are triggered directly from smart contracts.*


## How to trigger and send notifications

EPNS protocol provides many ways to trigger a notification. For instance, a channel owner or delegate can trigger notifications using:

* [EPNS Dapp](https://docs.epns.io/developers/developer-zone/sending-notifications/dapp-serverless-workflow)
* Using EPNS SDK
* [Using Subgraph](https://docs.epns.io/developers/developer-zone/sending-notifications/using-subgraph)
* [Using Showrunners](https://docs.epns.io/developers/developer-zone/sending-notifications/using-showrunners-scaffold-gasless)

---
# Receiving Notifications

Receiving notifications is a farily simple process and can be done very easily.

As of now, EPNS allows you to receive notifications directly to your wallet addresses through the crypto front-ends, in the form of SNS Notifications etc.

## Receiving notifications via SNS

### What are SNS Notifications
SNS module for Push Delivery Nodes allows any developer to receive notifications, chats, or any other form of web3 communication directly to the platform they are building with the help of webhooks.

Hosted SNS Module is a mid-level solution that eliminates all the heavy load of running a node or syncing information and gives you webhooks that you implement to start receiving notifications, chats, or any other web3 communication in your software.

### How to get started with hosted SNS module?

Integrating the SNS module into your code takes less than 10 mins and contains just 3 steps:

1. **Step 1**: Implement a webhook to listen to AWS SNS. Here’s a boilerplate along with specs to get you npm installed and running: https://github.com/ethereum-push-notification-service/epns-sns-boilerplate
2. **Step 2**: You will need to open an endpoint either at a dedicated IP that listens to SNS or, if you are testing locally, have to expose the public endpoint for which tons of software is available.

> *Hint: For testing locally, You can also use ngrok to expose the public endpoint. If you use this with the boilerplate, the port needs to be 6000. The ngrok URL is now the SNS endpoint required in step 3*.

 **Step 3**: Once you set up this, you need to contact us by either shouting / tagging us on Discord or reaching out via the contact form. We need this as the SNS module requires whitelisting of your webhook endpoint.

> [EPNS Boiler Plate](https://github.com/ethereum-push-notification-service/epns-sns-boilerplate) can also be used as a starting point to consume the feeds from the EPNS SNS Topic.

**Watch this quick video guide to ensure the right set-up**

[**SNS for Push Delivery Node**](https://www.youtube.com/watch?v=VocGkaL0eEA)

---
# EPNS Starter Kit

The SDK starter-kit is meant to showcase developers on how to use the EPNS SDK packages -

* [@epnsproject/sdk-restapi](https://www.npmjs.com/package/@epnsproject/sdk-restapi) Provides access to EPNS backend APIs.

* [@epnsproject/sdk-uiweb](https://www.npmjs.com/package/@epnsproject/sdk-uiweb) Provides React based components to show Notifications, Spam, SubscribedModal etc for dApps.

* [@epnsproject/sdk-uiembed](https://www.npmjs.com/package/@epnsproject/sdk-uiembed) Provides vanilla JS sidebar notifications for any dApp.

> CRA-Typescript
This particular kit is built out using CRA, Typescript. The SDK packages should also work out for React using plain JS.

## How to get started with the SDK Starter Kit?

```
git clone https://github.com/ethereum-push-notification-service/epns-sdk-starter-kit.git

cd epns-sdk-starter-kit

yarn install
yarn start
```

### Dependencies

If you are trying to build out a separate dapp following this starter-kit example, some of the following dependencies might be required for the SDK and any dApp to work.

1. @epnsproject/sdk-uiweb has a peerDependency on styled-components

    `yarn add styled-components`

2. Since its a dApp, the following are the web3 dependencies that you can install for wallet connection
 ` yarn add ethers`

3. The next package might only be needed if you are using web3-react. *You are free to use any other React based web3 solution.*

`yarn add @web3-react/core @web3-react/injected-connector`

> **Note:** *No need to install these if you are using the starter-kit itself since we have already installed these for you so that you can focus on how to use the EPNS-SDK packages*

## Quick Walkthrough of the App
The App has the following features-
The App has following features-

| Page    | Features    | SDK package used |
|----------|---------|---------|
| Notifications    | notifications, <br/>spams, <br/>subscribed modal  |  @epnsproject/sdk-uiweb, <br/>@epnsproject/sdk-restapi    |
| Channels     | get channel details for a specific channel, <br/>search for channel(s), <br/>get channel subscribers, <br/>is the logged-in user subscribed to the channel, <br/>opt in a channel, <br/>opt out a channel  | @epnsproject/sdk-restapi      |
| Payloads     | send notification for different use cases  | @epnsproject/sdk-restapi      |
| Embed | sidebar notifications for the logged in user if subscribed on EPNS  |   @epnsproject/sdk-uiembed    |
