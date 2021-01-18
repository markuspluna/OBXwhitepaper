## Derivatives Overview
We will briefly give an explanation of financial derivatives to help give context to OptionBlox. A derivative is a financial contract between two parties. Its value is based on an agreed-upon asset or a set of assets. The most common forms of financial derivatives are futures and options.
### Futures
Futures are contracts between two parties to buy/sell an agreed-upon quantity of an asset, called the underlying asset, for a set price at an established future time. Common uses of futures are to hedge against price movement by the underlying asset, increase leverage, and gain exposure to rates.\
\
**Sample Futures Use Case Supported by OptionBlox:**
1. *Hedging*\
A gold miner knows that they will be selling 6000 kilos of gold in 6 months. 1 kilo of gold is currently worth $1000. The miner does not want to risk gold prices falling in the next 6 months, so they enter a futures contract to sell 6000 kilos of gold for $6,000,000 in 6 months. This “locks in” the current price of gold for them and allows them to continue their operations without any risk of prices falling.

### Options
Options are contracts between two parties, a writer and a buyer. The contract gives the buyer the option, but not the obligation, to buy or sell an asset at an agreed-upon price until the option expires. If the buyer decides to exercise this right, the option writer will fulfill the buyer's purchase or sale. Options can be either puts or calls. A call option allows its owner to buy the underlying asset at the agreed-upon "strike price." A put option allows its owner to sell the underlying asset at the strike price. Common uses of options are hedging, increasing leverage, and income generation.\
 \
**Sample Options Use Cases Supported by OptionBlox:**
1. *Investing*\
Adam wants to invest in 1000 XLM but doesn't want to hold the XLM; he only wants to be exposed to the position's upside. Using a decentralized exchange, he purchases a XLM call option contract with a strike price of $100. Until it expires, the contract gives Adam the option to purchase 1000 XLM for $100. If the price of XLM increases to $0.20, he can exercise his option contract and purchase 1000 XLM for $100. Since, based on the new market price of $0.20, 1000 XLM is worth $200, he will receive the same returns he would receive if he had originally purchased 1000 XLM at $0.10. Thus, purchasing the contract allows Adam to gain exposure to the upside of investing in 1000 XLM without having to purchase and hold the cryptocurrency.
2. *Hedging*\
Latera holds a number of THUMB LLC shares but is concerned about share price volatility. To mitigate volatility risk, he decides to purchase a put option contract guaranteeing him the option to sell 100 THUMB shares for $10,000 ($100/share) until the contract expires in 1 year. This contract protects him from any potential decline in the market value of THUMB LLC.
3. *Passive Income Generation*\
Carlos owns 1 BTC and plans to hold it until it reaches his price target of $60,000. However, he would like to earn some passive income with his invested capital. He sells a Bitcoin call contract with a strike price of $100,000 for $100. This strategy allows him to continue to hold his Bitcoin until it hits his price target while earning additional capital with his investment. Even better, the contract is only valid until it expires. If it is not exercised and expires, he can sell another call contract using his Bitcoin holdings as the underlying. 
 
## OptionBlox Overview
Optionblox is a platform and DeFi protocol that enables users to write, trade, and execute financial derivatives using Stellar. The derivative contracts are fully ledger-based; margin and underlying balances are stored on-ledger, and Turing Signing Server smart contracts enforce the derivatives. OptionBlox uses DLT based derivatives to drive improvement in derivative ecosystem accessibility, efficiency, and flexibility. The pillars of our offering are:
 
### OptionBlox Pillar 1: Efficiency  
The incumbent derivatives market suffers from a large amount of friction. It requires market intermediaries to provide access to the market, facilitate trades, and lower counterparty risk. These additional parties cause inefficiency, which creates costs that get passed on to investors. By facilitating derivatives on Stellar, OptionBlox eliminates the need for market intermediaries. The diagrams below illustrate the efficiency gained from eliminating market intermediaries by comparing the traditional derivative ecosystem’s post-trade process with Optionblox’s post-trade process.
 
**Financial Transaction Processing Comparison**\
![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/post-trade%20processing%20comparison.jpg "Post-Trade Processing Comparison")
> Citation: ISDA. "The Future of Derivatives Processing and Market Infrastructure". ISDA Whitepaper. 2016. DOI= https://www.isda.org/2016/09/15/the-future-of-derivatives-processing-and-market-infrastructure/
 
A research paper that covered Stellar-based financial derivatives measured the monetary impact of their efficiency improvements. The paper delved into efficiency gains in both transaction processing and data accessibility. Data accessibility is a huge source of cost and inefficiency in the traditional derivatives ecosystem. Additionally, the paper measured costs associated with Ethereum based financial derivatives to demonstrate Stellar’s efficiency advantage in the DeFi ecosystem. The results of the research paper are shown in the tables below.\
 \
**Ecosystem Fees Associated with Stellar Based Derivatives**
|Writing and Executing Options|Writing and Executing Futures|Writing and Executing Swaps|Trading all Derivatives|
|---|---|---|---|
|$0.000261|$0.000319|$0.0004234|$0.000029|
 
