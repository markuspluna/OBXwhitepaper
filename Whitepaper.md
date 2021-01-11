![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/obx%20logo.png "Logo Title Text 1")
# OPTIONBLOX
## A Decentralized Derivatives Solution Built on Stellar

Markus Paulson-Luna: markuspaulsonluna@optionblox.com\
Andrew Pierskalla: andrew@optionblox.com\
Alexander Mootz: alex@optionblox.com

### Abstract

OptionBlox is a protocol for writing, trading, and exercising financial derivatives on Stellar's decentralized ledger. OptionBlox uses a unique smart contract system to make these derivatives trust-free as well as ledger-based. Doing so eliminates the need for market intermediaries- increasing ecosystem efficiency, flexibility, and accessibility. The OptionBlox protocol supports derivatives involving any asset pair, charges less than 1 cent per contract, and can be used by anyone in the world. Additionally, OptionBlox tokenizes derivative contracts, allowing them to be traded on any centralized or decentralized exchange, and even stored offline. Overall, OptionBlox makes vast improvements on incumbent derivative processing solutions and enables equitable access to a flexible, efficient derivatives market built on Stellar. 

*Note: The OptionBlox protocol refers to an umbrella of protocols that process different derivative types. Protocols vary slightly based on the derivative type they support.*

### Table of Contents:
- [Introduction](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#introduction)
- [Explination of Derivatives](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#derivatives)
- [Value Proposition](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#value-proposition)
- [Use Cases](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#use-cases)
- [Stellar - OptionBlox's Decentralized Ledger](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#stellar---optionbloxs-chosen-decentralized-ledger)
- [OptionBlox's Derivative Protocols](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#optionbloxs-derivative-protocols)
- [Security Measures](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#security)
- [Roadmap](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#roadmap)
- [Glossary](https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md#glossary)

### Introduction:

#### Derivatives:

A derivative is a financial contract between two parties. Its value is based on an agreed-upon asset or a set of assets. The most common forms of financial derivatives are futures, options, forwards, and swaps.

- *Futures*:   
Futures are contracts between two parties to buy/sell an agreed-upon quantity of an asset, called the underlying asset, at a set price at an established future time. Futures are commonly used to hedge against price movement by the underlying asset, as a means to increase leverage, or as a means of gaining exposure to rates. Futures are typically settled daily, so at the end of each day, an investor's profits or losses are realized.

- *Options*:   
Options are contracts between two parties, a writer and a buyer. The contract gives the buyer the option, but not the obligation, to buy or sell an asset, called the underlying asset, at an agreed-upon "strike price" until the option expires. If the buyer decides to exercise this right, the option writer would buy or sell the underlying asset. Options can be either puts or calls. A call option allows its owner to buy the underlying asset at the strike price, and a put option allows its owner to sell the underlying asset at the strike price. Common uses of options are hedging, increasing leverage, and income generation.

- *Forwards*:  
Forwards are similar to futures. The main difference is that they are not settled until the expiration date. They are typically highly specified to the involved parties' needs.

- *Swaps*:  
Swaps are similar to forwards. The difference is that instead of one exchange of assets at the expiration date, the parties swap assets twice. Once at the beginning of the contract and once at the end. These exchanges are referred to as the "near leg" and the "far leg". Like forwards, these contracts are typically highly specified to the involved parties' needs.
#### Value Proposition:  

##### Increased Efficiency  
The incumbent derivatives market suffers from a large amount of friction. It requires market intermediaries to provide access to the market, facilitate trades, and lower counterparty risk. These additional parties cause inefficiency which creates costs that get passed on to investors. By facilitating derivatives on Stellar's decentralized network, OptionBlox eliminates the need for market intermediaries. The diagram below illustrate the efficiency gained by eliminating market intermediaries by comparing the post-trade process in the traditional derivatives ecosystem with the post-trade process in the OptionBlox derivatives ecosystem.

**Post-Trade processing comparison**\
![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/post-trade%20processing%20comparison.jpg "Post-Trade Processing Comparison")
> Citation: ISDA. "The Future of Derivatives Processing and Market Infrastructure". ISDA Whitepaper. 2016.


A research paper that covered Stellar-based financial derivatives measured the monetary impact of the increased efficiency that Stellar-based derivatives provide. To measure the costs that get passed to users as a result of inefficiency in the traditional derivatives ecosystem, the paper measured central parties' revenue-per-contract. To measure the costs associated with Stellar-based derivatives, the researchers processed derivatives on-ledger and measured the network fees. Their findings are summarized in the tables below.\
 \
We expect these gains in efficiency to exponentially increase when it comes to OTC(Over-The-Counter) derivatives. OTC contracts are highly specified, complicated, and can carry a large amount of counterparty risk. Traditionally, a party that wants to enter an OTC contract has to find both a counterparty and a facilitating party. OptionBlox's protocol eliminates the need for the facilitating party and makes it easier to find a counterparty by improving ecosystem accessibility. As a result, OptionBlox significantly increases OTC derivative efficiency and accessibility.\
 \
The formentioned research paper also discussed data access fees that derivative users pay to central parties in the traditional derivative ecosystem. These fees are another example of inefficiency and friction in the traditional derivative ecosystem. In a Stellar-based derivative ecosystem, all data would be public since all transactions are recorded on-ledger. This would eliminate a significant source of cost and inefficiency.\
\
OptionBlox also holds efficiency advantages over other decentralized derivative products. Most of these are built on Ethereum, which is a fundamentally less efficient decentralized ledger than Stellar.\
\
Tables exhibiting the economic impact of the formentioned efficiency increases are exhibited below:


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

**Ecosystem Fees Associated with Ethereum Based Derivatives**
|Writing and Executing Derivatives|Trading all Derivatives|
|---|---|
|$5.50+|$1.10+|

> Citation: Paulson-Luna, Riley. "The Financial Derivatives Ecosystem is Old - Decentralized Ledger Technology is its Fountain of Youth". 2020. ASSE 2020. DOI= https://dl.acm.org/doi/abs/10.1145/3399871.3399904

##### Market Accessibility  
OptionBlox uses DLT(Decentralized Ledger Technology) to make improvements in derivative ecosystem accessibility. The decentralized nature of OptionBlox means it is accessible to anyone with an internet connection. This is a huge improvement over the current state of the derivatives ecosystem where only a minute portion of the world has efficient ecosystem access. The incumbent derivative ecosystem’s dependence on central parties makes it impossible for it to serve a wider market. Since OptionBlox uses DLT to facilitate derivatives instead of central parties, it does not suffer from these limitations. Accessibility is core to OptionBlox’s offering, we want the protocol to enable equitable derivative ecosystem access. With OptionBlox’s innovation in accessibility, flexibility, and efficiency we believe it will do so. 

##### Flexibility  
OptionBlox provides unparalleled flexibility, allowing users to accomplish any derivative use case. If our standardized derivatives do not meet a user's needs they can easily write OTC derivatives with custom contract specifications using OptionBlox. Additionally, derivatives written with OptionBlox use Stellar’s [Anchor](https://www.stellar.org/developers/guides/concepts/assets.html) system to manage contract underlying assets. Since the Anchor system can support any asset, OptionBlox contracts can be written with any underlying asset.

- *Tokenized Derivatives*:  
OptionBlox also uses the Anchor system to tokenize derivative contracts. Tokenized derivatives are essential in the decentralized ledger technology space. Tokenization allows OptionBlox derivatives to be traded on any cryptocurrency exchange and stored anywhere. This flexibility is essential due to the fragmentation of the DLT space. It also serves to further decentralize OptionBlox. In addition to improving trading and storage flexibility, tokenization allows users to write partial derivatives, enabling users with different levels of wealth to take advantage of derivatives while still allowing us to retain standardized derivative sizes. For example, default OptionBlox Ethereum options are standardized to have an underlying of 1 ETH to preserve contract volume, if a user wants to write this option but cannot fund the entire 1 ETH underlying, OptionBlox's partial derivative capability will allow them to write a fractional derivative. They will provide a fraction of 1 ETH as contract collateral and will receive a proportional fraction of an ETH option token. 

#### [Use Cases](http://optionblox.com/use-cases)

#### What Decentralized Ledger Technology Provides:

Using decentralized ledger technology to facilitate derivatives allows us to make OptionBlox more flexible and efficient than the incumbent derivative processing system, while still retaining a similar level of security. A decentralized system provides:

- *Proof of ownership*:  
The public and collective nature of a decentralized ledger prevents individuals from misrepresenting what they own on the ledger, including assets and transactions. This allows OptionBlox to verify asset ownership, and to ensure derivatives are set up correctly. As a result, participants' need for middlemen to handle counterparty risk is greatly reduced.

- *Accessibility*:   
Decentralized networks are open ecosystems. They are run by a network of nodes situated around the globe, and any individual can connect to the network or become one of the nodes. On top of this, Stellar has a decentralized exchange built into its ledger. The open nature of this system means that consumers no longer require a third party to host an electronic exchange and provide them access to it. Additionally, it opens the market to new parties that find it difficult to access incumbent markets. Finally, open-market access, combined with the OptionBlox's flexibility, allows consumers to write new kinds of derivatives, potentially creating new markets.

- *One source of truth*:  
The unquestionable nature of a decentralized network, combined with its accessibility means participants don't need to pay for or share market data to maintain an accurate source of information. This removes another source of friction and cost.

#### Stellar - OptionBlox's Chosen Decentralized Ledger:

OptionBlox uses Stellar's decentralized ledger to support its protocol.

In Stellar’s words:  

“Fundamentally, Stellar is a system for tracking ownership. It uses an accounting ledger, shared across a network of independent computers, to store two important things for every account holder: what they own (their account balances) and what they want to do with what they own (operations on those balances, like buy or sell offers.)

The computers that run Stellar and publish the ledger are called nodes. They systematically validate the ledger’s contents so it’s always consistent across the network. For example, when you send someone a dollar on a Stellar-built app, the nodes check that the correct balances were debited and credited, and each node makes sure every other node sees and agrees to the transaction.”

Stellar's open network allows anyone to submit a transaction to change the ledger. However, the transaction will only change the ledger after the nodes agree it is valid. In OptionBlox's case, before a derivative is exercised or traded, the local network of nodes agree upon the validity of the transaction. This prevents parties with ill intentions from engaging in illicit behavior on the network. Therefore, Stellar provides a secure financial network that has one source of truth and can be instantly accessed and modified by anyone in the world.  

For more general information visit: [Stellar's Website](https://www.stellar.org/developers/guides/walkthroughs/stellar-smart-contracts.html).  
For more information on how the nodes validate transactions see: [Stellar Consensus Protocol](https://www.stellar.org/developers/guides/concepts/scp.html).  
For more information on how OptionBlox interacts with Stellar’s network visit: [Network Overview](https://www.stellar.org/developers/guides/get-started/index.html).

##### Building on Stellar:

Stellar’s focus on financial applications has made it the ideal network to develop OptionBlox on.\
Characteristics of the Stellar network crucial to OptionBlox:
- *Efficiency*:  
Stellar’s network is efficient, having both fast transaction times and low fees. This is essential for a derivative market and is one of the main areas where Stellar shines versus other networks like Ethereum.  
- *Decentralization*:  
Unlike other blockchains, Stellar's network is truly decentralized. There is no governing body OptionBlox needs to rely on, as long as Stellar has users, OptionBlox will function.
- *[Anchors](https://www.stellar.org/developers/guides/concepts/assets.html)*  
Stellar has a multi-asset functionality called anchoring that enables users to create custom assets on its ledger and tie them to real-world assets. OptionBlox uses this to tokenize derivatives and to write derivatives involving any asset.  
- *Flexible Transaction System*:  
Stellar has a flexible transaction system that allows us to create derivatives and make them trust-free, tradeable, and safe.  
- *[Turing Signing Servers](https://github.com/tyvdh/turing-signing-server)*:\
The Stellar Community is currently discussing implementing a new ecosystem feature called Turing Signing Servers. These are a decentralized network of servers that hold uploaded smart contracts that are associated with private keys. The servers will sign transactions with these private keys if the transactions meet the specifications of the contracts. OptionBlox will use this tool to manage some of the business logic surrounding contract execution and closure. However, if this feature is not implemented OptionBlox will simply use an open-source repository to manage execution business logic.

[Stellar's website](https://stellar.org/developers)

### OptionBlox's Derivative Protocols:
OptionBlox features a range of tradeable decentralized derivative products
##### Covered Options
OptionBlox covered options are created using a network of accounts and TSS(Turing-Signing-Server) smart contracts. This protocol is based completely on Stellar's network and can operate without any input besides users submitting transactions. These options are American style meaning they can be exercised at any time before expiration.

Below is a basic model showing the writing, sale, and exercise processes of a covered call with an underlying of 1 Bitcoin(BTC), and a strike price of 1000 Lumens(XLM).

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/CoveredOptions(whitepaper)-(v2).png "Covered Options")

##### Uncovered Options
OptionBlox uncovered options are similar to OptionBlox covered options. The key differences are the holding account also serves as a margin account for the seller and the execution process differs slightly.

Below is a model showing the writing, sale, and execution process of an uncovered call. The call contract's underlying is 1 BTC, its strike price is 100 XLM, the initial margin requirement is 15%, and the minimum margin requirement is 10%. These options are American style.

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/UncoveredOptions(whitepaper)-noexample.png "Uncovered Options")

##### Futures
OptionBlox futures also operates using a network of accounts and TSS contracts. Instead of using derivative tokens, the futures protocol issues tokens for the underlying asset, so a party who enters a contract with an underlying of 100 XLM would receive 100 XLMFUTURE tokens. Contract parties exchange these tokens to enter a futures contract; the price they exchanged tokens at represents the spot rate the future is entered at. OptionBlox settles futures daily using a [mark-to-market](https://www.cmegroup.com/education/courses/introduction-to-futures/mark-to-market.html] system.

Below is a basic model showing the writing, sale, execution, and exit of a 100XLM:1BTC future with a 15% initial margin requirement and a 10% minimum margin requirement.

*Diagram is currently under revision*

##### Forwards
We have an internal forwards protocol we plan to implement in the future. It is a modified version of the OptionBlox futures protocol.

##### Swaps
We have an internal swaps protocol we plan to implement in the future. It is a modified version of the OptionBlox futures protocol.

#### Protocol Details

##### Contract Sizing
Contract sizes are standardized. This means that options and futures contracts have uniform underlying amounts. For example, all Ethereum options and futures will have an underlying of 1 ETH. This standardization helps maintain contract volume.

##### Partial Contracts
Tokenizing derivatives allows OptionBlox users to write partial derivative contracts. Users can write and sell fractions of contracts and they will just be sent an equivalent portion of the contract token(s). This is crucial to maintain standardized contract sizes but allow users with less capital to still utilize the derivatives ecosystem.

##### Liquidation Prodecures
OptionBlox uncovered options and futures require position liquidation when the position holders become delinquent in meeting their margin requirements or fail to provide the necessary underlying to complete contract settlement. In these situations, the protocol will attempt to liquidate positions on the Stellar DEX. However, if low volume makes this impossible, OptionBlox uses a TSS managed liquidity pool to liquidate the contracts. 

![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/UncoveredOptionLiquidation(whitepaper)-(v2).png "Insufficient Margin Liquidation (option)")
![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/FuturesNoUnderlying(whitepaper)-(v2).png "Insufficient Underlying(future)")

The OptionBlox liquidity pool is made up of user-provided funds and managed by a TSS contract. Users will receive tokens in exchange for the funds they contribute, the tokens represent their contribution and govern the percentage of liquidation profits they receive. Because of the margin requirements for OptionBlox contracts, it will never be in the position holder's economic interest to allow liquidation, and there will always be an economic incentive to liquidate the position. Profits from liquidating delinquent positions will be paid out to liquidity providers every week. 

### The OptionBlox App:
The OptionBlox team is currently developing web and mobile applications to allow all parties to easily use the OptionBlox protocol. This app will act as a platform that interfaces with the Stellar, OptionBlox, and user wallets to provide user-freindly derivative writing, trading, and execution experience. The app does not run orderbooks, pair buyers and sellers, issue securities, or serve as custodian over user funds or keys. It simply serves as a browser that enables users to easily interact with OptionBlox and Stellar.

### Security:

OptionBlox uses a variety of Stellar's features to ensure that derivatives and margin accounts associated with the protocol are secure.

- *Turing Signing Server Protocol*:\
The TSS protocol provides OptionBlox with a method of adding complex business logic to transactions without requiring our organization to have control over the accounts involved in the transactions. This further decentralizes OptionBlox without reducing efficiency.\
[More Info](https://github.com/tyvdh/turing-signing-server)

- *Locking Accounts*:\
In most OptionBlox protocols, collateral holding accounts add TSS contracts as signers then lock themselves. This ensures that the only transactions they can post in the future are ones approved by the contracts. This security measure locks funds in collateral holding accounts until contract exercise or expiration.  
[More Info](https://www.stellar.org/developers/guides/concepts/multi-sig.html)

- *Timebound Transactions*:  
In all OptionBlox protocols, timebound transactions are used in the closing process to ensure certain transactions cannot be submitted early. Submitting some transactions early would disrupt the exercise process.  
[More Info](https://www.stellar.org/developers/guides/concepts/multi-sig.html)

- *Stellar Consensus Protocol*  
Stellar's consensus protocol rejects transactions when they do not align with the correct ledger state. For example, a user could not fill a sell offer if their account lacked the necessary funds.  
[More Info](https://www.stellar.org/developers/guides/concepts/scp.html)  

- *Account Flags*  
  - *Authorization Required Flag*:\
  OptionBlox uses the authorization required flag for some custom derivative facilitation tokens it issues. This ensures that only users that should be allowed to hold certain tokens can hold the tokens.
  - *Authorization Revokable Flag*:\
  OptionBlox uses authorization revokable flags in combination with authorization required flags to allow accounts to hold custom tokens used for derivative facilitation only during certain transactions.\
[More Info](https://www.stellar.org/developers/guides/concepts/accounts.html#flags)

- *SEP-0007 Integration*:\
The OptionBlox app will use Stellar's SEP-0007 protocol to send transaction envelopes to users who can then add their signature in a trusted wallet or exchange. This ensures that the app will never serve as custodian over user funds or keys.\
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
- DSTOQ: Equities anchored on Stellar by [DSTOQ](https://dstoq.com).

More anchors can be viewed on [StellarX](https://www.stellarx.com/markets)

As Stellar's network grows we are confident that more anchors will materialize and expand OptionBlox's functionality.

### Roadmap
1. *Q3 2020*
- Finalize Backend Demo
- Finalize Web-App Demo
- Continue Application Development
- Expand Engineering Team
- Begin Seed Funding Search
- Explore Wallet Parnerships
 2. *Q4 2020*
   - Finalize Website
   - Continue Application Development
   - Expand Fundraising Efforts
   - Launch Advisory Board
   - Explore Further Ecosystem Partnerships
 3. *Q1 2021*
   - Roll-out Full Demo/Alpha
     - Functional Testnet Application
   - Explore Market Maker Partnerships
 4. *Q2 2021*
   - Launch Open-Beta for Covered Options
   - Launch Closed Alpha for Uncovered Options and Futures
   - Launch Closed Alpha for OTC contract development tool
   
### Glossary
Terms:  
- *Smart Contract:* A protocol to digitally facilitate, verify, or enforce the performance of a contract.  
- *Keypair:* When an account is created on Stellar's ledger, it is assigned a public and a private key. The private key is used to sign transactions and the public key is used to identify the account. These two keys make up the account's keypair.
- *Underlying:* The asset a derivative contract governs. This is what the contract's value is based on. In the case of a call option that gives the owner the right to buy Ethereum, the contract underlying would be Ethereum. 
- *Hedging:* Hedging is a term for making an investment that reduces the risk of another investment.
