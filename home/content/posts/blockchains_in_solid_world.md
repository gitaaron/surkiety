---
title: "How will blockchains exist in a Solid World?"
date: 2021-11-04T11:31:07-04:00
draft: false
---

I recently attended my first [Solid World Event](https://solidproject.org/events).  There seems to be a lot of potential for building a better internet here.

So I figured I'd share my thoughts on how [Solid](https://solidproject.org/) might work with blockchains since they are both rabbit holes I have been going down lately.

I should provide a caveat that I am extremely new to both spaces so the value in reading this is purely to get a newbie's perspective.  It is not to acquire a knowledge dump.

--- 

`BEGIN TLDR`

At first glance, they both seem to have different goals.

Blockchains are about removing intermediaries from a network of potential adversaries that requires trust.

Solid is about giving individuals control over their own data.

Perhaps they can both be grouped under a larger umbrella of initiatives that attempt to make a more equitable decentralized internet.

I think there could be some synergistic opportunisties for compelling solutions that involve both technologies.

`END TLDR`

---

First, let me write about the Solid experience.  As a perspective Solid user my first task is deciding on a Pod provider.  The Pod provider is essentially a program that runs and is available on the public internet.

I can be my own Pod provider or I can choose from a list of Pod providers out there that will store, manage and share my data on my behalf.

If an app integrates with Solid then it can allow me to sign in to the app using the credentials associated with my Pod.

This is very similar to the way 3rd party sign on works today.

When I click|tap login, I am directed to a 3rd party's website (eg/ Google, Facebook, Github) and the site asks me what information I want to share.

I am then redirected back to the app and I can continue interacting with it as if I signed in with my own email.

If I gave the app write permissions it might also write data back to my Pod.

In theory this should incentivize app developers to work with Solid because now they can benefit from piggy backing on a large network.

For example, lets say a large photo sharing app worked with Solid and I wanted to write a web based photo editing app.

If both apps were based on Solid then I would no longer have to ask my users to import all of their photos!  Their personal photos are already at their fingertips.

This sounds great in theory, however, I worry about how it will work in practice.

In fact, it kind of scares me because as a custodian of my user's data, I worry about a future where data I have collected on behalf of a user is easily misused by another entity.

If I close my eyes and imagine a world where EVERY user and service provider on the internet is based on Solid then this can easily become an overwhelming feat of knowing what ['Solid App'](https://solidproject.org/apps) to trust.

One might argue this is already the case with third party sign on.  However, I think there are a few key differences here.  The first difference is the role of the data / identity provider.

In today's third party sign on world, these large providers are storing an immense amount of data and a lot of it is sensitive.

It is their job to design a UX in such a way that it is very hard for me to accidently share sensitive data with an outsider.  They would never put 'share your credit card number' in fine print.

Perhaps part of the solution is utilizing [Solid Vocabularies](https://solidproject.org/developers/vocabularies/well-known) such that it makes it easier for a user to know what data they are sharing at a glance.

However, what if an app developer writes their user's credit card number to the wrong vocabulary?  Worse off - what if it becomes an unwritten standard and other developers start [following suit](https://www.youtube.com/watch?v=TrTk6DsEJ2Q)?

There are probably thousands of examples of websites today that break PCI compliance.

There is a simple fix for that though - I simply don't share my credit card number with sites I don't trust and rely on sites I do trust to not provide a poor UX that has me mistakenly share my credit card info with a scammer.

As a consumer it is impossible for me to verify the trustworthiness of every vendor I transact with so I just go with trusted brands.

We could all just agree on a single authority that has write permission for my credit card but but now we are back to centralization.

So how do we solve this in a Solid (or Web3) world?

One solution I can think of is it would be nice if there was a credentialing system for DApps/APIS/service providers/communities or any non-human entity.

Most of the conversations I see in Web3 revolve around credentialing humans.  I think they are incredibly important conversations with their own [treacherous pits](https://news.bitcoin.com/andreas-antonopoulos-case-reputation-identity-systems/).

However, as I already outlined, I am a lot more worried about how we credential the bots that we will all interact with.

The first thing I (a perspective user) would like to see when a DApp asks me for my permission to do something is a report card on various things I care about such as security, privacy, trustworthiness (you know all that good stuff).  If its a community|coop|DAO|guild then I would also like to see how governance works in their network and sound financials.

Even better than that from a UX perspective is a 'certified organic' badge since 99.999% of the population is not thinking about the deeper consequences of all these things.

Inevitably there may be tradeoffs (eg/ transparency vs privacy) so perhaps the answer is several cleverly designed badges that click|tap into a more detailed report card.

This is not a new concept.  There are many examples of [credentialing systems](/distributed_credentialing_systems) for distributed architectures in the wild.

Assuming the overall user facing design is figured out, then comes the problem of implementation details.  Technical audits are not cheap and usually only involve security.

We could just go with an APP store and there may be lessons learned from the pre-existing APP stores out there from a UX perspective.  However, like most other credentialing systems, APP stores for the most part involve centralization so they don't really help much.

Perhaps this is how blockchains could be utilized in a Solid world?

There are already several initiatives around [third party audits](https://openzeppelin.com/security-audits/) mainly focused on security of smart contracts.

The nice thing about contracts executed on a blockchain is they are unchangeable making it is easy to verify that they do what they claim.

In the example of persisting my credit card number, the program would need to get certified that it is storing my credit card number with proper encryption to the appopriate vocabulary.

If it executes on the blockchain it can get certified that it does this once and I can trust that the source code will not get updated (there are no backdoors).

There is also power in the [DSL](https://en.wikipedia.org/wiki/Domain-specific_language) (whatever that will look like).  The blockchain ecosystem itself is currently riddled with [scams](https://www.bbc.com/news/business-59129466).

As the ecosystem matures and converges on open standards, it should become more and more difficult for a scammer to succeed.

For example, a wallet maker could do a check for the liquidity of a coin.  If it is not liquid then they could offer a warning that the coin is probably worthless because it is not resellable.

This blacklist approach is great for covering scams we already know about but what about scams that have not occured yet?

In that case, if the transgressions of the DApp are simple enough the maker could utilize the DSL to more easily get whitelisted.

For example, lets say I am a marketplace selling artists' collections of their work.  I could simply offer off the shelf [ERC-721](https://eips.ethereum.org/EIPS/eip-721) and buyers can more readily trust I am indeed hocking collectibles.

This is great in theory because it should lower the cost of entry for anyone wanting to create a similar marketplace since the trust could be shared between the marketplace and the wallet.

Nonetheless, the bigger the entity becomes the less 'standard' their technical service will become and so their auditing expense will increase exponentially.

This is a good thing because it means the system was designed such that it is easy to get started and difficult to grow large.

The only issue is if this seemingly benevolent dictation causes the opposite effect.

What I mean is the ecosystem could also hamper innovation as the only economically viable 'new ideas' will come from a recipe of atomic units (aka contracts) and not from creating completely new atomic units themselves.

However, perhaps if a clever auditor can write acceptance level (aka pen) tests to execute in a standardized environment (eg/ [EVM](https://ethereum.org/en/developers/docs/evm/)) then the cost of verification of completely new ideas could also drop.

In both cases - a library of pre-existing contracts and completely new contracts - there will require a trusted set of human eyeballs to audit new lines of code so the cost will never be zero (unless someone can write a clever AI to outperform human auditors?).

However, the blockchain could also enable new business models that could potentially lower the cost of code verification.

Another [interesting initiative](https://www.decentology.com/blog/composing-the-hyperverse) could drastically lower the cost of audit by enabling auditors to stake their work in a startup and get rewarded if and only if the startup succeeds.

In my head a current equivalent might be personal injury lawyers that do not charge their clients upfront and instead take a commision of the benefit that the client receives.

In the case of a tech auditor profiting from a startup's success, the theory is it is in the auditor's interest to do good work because if a security flaw is found then they would end up losing money instead of gaining (at least this is what I believe is the intention of staking in the 'hyperverse').

There is one snag that I can think of though - auditors will essentially have to become angel investors and develop a recognition for startups with potential since that is where their payout will come from.

Even so, I think this is just an opportunity for enterprising individuals and does not represent a true barrier to the ultimate goal of better decentralization.

There are still many problems to solve here.  For example, how can the auditor registry also be decentralized?  Its a bit of a chicken and egg problem.

Perhaps looking at [other efforts](https://news.ycombinator.com/item?id=20625561) involving blockchains to create a globally decentralized registry will provide answers.

---

So far I have spoken about the role blockchains might play in a 'Solid World'.  But what about the other way around?

To imagine how Solid might be useful with blockchains, lets go on a journey and understand why large platforms exist in the web2 world in the first place.  Lets take a closer look at ride sharing platforms.

There are many functions this platform has to provide, however, for simplicity sake I will focus on a single function.  How does the rider trust the driver?

Its midnight and I am travelling in a country I have never been before perhaps because I made a romantic connection on the internet and we finally decided to meet face to face.

This country may not have the same social structures that I have taken for granted while living in the developed country where I am from.

So I can't just flag down a taxi from off the street because the taxi driver could easily drive me out into the middle of nowhere, take all my money, and leave me standing around in my underwear.

So I whip out my ride sharing application (an instituion I can trust) and find the closest trusted driver using it instead.

Another benefit of this model is a corporation can operate across boundaries so I don't have to install a different app for each country.  Because it is a single centralized entity, the corporation can also benefit from reuse where similar operating procedures can be applied to different geographic districts.

It is also beautifully designed and works seamlessly because of capitalism.

How does the institution know this is a driver I can trust?  The driver has an identity which a local government assigns to them that they can use to join the ride sharing platform.

They only get a single identity on this ride sharing platform and that way if they do something bad the platform can simply ban them or take some other punitive action.

Hopefully this scenario frightens you.  Why?  Because we are giving the corporation an immense amount of authority and they are not operating in the stakeholder's interest.  They are operating in the interest of the 1% - the shareholder.

With this authority they are able to act as a leach on society, extract wealth and further increase the gap between rich and poor.  This is the problem we are solving for.

This is where I think blockchains can play a role.  It will remove the need for an intermediary authority telling us which drivers to trust.

It will enable us to design the platform to function as a cooperative in the sense that all stakeholders (riders, drivers, and builders of the system) can share in ownership/authority transparently with all other participants.

With transparency we can ensure that we don't give up power to an elite minority and that there are proper checks and balances thus promoting democracy.

But what happens when the blockchain inevitably stops serving every participant's interest?

What if a driver is banned because they said or did something that is so incredibly controversial that the ride sharing platform no longers wants to associate themselves with the driver.

For absurdity sake lets say the driver decided to wear a purple hat with white polkadots and the meaning behind it is incredibly inflammatory.

This happens all the time today.  Celebrities are cancelled and people are fired from their jobs because of what they said or did.  I am not going to argue that there should not be repurcussions for deplorable actions.  Thats for a completely different rant about correctional vs penal institutions.

What I am going to argue is these new social structures need to be designed carefully so that people are not getting boycotted from the entirety of a global society.

On the rider side of things if the platform does not serve my interests (eg/ the platform allows for drivers wearing purple hats with white polkadots and that is a symbol for people that commited mass genocide in the country where I am from) then I should also have the ability to use a different platform.

How is this done?

The driver should be able to take all of their attributes (eg/ full name, car they drive, citizenship, driving history etc..) and bring it over to a different ride sharing platform.  The rider should be able to easily perform a similar action.

In order for this to work the data needs to flow freely between platforms.  There are [other mobility tools](/blockchain_scaffolding_tools) being developed for blockchains.

However, I think Solid shines because its focus is not only on data normalization and standardization of protocols.  Its also about putting the user in control of their data.

If DApp developers and Pod providers build on top of Solid they maintain a promise to their users that if they grow unhappy with their service they can always [exit](https://en.wikipedia.org/wiki/Exit,_Voice,_and_Loyalty).

The thing that has me the most interested about Solid is not the fact that I can share my user's data with another service provider or benefit from it's network effect (I am interested in that just not as much).  Its the fact I can easily maintain this promise of exit.

In a world where communities converge around a single source of truth, design for platform mobility will be even more important.

With platform mobility, perhaps the riders and drivers may not have the right to be forgotten but at least they will have the right to be forgiven.

---

This is why I am interested in both Solid and blockchain although I have only scratched the surface.  This is why I intend to [dig deeper](https://www.mcgill.ca/oss/article/did-you-know/ostriches-do-not-really-stick-their-heads-sand).


