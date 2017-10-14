#BlockVote Whitepaper

## TODO
* split the challenges into milestones
  * no prototype on Ethereum
  * launches immediately as its own zone on Cosmos
  
## Name
Delfos Network - The island in ancient Greece where the oracle sat. Identity is an oracle into
the real world.

## Purpose
BlockVote removes the exclusive right to hold nation wide democratic election from the hands of 
central government. Smaller regions can use national ID cards with private keys to host fully 
democratic and secure elections, with or without the permission of any central government. The 
people of Catalonia would be able to hold an independence referendum without the central government
having the ability to stop or even censor it. As long as a country has a strong id system and 
allows the subsection into subgroups based on some criterium, this system allows the subgroups to 
have democratic election on any topic. A possible extension can be to use the web of trust to 
bootstrap an identity system that is th n used in the vote.

## Features
* GUI that supports almost all ID-card readers and smart cards as well as hardware wallets
  * built on top of an abstraction like OpenSC
* state that has recoverable keys
  * either through government issued ids or web of trust
  * different levels, it's a spectrum for users
* state that tracks the trustworthiness of a key
  * either based on government id or web of trust
* light-client libraries that allow dapps and other applications to request information on a
specific address or signature
  * the zone provides an identity service to the rest of the world through light-clients
  * the entire cosmos ecosystem can use this zone for identity and reputation
* permanent store of value with cash accounts
  * it's a combination of bank and cash
  * the government keys / high trust / recoverable keys store all your wealth
    * the amount can be revealed, e.g. tax authority
    * no one else can see the funds
    * ability to withdraw coins to completely private cash accounts that can be used for spending
* wallet that is a light-client
  * no access to bank account
  * spending account
  * can be used to pay for goods and services across the entire cosmos network
* the ability to define arbitrary elections and run them through the trusted keys
  * Catalonia can use this for the next referendum
* 

## Angle
Present this system not as a dry research piece. It is the future of violence free elections. It
removes the election monopoly of governments. It is build to enable anyone to run an election that
upholds the highest international standards without the need for central government to enforce
these standards. It does what Bitcoin did for the financial world for the governance process.
Before Bitcoin the government had a monopoly on secure money, but Bitcoin enabled us to have the
same security is centralised money without the monopoly. BlockVote does the same but for democracy.
It's impact will be further reaching than Bitcoin itself, because it tackles the fundamental
problem of human governance. With BlockVote 1.3 billion people in India can coordinate and come to
consensus on every aspect of live. It goes beyond just finance, this enables truly democratic
society.

* removes monopoly from governments
* is completely decentralised like the traditional voting system

## Choices
* uses Tendermint Consensus for the blockchain level
* uses a different validator set than the Cosmos hub though

## Challenges
* how to you handle someone losing their id card
* do we care that voters can see the results in real-time
* it needs to allow an arbitrary number of voters to fail at any step
* it cannot require voters to have money, or only require trivial amounts
* ideally the rate limiting should be done an a per-key basis
* no voter interaction is necessary to setup the interaction
* everyone needs to be allowed to change multiple times before the end of the election
* make it programmable so that endusers can easily create their own votes
* users need to be able to define their own set of eligible voters and encode their election

