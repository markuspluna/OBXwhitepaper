# OptionBlox Margin Account Primer

## Intro
OptionBlox offers a margin account solution for organizations who want to provide their users with margin accounts built on a decentralized ledger. This solution is flexible and designed to be tailored to our partner's needs. 
### Margin Asset
Our protocol uses a custom margin asset which serves as the user's margin balance. This allows us to issue credit to users. When the user closes their account, our holding account will exchange the margin asset for the asset type the user deposited.  
For example:
1. The user deposits 100 Lumens(XLM) in exchange for 150XLM worth of margin balance (XLMM)
2. The user makes 30 XLM through trading
3. The user closes their account sending 180XLMM to the holding account
4. The holding account sends 130 XLM back to the user

Using a custom margin asset means the ecosystem will have to use custom margin assets for all trading. Stellar does not allow accounts to have multiple sell offers for the same asset. For example, a user would not be able to have an offer to sell 1 BTC for 500XLM  and an offer to sell the same BTC for 500 XLMM. Therefore, all accounts will need to exchange their deposit asset for a custom margin asset, whether or not they are using margin. Non-margin accounts would not receive any margin asset on credit.
### Global Holding Account
Our protocol uses a Global Holding Account to store user deposits. It pays out these deposits to users who close accounts in exchange for their margin assets. The only signer on this account is the repository, and it will only sign a few predefined transactions.
### Repository
Our protocol uses an open-source repository to manage the holding account and user accounts. It signs pre-defined transactions such as trading transactions, deposit transactions, and the transactions required to close an account. Using the repository ensures users know their deposits are secure, and users cannot transfer assets purchased with margin credit outside of our network.
### Margin Calls
In the case of a margin call, our repository stops signing transactions for the user until they deposit the necessary funds. If they fail to do so, we liquidate their account. 

Our margin requirements are flexible to the needs of the organization we are working with. If a user's account value falls to the point where the account is illiquid, we do not take responsibility for the bad debt expense.

## Model

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/Margin%20Account%20.png "Model")
