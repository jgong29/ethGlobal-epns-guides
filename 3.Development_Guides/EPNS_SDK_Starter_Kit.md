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
