# Self custody

Taking custody of your own crypto assets (self custody) exposes you to total loss of your crypto assets. In this post, we'll apply the [*Opsec Framework*](https://opsec101.org/) to self custody and answer the following five questions:

1. What needs protecting
2. What is the potential threat
3. What are the potential vulnerabilities
4. What is the potential riks
5. What are the countermeasures

After reading this guide, you should understand how your funds can be lost and how to protect yourself from those potential losses. 

## What needs protecting

The contents of your wallet--cryptocurrencies, tokens, NFTs--need protecting.

Note: centralized exchange out of scope for this guide because it's not self custody

## What is the potential threat

Losing or compromising access to your crypto wallet is permanent. There's no company or government that can reliably get your assets back. This is a critically important difference to checking, savings, and trading accounts in traditional finance. 

There are two types of potential threat:

1. You lose access
2. An attacker gains access

If you lose access, nobody can help you recover your wallet. There's no phone number to call or account reset flow. 

If an attacker gains access, nobody can take it away from them. This means they can irreversibly transfer all of your assets to an address that only they control. 


## What are the potential vulnerabilities

### How you can lose access to the assets in your wallet

* Forget to back-up private key
	- When you set up a new wallet, you'll be asked to back up your private keys. 
	- If you lose access to your wallet (e.g. forget metamask password, lose your hardware wallet), you'll be able to restore it by using your private keys. 
	- If you lose access to your wallet *and* your private keys, your funds are gone forever. 
* Lose your back-up private key
	- When you back-up your private key, you need to make sure it's secure and recoverable
	- You can lose your funds by discarding, destroying, or forgetting your back-up
	- Discarding means you backed up your keys but threw the back-up away (e.g. a notebook that got discarded during spring cleaning, here's a guy who [lost hundreds of millions](https://www.cnbc.com/2021/01/15/uk-man-makes-last-ditch-effort-to-recover-lost-bitcoin-hard-drive.html) by throwing out a hard drive with his private keys)
	- Destroying means your back-up failed to survive the elements. For example, a back-up written on paper being burned in a fire
	- Forgetting means you backed up your keys but no longer know where the back-up is
* Die without sharing private key back-up
	- Your funds can be lost if you die and don't prepare a way for your loved ones to recover your wallet
	
What to do when you lose your private keys? If you still have access to your wallet, create a new wallet, make sure sure you back-up your private keys, and transfer all of your assets from your old wallet to your new wallet. 

### How an attacker can gain access to your wallet

* Reveal private key
	- Storing your private key encrypted on your device and opening an infected file that installs a virus that sends the encryptoed file to the hacker
	- Entering your private key into a fraudulent website
	- Revealing a recovery QR code (usually over video chat with fraudulent "support" call)
	- Using an insecure private key generator that allows an attacker to brute force generate your private key (example: [profanity](https://halborn.com/explained-the-profanity-address-generator-hack-september-2022/))
* Permit asset transfer
	- Signing a fraudulent transaction that gives the attacker permission to transfer your assets (most commonly on a fraudulent site that pretends to be an official site offering an airdrop or mint or on a compromised official site)
	- Approving a legitimate contract to transfer your funds that has a security vulnerability that allows an attacker to transfer your funds to their address 
* Hijacking destination address of transfer
	- Adding a malicious browser extention that replaces your intended address with the attacker's address when you use the clipboard (e.g. 0x123 to 0xabc)
* Physical attack ("wrench attack")
	- An attacker physically attacks or threatens you for access to your wallet
	
What to do when you think an attacker has gained access to your wallet? If you revealed your private key, create a new wallet and transfer any remaining assets to the new wallet. If you permitted asset transfers, visit revoke.cash to remove the permissions. 


## What is the potential risk

If you lose or compromise your private keys, you stand to lose all of the assets in your wallets. If you permit asset transfers, you stand to lose all of the asset type your permitted the transfer of. 

* seed phrase compromise: everything
* fraudulent permit: the asset(s) you permit from that address
* physical attacks: your life or the lives of loved ones

## What are the countermeasures

(to be fleshed out)

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

## Summary and next steps

(to be fleshed out)