---
layout: post
title: Comment on FinCEN response
subtitle: Why MPWG supports rule change
cover-img: https://moneropolicy.org/assets/img/pexels-burst-374103.jpg
thumbnail-img: https://moneropolicy.org/assets/img/pexels-burst-374103.jpg
share-img: https://moneropolicy.org/assets/img/pexels-burst-374103.jpg
gh-repo: monero-policy/monero-policy.github.io
gh-badge: [star, fork, follow]
tags: [fincen, unhosted]
comments: true
---

On December 18th 2020, the Financial Crimes Enforcement Network (FinCEN) issued a proposal for a new set of rules for certain digital currency transactions. More specifically, the rules set out to impose new reporting, recordkeeping, and identity verification requirements upon banks and Money Services Businesses (MSBs) for certain transactions involving what is termed "unhosted" (self-custodied) wallets. On January 4th, 2021, the Monero Policy Working Group (MPWG) [submitted a response](https://www.regulations.gov/comment/FINCEN-2020-0020-6210) for comment from the perspective of cryptocurrency’s leading privacy preserving project. This blog will serve as another, less formal method of sharing the views of this working group.

**Perhaps surprisingly on the surface, the MPWG *supports* most of these proposed FinCEN changes, unlike most of the cryptocurrency industry.** The MPWG believes that the proposed changes will substantially clear up many of the common (and unnecessary) fears of transacting in specific assets.

The MPWG largely disagrees with the Bank Secrecy Act (BSA) and the Patriot Act, as well as their warrantless collection of sensitive, non-suspicious financial data. Nevertheless, it is unclear why cryptocurrencies would not fall within this data collection, and so long as the lines are blurred, Monero is most likely to be disproportionately harmed by this uncertainty. In our view, accepting clear lines will benefit Monero and reduce overall ML/TF risks.

# Monero is the ugly duckling

Many members of the Monero community have spent years trying to improve the image of Monero. These efforts include supporting the [Perkins Coie “privacy coin” whitepaper](https://www.perkinscoie.com/en/news-insights/anti-money-laundering-regulation-of-privacy-enabling-cryptocurrencies.html), bringing a Monero perspective to [ComplyFirst](https://www.complyfirst.org/), and discussing the importance of privacy behind the scenes. Despite all this, Monero continues to act as a “foil” of sorts for many in the industry. Monero undeservingly acts as the symbol of risk. Exchanges and services use statements in their AML policies such as “we do not trade privacy coins to reduce AML risks” in a feeble attempt to signal compliance. Such statements completely fail to address real ML/TF risks, but Monero’s market capitalization today does not apply enough business pressure on compliance teams to justify even basic action.

For banks, it can be even worse. Even among the cryptocurrency-friendly ones, they often make exchanges justify why they are trading in privacy-preserving cryptocurrencies specifically. Some banks have blanket bans, saying that under no circumstances can their client’s customers ever touch privacy-preserving cryptocurrencies.

Why is Monero the ugly duckling, even among all privacy-preserving cryptocurrencies? To some extent, exchanges use this foil to signal de-risking (ironically at the expense of increasing overall money laundering (ML) and terrorist financing (TF) risks worldwide, discussed later). But the larger reason is that exchanges and regulators have a completely inaccurate misconception that cryptocurrencies intrinsically offer full transaction records to the public. From this general apathy and from these misconceptions, and from accelerated lobbying from blockchain analysis companies perpetuating the false “everything should be public” narrative, most exchanges simply don’t feel comfortable listing assets for which they don’t have a blockchain analysis tool. The MPWG believes that this response is lazy and completely misses the goals of a compliance program. Nevertheless, blockchain analysis is such a deep-rooted assumption that Monero has little chance.

Every respectable exchange uses blockchain analysis. However, it’s an obviously incorrect assumption that these sorts of tools will be available for every technology and cryptocurrency that comes along. Many skilled criminals can stay ahead of the analysis on public networks, and Monero is increasingly used for activities that regulators want to prosecute. By historically relying so heavily on these blockchain analysis tools, regulators are ill-prepared to deal with the challenges that come with the increasing popularity of less-traceable money. Further, exchanges, banks, regulators, and blockchain analysis companies should be aware of the severe negative consequences for financial inclusion if their attributions are incorrect and result in undue discrimination on specific groups.

# CTRs reduce risks with the same strategies applied to cash

Cash ML/TF risks are well-understood since cash has been around for a long time. Cash also shares many properties with Monero: both are private and fungible bearer assets. One can argue that cash is even more private than Monero, since there is no public record of a cash transaction occurring. A Currency Transaction Report (CTR) is required for all deposits exceeding $10,000, among other recordkeeping and reporting requirements.

Mandating recordkeeping and reporting requirements at thresholds equivalent to cash will narrow the compliance gap for cryptocurrencies considerably. There will be far less room to argue that cryptocurrencies (Monero in particular) need some vague concept of further enhanced due diligence when the risks are already quite severely mitigated using existing, proven reporting and recordkeeping requirements.

Many exchanges refuse to support Monero due to the perception of increased risks, despite [many](https://www.perkinscoie.com/en/news-insights/anti-money-laundering-regulation-of-privacy-enabling-cryptocurrencies.html) [resources](https://www.complyfirst.org/resources/) indicating that these risks can be mitigated. This is because most exchanges heavily rely upon blockchain analysis software to mitigate risks. Sadly, this overly conservative, narrow-minded approach restricts their AML capabilities to exclusively transparent coins. We believe that for open, permissionless cryptocurrencies, where any user can attempt to achieve privacy using a variety of any means, solely relying on blockchain analysis as a primary AML tool is severely insufficient for genuine, preventative management of risks. Exchanges will encounter users who ‘mix’ in an attempt to obfuscate the true source of funds, including through less-detectable methods such as PayJoin, even on transparent networks.

Instead, cryptocurrency exchanges should be forced to design compliance programs that adequately address the underlying risks of bearer assets including non-transparent fungible bearer assets. There is an industry delusion that users will always use a transparent means of exchange such that Counterparties of Customers will be known. This is not the case for any other bearer asset, nor should it be; thus, this incorrect assumption holds exchanges back to supporting primitive technologies exclusively. Thus, Monero’s advanced privacy features that make it more similar to other bearer assets result in it being excluded.

Put bluntly, if exchanges are unable, or unwilling, to address AML risks for privacy respecting assets, then they are ill-prepared to address AML risks for other bearer assets. This FinCEN regulation forces these exchanges who have relied too heavily on blockchain analysis tools to design more inclusive AML policies that cover all bearer assets, including Monero.

# Some caveats

While the MPWG largely is in favor of these changes, there are a few important caveats.

First, the recordkeeping and reporting of the “customer’s counterparty” needs to be removed. This is not required of any other asset, including cash.

Second, some industry groups advocate to not include addresses and transaction IDs in the report. We somewhat agree with this view. For Monero, we do not care if Monero transaction IDs are included, because they reveal far more limited information on-chain. However, we understand that Bitcoin and other networks would leak a lot of additional data. We argue that this is Bitcoin and other cryptocurrencies’ problems, not FinCEN’s. Furthermore, blockchain analysis companies have the most to lose if this information is included in reports. Nevertheless, for the sake of reducing unnecessary data collection, this workgroup believes it’s unnecessary to include these identifiers. The MPWG also stresses that Monero view keys and key images explicitly not be required to be reported. Those should only be reported in a SAR, and only if they are available.

Of course, the MPWG does not like mandatory reporting overall. However, Monero has the most to lose if FinCEN does not create clear requirements. Currently, exchanges and banks hide behind a weak form of “compliance signaling” in saying they avoid the high-risk stuff “privacy coins,” while not understanding or caring that 1) these regulated entities are essential to mitigate money laundering and terrorist financing, and that 2) Bitcoin and other cryptocurrencies with robust P2P, or no-KYC DEX applications (like Ethereum) pose similar ML/TF risks by the nature of them being highly-liquid bearer assets.

# The time to act is now

Monero is increasingly used for a variety of activities as its network continues to grow. It is obvious that Monero is not going away. Both legal and illegal uses add to this growth.

Should FinCEN not take a stand to get the industry on the same page and to address the real and present risks with bearer assets, further Monero economic growth will occur in other more favorable jurisdictions and outside of regulated financial institutions. If this occurs, or if Monero is driven underground and off regulated exchanges, any exchange-generated data points that regulators and law enforcement currently have related to Monero use will be lost. FinCEN should quickly, actively, and clearly encourage exchanges to list Monero. If FinCEN does not, they will not have any significant partners to address growing ML/FT risks.

In short, Monero aims to be digital cash, and we believe that regulators should enforce existing regulations for cash on other bearer assets. The risks inherent in cash transactions are present in Monero and Bitcoin, and similar risk mitigations may be applied in these cases.


*The Monero Policy Working Group (MPWG) is responsible for this content. This is not legal advice, and it should not be relied upon for any purpose by third parties. To learn more about the MPWG, [click here](https://moneropolicy.org/about/).*
