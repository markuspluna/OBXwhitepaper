![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/obx%20logo.png "Logo Title Text 1")
# OPTIONBLOX
## A Derivatives Writing and Trading Solution Built on Stellar

Markus Paulson-Luna: markuspaulsonluna@gmail.com  
Andrew Pierskalla: piers274@gmail.com  
Alexander Mootz: alexjmootz@gmail.com  

### Abstract

Adventum Technology presents OptionBlox, a solution for writing, trading, and exercising financial derivatives on Stellar's decentralized ledger. OptionBlox  decreases derivative market friction and costs by eliminating the need for market intermediaries. Processing derivatives on a multi-asset decentralized ledger increases market flexibility and accessability. We support derivatives involving any asset pair, and enable open derivative market access. OptionBlox uses a unique smart contract structure which allows for trust-free option, future, and swap writing. Our protocol tokenizes derivative contracts, which means they can be traded on any centralized/decentralized exchange and stored offline. Our protocol also excercises derivatives on-ledger without putting any part at risk. In addition, Adventum Technology showcases a unique ledger-based margin account framework. Using our protocol, organizations building exchanges on Stellar can provide their users with decentralized margin accounts that minimize default risk. 

### Introduction:

#### Derivatives:

A derivative is a contract between two parties. Its value is based on an agreed-upon asset or a set of assets. The most common forms of financial derivatives are futures, options, forwards, and swaps.

- Futures are contracts between two parties to buy/sell an agreed-upon quantity of an asset at a set price at an established future time. Futures are most commonly used to hedge against price movement by the underlying asset, as a means to increase leverage, or as a means of gaining exposure to rates. Futures are typically settled daily, so at the end of each day, an investor's profits or losses are realized.

- Options are contracts between two parties, a writer and a buyer. The contract gives the buyer the option, but not the obligation, to buy or sell an asset at an agreed-upon price until the option expires. If the buyer decides to exercise this right, the option writer would buy or sell the asset. Options can be either American or European style and can be either puts or calls. American style options can be exercised at any date up until their expiration date. European style options can only be exercised on their expiration date. A call option allows its owner to buy the underlying asset at the agreed-upon "strike price", and a put option allows its owner to sell the underlying asset at the strike price. Common uses of options are hedging, increasing leverage, and income generation.

- Forwards are similar to futures. The main difference is that they are not settled until the expiration date. They are typically highly specified to the buyer and seller's needs.

- Swaps are similar to forwards. The difference is that instead of one exchange of assets at the expiration date, the parties swap assets twice. Once at the beginning of the contract and once at the end. These exchanges are referred to as the "near leg" and the "far leg". Like forwards, these contracts are typically highly specified to the involved parties needs.
#### Value Proposition:  

- *Increased Efficiency*  
The incumbent derivatives market suffers from a large amount of friction. It requires middlemen to provide access to the market, facilitate trades, and lower counterparty risk. This inefficiency creates costs that get passed on to investors. A research paper that covered Stellar-based financial derivatives measured the increased efficiency that Stellar-based derivatives provide. To measure the costs that get passed to users in the traditional derivatives ecosystem, the paper measured central parties revenue-per-contract. To measure the costs associated with Stellar-based derivatives, they processed derivatives on-ledger, and measured the network fees. Their findings are summarized in the tables below.\ 
We expect these gains in efficiency to exponentially increase when it comes to OTC(Over-The-Counter) derivatives. OTC contracts are highly specified, complicated, and can carry a large amount of counterparty risk. Traditionally, a party that wants to enter an OTC contract will have to find both a counterparty, and a facilitating party. Our system eliminates the need for the facilitating party, and makes it easier to find a counterparty due to our open-market access. As a result, OptionBlox makes it significantly easier and cheaper to participate in the OTC derivatives markets.\
The formentioned research paper also discussed data access fees that derivative users pay to central parties in the traditional derivative ecosystem. These fees are another example of the inefficiency and friction in the traditional derivative ecosystem. In a Stellar-based derivative ecosystem all data would be public since all transactions are recorded on ledger. This would eliminate a significant source of cost and inefficiency. A table measuring these costs is pictured below.

