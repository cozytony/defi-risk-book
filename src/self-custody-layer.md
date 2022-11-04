# Self custody

Taking custody of your crypto assets (self custody) offers unprecedented control of your financial property but comes with the unprecedented risk of losing your stuff. In this post, we'll apply the [*Opsec Framework*](https://opsec101.org/) to self custody and answer the following five questions:

1. What needs protecting
2. What is the potential threat
3. What are the potential vulnerabilities
4. What is the potential risk
5. What are the countermeasures

After reading this guide, you'll know how to enjoy the benefits of self custody while keeping your stuff safe. 

## What needs protecting

The contents of your crypto wallet--cryptocurrencies, tokens, NFTs--need protecting[^1].


## What is the potential threat

Losing or compromising access to your crypto wallet is permanent.

There are two types of potential threat:

1. You lose access
2. An attacker gains access

If you lose access, nobody can help you recover your wallet. There's no phone number to call or account reset flow. 

If an attacker gains access, nobody can take it away from them--they'll be able to irreversibly transfer all of your assets to their own address. 

## What are the potential vulnerabilities

### How you can lose access to the assets in your wallet

**Forget to back-up seed phrase**

When you set up a new wallet, you'll be asked to back up your seed phrase keys. If you lose access to your wallet (e.g. forget metamask password, lose your hardware wallet), you'll be able to restore it by using your seed phrase. And if you lose access to your wallet *and* your seed phrase, your funds are gone forever. 

**Lose your back-up seed phrase**

When you back-up your seed phrase, you need to make sure it's secure and recoverable.

You can lose your funds by discarding, destroying, or forgetting your back-up. 
* Discarding means you backed up your keys but threw the back-up away (e.g. a notebook that got discarded during spring cleaning, here's a guy who [lost hundreds of millions](https://www.cnbc.com/2021/01/15/uk-man-makes-last-ditch-effort-to-recover-lost-bitcoin-hard-drive.html) by throwing out a hard drive with his seed phrase).
* Destroying means your back-up failed to survive the elements. For example, a back-up written on paper may not survive a fire.
* Forgetting means you backed up your keys but no longer know where the back-up is.

**Die without sharing seed phrase back-up**

Your funds can be lost if you die and don't prepare a way for your loved ones to recover your wallet.
	
**What to do when you lose your seed phrase?** 

If you still have access to your wallet, create a new wallet, make sure sure you back-up your seed phrase, and transfer all of your assets from your old wallet to your new wallet. 

### How an attacker can gain access to your wallet

**Reveal seed phrase**

- Storing your seed phrase encrypted on your device and opening an infected file that installs a virus that sends the encrypted file to the hacker
- Entering your seed phrase into a fraudulent website
- Revealing a recovery QR code (usually over video chat with a fraudulent "support" call)
- Using an insecure seed phrase generator that allows an attacker to brute force generate your seed phrase (example: [profanity](https://halborn.com/explained-the-profanity-address-generator-hack-september-2022/))

**Permit asset transfer**

* Signing a fraudulent transaction that gives the attacker permission to transfer your assets (most commonly on a fraudulent site that pretends to be an official site offering an airdrop or mint or on a compromised official site)
* Approving a legitimate contract to transfer your funds that has a security vulnerability that allows an attacker to transfer your funds to their address 

**Hijacking destination address of transfer**

* Adding a malicious browser extension that replaces your intended address with the attacker's address when you use the clipboard (e.g. 0x123 to 0xabc)

**Physical attack ("wrench attack")**

* An attacker physically attacks or threatens you for access to your wallet
	
**What to do when you think an attacker has gained access to your wallet?** 

If you revealed your seed phrase, create a new wallet and transfer any remaining assets to the new wallet. If you permitted asset transfers, visit revoke.cash to remove the permissions. 


## What is the potential risk

If you lose or compromise your seed phrase, you stand to lose all of the assets in your wallets. If you permit asset transfers, you stand to lose all of the asset type for which you permitted transfers. 

* seed phrase compromise: everything
* fraudulent permit: the asset(s) you permit from that address
* physical attacks: your life or the lives of loved ones

## What are the countermeasures

**Best practices for storing your seed phrase back-up**

Your seed phrase back-up should be safe from destruction, discarding, forgetting, death, and both physical and digital theft. 

* Destruction: instead of paper, consider using stainless steel. This will give your back-up a better chance of surviving time and natural disasters like fire. 
* Discarding: store your back-up somewhere it won't be mistaken for trash. Like a safety deposit box or a fire-proof safe. 
* Unforgettable: store your back-up somewhere you won't forget it. 
* Death: leave instructions for your loved ones to recover your address in case of your unexpected death. But make sure the instructions don't compromise the security of your back-up while you're living.
* Physical theft: minimize the likelihood of being targetted by keeping a low profile. 
* Digital theft: store your back-up offline, either on a physical medium or on an air-gapped computer (meaning it never connects to the internet).

**Best practices for securing your wallet from attackers**

When you use your wallet, you must do it in such a way that makes it difficult or impossible for attackers to hijack your asset transfers, insert fraudulent transfer permissions, or trick you into revealing your seed phrase. 

* Hardware wallet: a hardware wallet is highly recommended if you are storing greater than a few hundred dollars worth of assets. It will ensure your seed phrase was generated securely and adds a second layer of defense against any and all transactions by requiring physicial confirmation of transactions using the hardware wallet. 
* Seed generator: avoid third party seed phrase generators when possible. There have been large hacks due to insecure seed phrase generators like the [Profanity hack](https://rekt.news/wintermute-rekt-2/).
* Verify transactions: double check that all of your transactions are as you expect before submitting them. Popular wallets like Metamask don't make it easy but there are tools [like blowfish](https://blowfish.xyz/) that are working on making this easier. 
* Check and manage permissions: periodically review your permissions on a site like [revoke.cash](https://revoke.cash/) to make sure the contracts that have permission to transfer your assets should have permission.
* Segregate accounts: when possible, use separate addresses for separate use cases. So if one of your addresses is compromised, you can isolate the damage to just the assets in that address. 
* Never give out your seed phrase: a common tactic of attackers is to come up with a convincing reason that you need to enter your seed phrase on their fraudulent website to either recover your account or claim some reward. As a general rule, you should never ever enter your seed phrase anywhere. 

## Summary and next steps

Choosing self-custody is empowering but comes with great responsibility. You will need to protect your funds from threats like losing or compromising access to your wallets by carefully managing your seed phrase back-ups and exercising extreme caution when using your wallet. Luckily, there are best practices you can take advantage of to reduce your risk. And better and better countermeasures are being released every year. 

Keep tabs on this post for the latest developments on how to self-custody safely.  

[^1]: Centralized exchanges are out of scope for this guide because it's not considered self custody