**Ecosystem Fees Associated with the Traditional Derivative Ecosystem**
|CBOE Options|CBOE Futures|CME Derivatives|
|---|---|---|
|$0.235|$1.759|$0.725|
 
**Ecosystem Fees Associated with Ethereum Based Derivatives**
|Writing and Executing Derivatives|Trading all Derivatives|
|---|---|
|$5.50+|$1.10+|
 
**Live Data Fees by Ecosystem**
|Stellar Ecosystem Data Fees|Traditional Ecosystem Live Data Fees|Ethereum Ecosystem Data Fees|
|---|---|---|
|$0|$105/month|$0|
> Citation: Paulson-Luna, Riley. "The Financial Derivatives Ecosystem is Old - Decentralized Ledger Technology is its Fountain of Youth". 2020. ASSE 2020.DOI = https://dl.acm.org/doi/abs/10.1145/3399871.3399904


We expect these gains in efficiency to exponentially increase when it comes to OTC(Over-The-Counter) derivatives. OTC contracts are highly specified, complicated, and can carry a large amount of counterparty risk. Traditionally, a party that wants to enter an OTC contract must find both a counterparty and a facilitating party. OptionBlox's protocol eliminates the need for the facilitating party and makes it easier to find a counterparty by improving ecosystem accessibility. As a result, OptionBlox significantly improves OTC derivative efficiency and accessibility.

 
### OptionBlox Pillar 2: Flexibility  
OptionBlox provides unparalleled flexibility, allowing users to accomplish any derivative use case. If OptionBlox’s standardized derivatives do not meet users' needs, Optionblox enables them to write OTC derivatives with custom contract specifications. Additionally, derivatives written with OptionBlox use Stellar’s [Anchor](https://www.stellar.org/developers/guides/concepts/assets.html) system to manage contract underlying assets. Since the Anchor system supports any asset, our contracts also support any asset.
 
- *Tokenized Derivatives*:  
OptionBlox also uses the Anchor system to tokenize derivative contracts, which is essential in the DLT(decentralized ledger technology) space. Tokenization allows our derivatives to be traded on any cryptocurrency exchange and stored anywhere. A derivative writer could write a derivative on our platform, then transfer it to their Binance account and sell it on their market. A derivative buyer could take their newly purchased derivative tokens and transfer them to their Ledger Nano S for added security. This flexibility is essential due to the fragmentation of the DLT space. It also serves to decentralize OptionBlox further. In addition to improving trading and storage flexibility, tokenization allows users to write partial derivatives. This enables users with different levels of wealth to use derivatives while still allowing OptionBlox to retain standardized derivative sizes. For example, our Ethereum options are standardized to have an underlying of 1 ETH to preserve contract volume. If a user wants to write an ETH option but cannot provide the entire 1 ETH underlying, our partial derivative capability allows them to write a fractional derivative. They can provide us with a fraction of 1 ETH as their contracts underlying and receive a proportional fraction of an ETH option token.

 
 ![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/OBX%20flexibility.png "Flexibility Graphic")

 
### OptionBlox Pillar 3: Accessibility
OptionBlox uses DLT to make huge improvements in derivative ecosystem accessibility. The decentralized nature of our system means OptionBlox is accessible to anyone with an internet connection. This is a huge improvement over the derivatives ecosystem's current state, where only a small portion of the world has efficient ecosystem access. The incumbent derivative ecosystem’s dependence on central parties makes it impossible for it to serve a wider market. Since OptionBlox uses DLT to facilitate derivatives instead of central parties, it does not suffer from these limitations and can truly enable global equitable access to the derivatives ecosystem. 
 
### OptionBlox Pillar 4: Useability
We’re building OptionBlox for users of all types, from experienced traders to new users in developing countries. As such, UI/UX excellence is paramount for us. However, financial inclusion doesn’t just mean throwing an app at someone in a developing country and having them figure it out. Education is crucial to truly working towards financial inclusion. Our approach to a user-friendly interface not only involves simple and sleek controls, but also focuses on educating our users about financial derivatives.


## Platform/Protocol Overview
OptionBlox serves as a tier-3 blockchain app, a layer between users and the Stellar ledger. Users link their wallets to our web-app to write, trade, or execute derivative contracts. The OptionBlox web-app takes user inputs and communicates them to the OptionBlox protocol, which uses TSS(turing signing server) smart contracts to build Stellar transactions that carry out the users’ commands. Users approve these transactions with their wallet and receive the result of their transaction, whether that’s derivative tokens, sale proceeds, or underlying assets.


For more technical details regarding how our protocol and TSS smart contracts function, see our whitepaper: https://github.com/markuspluna/OBXwhitepaper/blob/master/Whitepaper.md


