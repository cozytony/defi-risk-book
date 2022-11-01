# Self custody

Taking custody of your own crypto assets (self custody) exposes you to total loss of your crypto assets. In this post, we'll apply the opsec framework to self custody and answer the following five questions:

1. What needs protecting
2. What is the potential threat
3. What are the potential vulnerabilities
4. What is the potential riks
5. What are the countermeasures

After reading this guide, you should understand how funds can be lost and how to protect yourself from those potential losses. 

## What needs protecting

The contents of your wallet--cryptocurrencies, tokens, NFTs--need protecting.

Note: centralized exchange out of scope for this guide because it's not self custody

## What is the potential threat

Losing or compromising access to your crypto wallet is permanent. There's no company or government that can reliably get your assets back. This is a critically important difference to checking, savings, and trading accounts in traditional finance. 

There are two ways to lose access:

1. You lose access
2. An attacker gains access

If you lose access, nobody can help you recover your wallet. There's no phone number to call or account reset flow. 

If an attacker gains access, nobody can take it away from them. This means they can irreversibly transfer all of your assets to an address that only they control. 


## What are the potential vulnerabilities

How you can lose access to your wallet

* Forget to back up private key
* Forget location of private key back-up
* Die without sharing private key back-up
* Destroy private key back-up
* Discard private key back-up

How an attacker can gain access to your wallet

* Reveal private key
	- Storing your private key encrypted on your device and opening an infected file that installs a virus that sends the encryptoed file to the hacker
	- Entering your private key into a fraudulent website
	- Revealing a recovery QR code (usually over video chat with fraudulent "support" call)
* Permit asset transfer
	- Signing a fraudulent transaction that gives the attacker permission to transfer your assets (most commonly on a fraudulent site that pretends to be an official site offering an airdrop or mint or on a compromised official site)
	- Approving a legitimate contract to transfer your funds that has a security vulnerability that allows an attacker to transfer your funds to their address 
* Hijacking destination address of transfer
	- Adding a malicious browser extention that replaces your intended address with the attacker's address when you use the clipboard (e.g. 0x123 to 0xabc)
* Physical attack ("wrench attack")
	- An attacker physically attacks or threatens you for access to your wallet


## What is the potential risk

Either everything, or one thing

* seed phrase compromise: everything
* fraudulent permit: the asset(s) you permit from that address
* physical attacks: your life or the lives of loved ones

## What are the countermeasures

Lose
* PK storage best practices
* Recovery best practices

Give away
* Hardware wallet
* Seed generator
* Verify transactions
* Check permissions revoke.cash
* Segregate accounts
* Be inconspicuous (general opsec guides apply here)