
There is no 1-for-all pool that you can delegate with, otherwise - every one would be delegating to same pool and there wouldnt be a point of decentralisation :) . While many users are attracted to the pool with lowest fee margins, it is usually the least important factor to distinguish between stake pools. Below are a few factors that might be important to take into consideration.

> Remember, you - a delegator - are indirectly one of the core components of the protocol and your actions may determine the decentralisation as well as adoption of the platform. Whether it is for your benefit, or benefit of the network - it is important that you select carefully who you will be delegating to.

!> There are heavy contributors to the ecosystem that may not be advertising and do not incur enough delegations, you can read more about them [here](community-contrib.md) if you'd like to support them.

In this section we will discuss the different aspects that users should consider when selecting who they would like to support. If you're unsure about any of the parameters when simply using wallet, please leverage benefits of community platforms built to help you with the decision making. The platforms are:
- [Pooltool](https://pooltool.io)
- [ADAPools](https://adapools.org)
- [ADAStat](https://adastat.net)
- [CardanoScan](http://cardanoscan.io)

Most of these sites will allow you to filter using various parameters to help you with the decision making. Furthermore, note the points below:

#### The Pool Operator  
  When staking with a pool, the first and foremost think you'd want to know about is the pool operator and his/her presence in the community. When things go south, you should be able to get in touch with the owners/operators of the pool. Most of the pools out there will have their social links available either via the website associated with the pool, or via extended metadata information. While we cannot judge everyone who wishes to not disclose their identities, you can be certain that ones who have been around for a while will not be putting their reputation at risk.  

#### Number of pools run by operator  
  There are a few operators running multiple pools with attractive marketing of low fees and very low pledge. While they're completely within their rights to do so - as allowed by the protocol, it is something controversial - and the aesthetics of such a pool is questionable (as there is an option to increase individual pool's fee instead of adding new pools). What such pools are doing (perhaps unintentionally) is a start of [Sybil attack](https://en.wikipedia.org/wiki/Sybil_attack#:~:text=In%20a%20Sybil%20attack%2C%20the,diagnosed%20with%20dissociative%20identity%20disorder) on the protocol. The protocol is designed to have incentives against this behaviour, but it only works on *basic rationale of delegator* being careful to not to make such pools too powerful. Perfect examples of such behaviour are 1PCT and OCE pools. From decentralisation point of view, you'd want to *stay away from those running multiple pools in general*.

#### Update channels  
  More often than not, Pool Operators will add ways to subscribe to their channels (be it telegram groups or twitter feed or website). It is important to join these channels for things like change of pledge amount or fees. Not doing so may leave a feeling of being blindsided when seeing a change of pool parameters. If you cannot find a way to reach the operator, you might want to question your decision.  

#### Saturation Point
  In order to not centralise all stake delegation to a single pool, after reaching a certain delegation criteria (calculated by `Total Supply in Circulation`/`nOpt`) where nOpt is currently 500, a pool will no longer be getting higher rewards for more delegation (currently this amounts to ~ `64M`). Thus, the reward portion of individual delegator will start reducing further as more stake is delegated to such a pool.  
  While in theory, rewards against a pool are optimal at saturation point, delegating to a pool close to saturation could always mean you're close to being over saturated (and will have to keep a constant eye on the delegation). Instead, having it against a comparatively smaller pool also means that your rewards are not necessarily impacted by much, but you help the network further by not participating against oversaturated (or potentially soon to be over saturated) pools. Depending on amount of stake you're going to delegate , you would ideally want to be stake with a pool whose Live Stake is somewhere between 5% to 70% of saturation point.

#### Fees  
  While standing a basic stakepool isnt really difficult, managing a pool operator with good security, availability, maintainance, and visibility requires incurs time as well as financial expenses. The protocol , thus, allows pool to specify their fees and allows it to do so based on a number of parameters. Note that this fee is *only taken from rewards* the network calculates against the pool, before distributing rewards further to delegators. As a delegator, below is a gist of things to know about when looking at pool fees:

#### Pool Pledge
  Pledge is basically the promise from the owners of a pool to maintain in their owner keys of the pool (thus , their own "skin-in-the-game"). Higher amount of pledge is rewarded by higher amount of rewards. However, note that at the current protocol parameters, the overall difference for rewards is not hugely affected by a pool pledging 100K vs pool pledging 1M (eg: for base assumptions, delegating 100K towards 100K pledged pool might earn you 5159 v/s 1M pledged pool might earn you 5161 ADA annually. However, delegating with 10M pledged pool for same assumptions might earn you 5223 ADA for the same scenario over a year. You can play with pledge parameter and their effects using the IOHK staking calculator [here](https://testnets.cardano.org/en/cardano/tools/staking-calculator/)

#### Pool Fixed costs
  This is the minimum rewards a pool will earn before rewards against blocks made by a specific pool is distributed to its delegators by the protocol. Current protocol parameters dictate a minimum of 340 ADA as a fixed minimum cost. The fee is enforced to prevent a race to 0 fee pools that are not really sustainable for protocol in future. Note that this the fixed cost from entire reward pot against all delegators delegating to pool.
  
#### Pool Margin (%)
  This is the percentage of rewards that a pool will be able to make from the total rewards pot. As compared to the reward pot that a pool generates (eg: 10000 ADA), the delegator's margin (eg: 2.5% of total rewards from pool) is not hugely affected by the Pool's margin being 1% (i.e. 230.9 ADA) v/s 4% (224.9 ADA) does not really affect delegator's rewards by a very big margin, unless that delegator forms a substantial amount of stake for that pool. The rewards are affected by lottery of slot allotment and pool's performance a lot more than the difference of margin. It is strongly recommended to *NOT* run towards a 0% pool *IF* it does not meet the rest of the points discussed above.  
  
#### Performance  
  This is an estimate of pool's performance based on how much stake protocol *thinks* a pool would have made versus how much pool actually did. Every block is rewarded by protocol (until saturation point), thus a delegator would want to stick with a pool that has greater than 85-90% of performance. Note that we cannot conclusively say 100% here because the actual blocks made by pools will also depend on how much blocks were actually assigned to a pool. There is a bit of randomness involved here for blocks to be assigned, which is proportional (like a roulette reserving higher number of slots corresponding) to stake.

#### Wallet Ranking  
  Wallet ranking in Daedalus does *NOT* take into account a few factors (luck associated with slot assignments to pools, even if proportional to stake, decentralisation factor making a further impact to randomisation), as well as not counting for the amount of stake user would like to add. While this should not be followed blindly, it would be a good reference point in long term for delegators to see how desirable the pool is as per the original specifications of the wallets.  

Hope the above helps you pick up a pool of your choice. If you would like to see any additions to this list, please raise an issue/PR against this repo using the icon on top right corner of the page.