**Ecosystem Fees Associated with Stellar Based Derivatives**

|Writing and Executing Options|Writing and Executing Futures|Writing and Executing Swaps|Trading all Derivatives|
|---|---|---|---|
|$0.000261|$0.000319|$0.0004234|$0.000029|

**Ecosystem Fees Associated with the Traditional Derivative Ecosystem**

|CBOE Option Revenue Per Contract|CBOE Futures Revenue Per Contract|CME Average Revenue Per Contract|
|---|---|---|
|$0.235|$1.759|$0.725|

**Live Data Fees in the Traditional Derivative Ecosystem**

|CBOE Live Data Fees|CME Live Data Fees|
|---|---|
|$105/month|Individual - $15,000
||Enterprise - $100,000|

> Citation: Paulson-Luna, Riley. "The Financial Derivatives Ecosystem is Old - Decentralized Ledger Technology is its Fountain of Youth". 2020. ASSE 2020.

- *Market Accessibility*  
OptionBlox increases market accessibility. Potential derivative users struggle to participate in derivative markets unless they live in developed nations. The decentralized nature of our system means our service is accessible to anyone with an internet connection. This accessibility creates open-access derivative markets.

- *Market Flexibility*  
Stellar's Anchor system combined with the flexibility of OptionBlox allows users to write derivatives with any asset. People with use cases for derivatives that are not currently supported by the traditional market can use our solution to write and trade derivatives that better suit their requirements.  

-*Tokenized Derivatives*
Derivatives written with OptionBlox are tokenized. Tokenized derivatives are essential in the decentralized ledger technology space. Tokenization allows our derivatives to be traded on any cryptocurrency exchange, and stored anywhere. A user could write a derivative on our exchange, then transfer it to their Binance account and sell it on their market. A derivative buyer could take their newly purchased derivative tokens and transfer them to their Ledger Nano S for added security. This flexibility is essential due to the fragmentation of the decentralized ledger technology space. It also serves to further decentralize OptionBlox. 

#### What Decentralized Ledger Technology Provides:

Using decentralized ledger technology to facilitate derivatives allows us to make OptionBlox more flexible and efficient than the incumbent derivative processing system, while still retaining a similar level of security. The elements of a decentralized system that are most important to us are:

- *Proof of ownership*  
The public and collective nature of a decentralized ledger prevents individuals from misrepresenting what they own on the ledger, including assets and transactions. This allows us to verify asset ownership, and to ensure derivatives are set up correctly. As a result, participants need for middlemen to handle counterparty risk is greatly reduced.

- *Accessibility*   
Decentralized networks are incredibly accessible. They are run by a network of nodes situated around the globe, and any individual can connect to the network or become one of the nodes. On top of this, Stellar has an exchange functionality built into its network. The open nature of this system means that consumers no longer require a third party to host an electronic exchange and provide them access to it. Additionally, it opens the market to new parties that find it difficult to access incumbent markets. Finally, open-market access, combined with the OptionBlox's flexibility, allows consumers to write new kinds of derivatives, potentially creating new markets.

- *One source of truth*  
The unquestionable nature of a decentralized network, combined with its accessibility means participants don't need to pay for or share market data to maintain an accurate source of information. This removes another source of friction and cost.

#### Our Decentralized Ledger:

We use Stellar's decentralized ledger to support our protocol.

In Stellar’s words:  

“Fundamentally, Stellar is a system for tracking ownership. It uses an accounting ledger, shared across a network of independent computers, to store two important things for every account holder: what they own (their account balances) and what they want to do with what they own (operations on those balances, like buy or sell offers.)

The computers that run Stellar and publish the ledger are called nodes. They systematically validate the ledger’s contents so it’s always consistent across the network. For example, when you send someone a dollar on a Stellar-built app, the nodes check that the correct balances were debited and credited, and each node makes sure every other node sees and agrees to the transaction.”

