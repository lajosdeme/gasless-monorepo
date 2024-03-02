# Gasless

Gasless is a plug-in and play relayer as a service app that dapp developers can subscribe to and then import our SDK into their dapps, to execute transactions using our relayer service and pay for gas on the users' behalf.    
     
This is a hackathon project so I was short on time to implement a good looking, great UI. All the other parts of the code are fully functional, working elements that users could actually use. If given more time, the frontend would have been more polished.

## Monorepo structure:
- `relayer`: This a Golang backend that is responsible for the core logic of Gasless. It handles registrations, logins, user subscriptions, and relay transaction executions.
- `relayer-sdk`: This is the frontend SDK that dapp developers can import into their apps to use Gasless.
- `relayer-subscription`: This is the smart contract on Lukso that handles collecting subscription payments in the form of LYX tokens and verifying whether a user is subscribed or not.
- `relayer-frontend-demo`: A minimal frontend to demonstrate retrieving user quota, registering, logging in, and subscribing to Gasless.
- `relayer-demo-script`: A simple script that demonstrates how a dapp developer can use our SDK to execute any action on a smart contract and have Gasless pay the gas.
