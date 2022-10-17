# The DeFi stack

* Before we can understand what causes hacks, we need to understand where hacks can happen so we'll start by proposing a framework for the DeFi value chain called "the defi stack."
* The DeFi stack tracks the flow of funds from a user's non-crypto holdings all the way to their final DeFi position
* The layers of the stack
	- Self custody layer
		+ Onramps
		+ Key management
	- Infrastructure layer
		+ Wallets
		+ DNS providers
		+ Data indexers
		+ Private key generators
	- Transaction layer
		+ Smart contract language
		+ Consensus 
	- Protocol layer
		+ Security
		+ Governance
		+ Risk management
	- Ecosystem layer
		+ Oracles
		+ Assets
* Anatomy of a transaction
	- User buys crypto with a credit card using an onramp
	- That crypto goes to an address in a wallet they created using a popular wallet application, they save their private keys somewhere
	- The user goes to the website of the application they want to use, the contents of that app are served by DNS provider
	- The contents of the app are populated from an data indexer
	- The user navigates to the relevant page in the app and goes to deposit assets
	- They're asked to approve the contract to spend their assets
	- They deposit their assets into the contract by transferring their assets from their address to the contract using, facilitated by the transaction layer they're using
	- Those assets are now exposed to the rules of the smart contracts and all things that can impact the rules of the smart contracts at the protocol layer
	- They are also exposed to failure in the protocols ecosystem dependencies like oracle failures or asset failures
* A failure at any stage of this process could lead to loss of funds. Let's find out how. 