### High-Level Protocol Overview

 ![alt text](https://github.com/markuspluna/OBXwhitepaper/blob/master/photos/High-Level%20OBX%20protocol.png "OBX Protocol")
 
### OptionBlox User Journey
1. User links their wallet on the OptionBlox home page\
2. User clicks XLM card to navigate to XLM option market page\
3. User selects XLM option at one strike price (.20) and selects to sells it [they should get a popup saying a request has been sent to their wallet for them to approve]\
User selects a different XLM strike price (.15) and buys it [they should get a popup saying a request has been sent to their wallet for them to approve]\
User navigates to their wallet page and executes their XLM option (.15 strike price) [they should get a popup saying a request has been sent to their wallet for them to approve]\
 
 ### Note on Turing Signing Servers
The TSS(turing signing server) system is an SDF solution that enables turing complete smart contracts on Stellar. TSS smart contracts are a valuable part of the OptionBlox protocol as they ensure the security, trustworthiness, and decentralization of the protocol. However, the OptionBlox team is aware that the TSS solution is currently in its proposal stage. We are optimistic about its future and believe it will be fully implemented into the Stellar ecosystem. However, if the proposal fails, OptionBlox can pivot to function without TSS smart contracts, as it was originally designed before the TSS solution existed.

For more information on turing signing servers see: https://tss.stellar.buzz/
 
## Motivation for OptionBlox


### Equitable Access to Financial Derivative Markets
Decentralized Ledger Technology enables the disruption of the incumbent financial ecosystem that suffers from inefficiency and fails to serve so much of the world. In traditional financial markets, wealth comes with better market access and cheaper pricing. Financial derivative markets are especially prone to this effect; a study published by the IMF showed that more sophisticated parties receive significantly better prices in derivative markets. With OptionBlox, we strive to even the playing field. Whether users are hedge funds or farmers in Venezuela, OptionBlox will enable them to utilize any derivative and give them holistic access to global derivatives markets.\
 \
Equitable access to efficient derivative markets is crucial to attaining global economic equality and fostering global economic growth. This was shown by a study published in the Journal of Risk and Financial Management. The study found that financial derivatives serve as hedging tools for businesses and help drive market efficiency. We hope that by creating equitable access to financial derivatives, OptionBlox can help foster economic growth across the globe.
 
> Citation: Hong Vo, Duc; Van Huynh, Son; The Vo, Anh; Thi-Thieu Ha, Dao. “The Importance of the Financial Derivatives Markets to Economic Development in the World’s Four Major Economies.” Journal of Risk Financial Management. 2019. DOI= https://www.mdpi.com/1911-8074/12/1/35  

> Citation: IMF. “Discriminatory Pricing of Over-the-Counter Derivatives.” 2019. IMF. DOI = https://www.elibrary.imf.org/view/IMF001/25871-9781498303774/25871-9781498303774/25871-9781498303774_A001.xml?redirect=true
 
 
### The Derivative Ecosystem is Ripe for Innovation
The current derivative ecosystem is inefficient. Writing and executing contracts costs 1000X more than what is technologically possible. The incumbent ecosystem is held back by middlemen that add unnecessary friction. In the incumbent ecosystem, a single derivative contract involves not only the contract parties, but also a derivatives exchange, a central clearing party, and a derivatives broker. These middlemen exist to lower counterparty risk and match buyers and sellers. OptionBlox uses Stellar to accomplish these directives, removing the need for middlemen. This significantly lowers ecosystem costs and increases efficiency. 


Despite the incumbent ecosystem’s inefficiency, volume in options has been increasing in retail spaces like on Robinhood and other platforms, showing the increasing demand for derivative products. We expect these numbers to continue increasing due to expanding market accessibility, of which OptionBlox will be at the forefront. OptionBlox will compete in the current market with our higher efficiency and capture the expanding market with improved accessibility. Overall, OptionBlox drives necessary innovation in the derivatives ecosystem. It is bringing efficiency in line with what is technologically possible and improving accessibility and flexibility to meet the needs of an expanding derivatives market.
 
## Business Details
### Monetization
OptionBlox will monetize through premium market analytics features and market-maker data services. We do not charge fees to use our protocol. 
### Roadmap
The OptionBlox team hopes to use resources gained from the Stellar Seed Fund to launch and expand OptionBlox. Below is a list of goals, beyond launching OptionBlox, that these resources will help us accomplish.
1. *Expand the OptionBlox Team*\
To properly support OptionBlox, we want to expand our team to include additional development, business, and legal resources.
2. *Tier-1 Validator*\
Given OptionBlox’s high level of interaction with Stellar and Horizon, we want to become a tier-1 network validator. 
3. *Mobile Application for OptionBlox*\
  Our team believes that to properly serve users in developing countries, we need to launch a mobile application.\
4. *OptionBlox Hedging Tool*\
  To help the Stellar Community fully utilize derivatives, we want to create a tool that will help OptionBlox users calculate the best way to hedge their portfolios using derivatives.
5. *OptionBlox Yield Pools*\
  Selling covered options is a great way to generate passive income using your investments. However, it is often over-complicated and difficult. We hope to develop OptionBlox yield pools where users can easily stake their holdings to generate yield by writing options.
  ## YieldBlox – a Future OptionBlox Initiative
The OptionBlox team is currently developing a decentralized loan protocol powered by Turing Signing Servers. This protocol will allow asset holders on Stellar to lend out their assets and receive interest payments from borrowers. It will be structured as a combination of DAI and Compound. We are excited to share more details about this project as it gets further along in development.