Stellar's open network allows anyone to submit a transaction to change the ledger. However, the transaction will only change the ledger after the nodes agree it is valid. In our case, before a derivative is exercised or traded, the local network of nodes agree upon the validity of the transaction. This prevents parties with ill intentions from engaging in illicit behavior on the network. Therefore, we have a secure financial network that has one source of truth and can be instantly accessed and modified by anyone in the world.  

For more general information visit: [Stellar's Website](https://www.stellar.org/developers/guides/walkthroughs/stellar-smart-contracts.html).  
For more information on how the nodes validate transactions see: [Stellar Consensus Protocol](https://www.stellar.org/developers/guides/concepts/scp.html).  
For more information on how we interact with Stellar’s network visit: [Network Overview](https://www.stellar.org/developers/guides/get-started/index.html).

Terms:  
- *Smart Contract:* A protocol to digitally facilitate, verify, or enforce the performance of a contract.  
- *Keypair:* When an account is created on Stellar's ledger, they are assigned a public and a private key. The private key is used to sign transactions and the public key is used to identify the account. These two keys make up the account's keypair.

#### Stellar's Features:

OptionBlox utilizes Stellar's transaction system to create derivative smart contracts. Stellar has unique features that make it an ideal platform to develop our application on.  
- *Efficiency*  
Stellar’s network is efficient, having both fast transaction times and low fees. This is essential for a derivative market and is one of the main areas where Stellar shines versus other networks like Etherium.  
- *Decentralization*  
Unlike other blockchains, Stellar's network is truly decentralized. There is no governing body we need to rely on, as long as Stellar has users, our product will function.
- *[Anchors](https://www.stellar.org/developers/guides/concepts/assets.html)*  
Stellar has a multi-asset functionality called anchoring that enables users to create custom assets on its ledger and tie them to real-world assets. We use this to tokenize derivatives and to write derivatives involving any asset.  
- *Flexible Transaction System*  
Stellar has a flexible transaction system that allows us to create derivatives and make them trust-free, tradeable, and safe.  

[Stellar's website](https://www.stellar.org/developers/guides/walkthroughs/stellar-smart-contracts.html)

### Use Cases:
OptionBlox can be used for all of the functions traditional derivatives could be used for such as investment and risk management. It performs these functions more efficiently than incumbent system due to the friction reduction we discussed previously. We will discuss a few use cases that highlight the flexibility and accessability of our system. 

1. **Cryptocurrency Investment Hedging:**  
A primary concern for cryptocurrency holders is volatility. OptionBlox enables users to utilize financial derivatives to hedge against cryptocurrency volatility. OptionBlox's capability of supporting any asset pair means it supports a wide range of cryptocurrencies. In addition, OptionBlox's efficiency and accessibility results in lower fees and tighter spreads than competing solutions.

   Latera is an investor. He beleives in Stellar's future and wants to hold XLM. However, the volatility of cryptocurrency is a major deterrent. He comes across a tool called OptionBlox that allows him to enter into an option contract guaranteeing him the option to sell 100xlm for $7.00 in 1 year's time. This hedges him against any potential downward movement by XLM. He purchases a large batch of contracts and enters into his XLM investment.

2. **OTC Derivatives in Developing Countries:**  
OTC derivatives are useful for all businesses. However, in order to enter an OTC derivative contract, the interested party must find a counterparty and facilitating party. This creates issues for unsophisticated parties lacking relationships with these entities. [A recent paper published by the IMF](https://www.elibrary.imf.org/view/IMF001/25871-9781498303774/25871-9781498303774/25871-9781498303774_A001.xml?redirect=true) found that the OTC derivative market suffers from price discrimination. Unsophisticated parties lack market accessibility, and as a result, they pay larger spreads than sophisticated parties. OptionBlox solves this problem by removing facilitating parties from the equation, and by enabling derivative trading on an distributed ledger. This makes it much easier for unsophisticated parties to find a counterparty, and eliminates their need to find a facilitating party. 

   Adam is a citizen and resident of Vietnam. He owns a clothing factory and most of his revenue is received in USD. However, most of his expenses are paid in Vietnamese Dong(VND). He would like to hedge against exchange rate fluctuations by entering an OTC USD:VND future. However, he is not a large enough client to have connections with foreign banks or facilitating parties in the derivatives market. To make things more difficult, foreign currency exchange is illegal in Vietnam. Adam finds out about OptionBlox and realizes it is the answer to his problems. Using OptionBlox, he enters into an OTC USD:VND future with a western bank that also wants to hedge against exchange rate fluctuations. Because he did not have to find a facilitating party, and had access to a wide range of counterparties, the spread he payed using OptionBlox was small. The distributed nature of the application also allowed him to circumvent local currency controls.

3. **Carbon Credits Use Case:**\
Carbon emissions are a crucial issue today. One proposed way to handle them is by issuing carbon credits to companies. These credits govern how much carbon companies can emit and can be traded between companies, so that they are used most efficiently. Using OptionBlox, with the help of a carbon credit anchor, companies could trade derivatives on their carbon credits.

   Xiao is an executive at a major battery producer. Business is booming, and she wants to expand operations, however, her company needs to continually purchase more carbon credits to do so. As a result, future carbon credit price increases are a risk for this expansion. Xiao does some research and discovers OptionBlox. She realizes she can use our product to purchase carbon credit call options, hedging her company against the risk of carbon credit price increases. Her company purchases the calls and goes ahead with the expansion. 
   
4. **Large Scale Derivative Clearing**\
Central derivative post-trade processing is a time intensive and costly process. We beleive that the eventual path of the industry is to move derivative processing onto a decentralized ledger. Once this transformation takes place, central parties could use our protocol to replace a majority of their post-trade processes.

### OptionBlox's Solutions:
#### Derivatives:
OptionBlox features a range of tradeable decentralized derivative products
##### Covered Options
Our covered options are created using a network of accounts and preauthorized transactions. This protocol is based completely on Stellar's network and can operate without any input besides users submitting transactions. These options are European style.  

Below is a basic model showing the writing, sale, and exercise processes of a covered call with an underlying of 1 Bitcoin(BTC), and a strike price of 50 Lumens(XLM).

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/coveredOptions-model(whitepaper).png "Covered Options")

##### Uncovered Options
Our uncovered options use a similar process as our covered options. The key difference is the holding account also serves as a margin account for the seller. We use an open-source code repository to operate the logic surrounding margin requirements. Stellar's native operations are not complicated enough to allow us to calculate margin requirements within transactions. Using a repository also increases processing speed.  We create an encrypted keypair for the repository to accomplish this securely. We do not have access to this keypair. We then add the repository's secret key as a signer on the holding account. This allows the repository to sign pre-defined transactions for the holding account.

Below is a model showing the writing, sale, and execution process of an uncovered call. The call's underlying is 1 BTC, its strike price is 50 XLM, the initial margin requirement is 20%, and the minimum margin requirement is 15%. These options are European style.

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/uncoveredOptions-model(whitepaper).png "Uncovered Options")

##### Futures
Our futures protocol expands on the uncovered options protocol. We use two margin and holding accounts, one for the buyer and one for the seller. We use the same open-source repository that we use with uncovered options to handle the margin and settlement operations. We settle our futures daily

Below is a basic model showing the writing, sale, execution, and exit of a 100XLM:1BTC future with a 15% initial margin requirement and a 10% minimum margin requirement

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/Futures-model(whitepaper).png "Futures")

##### Forwards
Our forwards protocol operates almost the same way as our futures protocol. The main difference is that forwards do not settle daily. As a result, underlying values do not change. Therefore, we can use joint-preauthorized transactions in the exercise process instead of signing transactions with the repository.

##### Swaps
Our swaps protocol operates almost the same way as our forwards protocol. We just add a near leg exercise step.

Below is a basic model showing the writing, sale, and execution of a 100XLM:1BTC swap with a 15% initial margin requirement and a 10% minimum margin requirement

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/Swaps-model(whitepaper).png "Swaps")

#### Margin Accounts:
We offer margin accounts for organizations that want to provide their decentralized exchange users with margin. We utilize a global holding account that stores user's deposits and sends them a custom margin asset in exchange. The margin funds are deposited in user accounts where the repository is the only signer. The repository will only sign trustline operations for approved assets and buy/sell transactions. This prevents users from moving margin assets or assets they purchase out of this account. We require a margin balance in this account and will perform margin checks and calls on it.

Below is a basic model showing a margin account with a 50% margin, an initial deposit of 100xlm, and rebalancing required when the account loses 20% of its initial value.

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/margin%20account%20(whitepaper).png "Margin Account Architecture")

### Security:

We use a variety of Stellar's features to ensure that our derivatives and margin accounts are secure.

- *Locking Accounts and Preauthorizing Transactions*  
In most of our protocols, we have accounts preauthorize transactions then lock themselves. This ensures that the only transactions they can post in the future are the preauthorized ones. We use this to lock funds in holding accounts until contract exercise.  
[More info](https://www.stellar.org/developers/guides/concepts/multi-sig.html)

  - *Joint Preauthorized Transactions*  
Joint-preauthorized transactions allow us to preauthorize transaction envelopes involving multiple source accounts. This prevents situations where preauthorized transactions for one holding account fail while the other account's preauthorized transactions succeed.

- *Timebound Transactions*  
In all of our protocols, we use timebound transactions in the exercise process to ensure certain transactions cannot be submitted early. Submitting some transactions early would disrupt the exercise process.  
[More Info](https://www.stellar.org/developers/guides/concepts/multi-sig.html)

- *Stellar Consensus Protocol*  
Stellar's consensus protocol rejects transactions when they do not align with the correct ledger state. For example, a user could not fill a sell offer if their account lacked the necessary funds.  
[More Info](https://www.stellar.org/developers/guides/concepts/scp.html)  

- *Authorization Required Flag*  
We have the option of adding an authorization required flag to our issuing accounts. This ensures that the only accounts which can hold our custom assets are accounts that we approve.

- *SEP-0007 Integration*
We do not want to serve as custodian for users keys due to the risks this entails. Instead we will use Stellar's SEP-0007 protocol to send transaction envelopes to users who can then add their signature in a trusted application or exchange.
[More Info](https://github.com/stellar/stellar-protocol/blob/master/ecosystem/sep-0007.md)

### Anchors:

The functionality of OptionBlox is directly tied to the availability of Anchors in the Stellar ecosystem. To use a non-native asset as an underlying there has to be a third party already anchoring the asset.  
Here are some non-native assets that are currently anchored by reputable parties:
- USD: US dollar anchor provided by [AnchorUSD](https://www.anchorusd.com/), a Stellar partner.
- XCN: Chinese yuan anchor provided by [FChain](https://fchain.io).  
- BTC: Bitcoin anchor provided by [Papaya](https://apay.io/in).
- EURT: Euro anchor provided by [Tempo](https://tempo.eu.com/en).
- NGNT: Nigerian Naira anchor provided by [Cowrie](https://www.cowrie.exchange/).
- GOLD: Gold anchor provided by [StellarMetals](stellarmetals.org).
- ETH: Etherium anchor provided by [Papaya](https://apay.io/in).

More anchors can be viewed on [StellarX](https://www.stellarx.com/markets)

As Stellar's network grows we are confident that more anchors will materialize and expand OptionBlox's functionality.

### Next Steps:

At Adventum we are in the beginning stages of building the OptionBlox backend and platform. While we are doing this we will be searching for potential investors and partnerships.
##### Roadmap
1. *Q1 2020*
   - Begin Application Development
   - Grow OptionBlox's Brand
      - Put out content.
      - Explore presenting at conferences.
   - Attract New Talent (primarily in engineering)
   
 2. *Q2 2020*
   - Finalize Investor Material
      - Finalize Website.
      - Finalize Investment Pitch.
   - Continue Application Development
   - Continue Building OptionBlox's Brand
   - Begin Approaching Potential Investors and Partners
      - We will begin looking for a seed investor.
      - We are going to start reaching out to blockchain and finance orgs that may have a use for our platform.
           - Focusing on Wallets, Exchanges, Market Makers, Hedge Funds, and Payment Platforms.
 3. *Q3 2020*
   - Launch MVP and Push it Open-Source
