Delegation allows holders of ada to transfer their right to participate in the proof of stake protocol to stake pools. Stake pools are run by stake pool operators (SPOs) and a person delegating to a stake pool is called delegator, member, or participant. A stake pool consists of a block producer (BP) and any number of relays - each of these are called a node. The blockchain is made up of consecutive blocks and stake is power to make blocks.

If one pool or person is given too much stake power they can control consensus, engage in double-spending attacks, create forks, censor blocks, and damage or even destroy the system. Your delegation choice, who you give your power to, is very important at limiting a single entity from creating too many blocks.

“There should never be a conflict of interest between maximizing rewards and ‘doing the right thing’”

The staking mechanism was designed so that you can optimally secure the network by trying to maximize your rewards and being greedy with your delegation choice. Stake pools can offer very different return rates.

“How attractive a pool is to delegators depends on four interacting elements: pledge (the higher, the better); operating costs (the lower, the better); operator margin (the lower, the better); performance (the higher, the better).”

It is important that you understand each of these elements and how they can effect your rewards.

The first thing you should consider when looking for a pool is pledge. Pledge is the amount of stake the SPO has in their own pool.

“Think of pledge as a ‘commitment’ to the network.”

An operator with very little pledge that controls a lot of stake is highly leveraged.

“The lower the leverage of a blockchain system, the higher its degree of decentralization.”

Pledge is part of the mechanism that prevents one person from operating many pools (pool-splitting) by making pool reward rates increase with pledge. If an operator wants to split one pool into many, they have to dilute their pledge between all the new pools, causing all of the pools to receive lower rewards than if the pledge were consolidated into one pool. Pledge is the only pool parameter that increases rewards and, paired with saturation, aids in decentralizing the network.

It is prohibitively expensive for one person to open many high pledged pools and relatively cheap for one person to open many low pledged pools. This is what makes it almost impossible for a single individual to gather a majority of stake by opening many high rewarding pools, it’s simply too expensive. This principal is the backbone of Cardano’s security model.

Every 500k pledge increase means delegators will receive ≈ 0.008% APY MORE rewards

Next consider pool fees, both margin and fixed. The fixed fee is subtracted from the total pool rewards for an epoch. Then the margin is applied. Then the remainder is paid to delegators proportional to their stake.

Ex. 340 ADA fixed and 1% margin
(total_pool_rewards - 340) * 0.99 = total_delegate_rewards

Margin can range from 0% - 100%; a 0% margin pool collects no additional fee over the fixed fee, and a 100% margin pool pays no rewards to its delegators.

Every 1% margin increase means delegators will receive ≈ 0.037% APY LESS rewards.

“By pledging more, the pool operator can ask for a higher operator margin while still being attractive to delegators.”

As a rule of thumb, 2.3 million pledge and 1% margin cancel each other out.

Fixed fee effects delegate rewards proportional to pool size. If the pool has little total stake then each delegate pays more of the fee from their cut of the rewards. The minimum fixed fee is 340 ADA/epoch.

Saturation is the level at which a pool becomes too large. A pool is saturated at 100% and at that point is offering its best returns. Rewards drop pretty drastically when a pool becomes oversaturated.

Next consider performance. Actual performance, the ratio of blocks assigned to blocks forged, will always be somewhere less than 100%. A certain number of blocks are expected to be missed as orphans and from *factors out of the control of the operator, but generally the pool should be forging all of its assigned blocks. Performance is most difficult to judge because only the attentive SPO knows actual performance and few make this public. Those that do voluntarily report actual performance to pooltool.

*Early iterations of Cardano-node contained bugs that would cause pools to miss blocks for various reasons. Pools that have been around since Shelley launch will naturally have lower overall performance than pools that started more recently. Not all of these bugs have been corrected yet.

Certain websites track a pool’s luck, which is the ratio of blocks forged to blocks expected. This metric is only really useful for finding pools that are drastically underperforming. You can guarantee that a pool with greater than 100% luck has been scheduled more blocks than expected but it does not mean they have outperformed other pools. Conversely, a pool with less than 100% luck might have just been assigned fewer blocks than expected or may be underperforming by missing scheduled blocks.

You can find pool parameters (pledge, margin, fixed fee, saturation, etc.) on pooltool.io or cardanoscan.io.

Besides looking at reward rates you should also judge a pool by its infrastructure. At a minimum, a pool should have a block producer and two relays. Relays speak with other pool’s relays and are responsible for transmitting blocks and transactions through the network. The more relays a pool has the better. The pool should have some redundancy in place that responds automatically to failures within the system. For example, if the block producer node blows up, there should be another node quickly taking its place. All of the nodes should be distributed and not under the same roof.

Finally, do some research into the pool operator. Are they asking questions about how to run a pool or are they answering questions? Do they run many different pools? If so, why so many and why not consolidate pledge for delegate benefit? Do they contribute to the overall community or ecosystem in some way? Is the pool run by an individual or a team? Do they completely understand how the protocol and reward model works? Can you reach out to them with questions?

Be cautious accepting delegation suggestions or advice from any SPO. SPOs and delegators have different financial incentive within the system. Delegators want high rewards from their stake. SPOs want to run as many pools as they can at the highest acceptable fee. This always comes at the expense of the delegators’ rewards. SPOs will suggest that you delegate to their pool, but it’s unlikely that their pool offers the highest return on stake.

Here are some, but not all, examples of fraudulent pool behavior that should be avoided:
Pools that…
impersonate other pools or businesses without any affiliation,
promise higher rewards than their pool can offer,
promise additional tokens or any other future value in exchange for your rewards,
modify their parameters just before and and after epoch switch to avoid detection

You should use a notification service like pooltool or cardanoscan bot on telegram to notify you of any parameter changes, like pledge or fees, or if your pool becomes oversaturated.

It cost almost 0.18 ADA every time you switch pools. If you only have a few thousand ADA you should try to minimize your pool changes. Your transaction fees can quickly eat up your rewards.

You do not need to withdraw your rewards. Rewards and any new ADA in your wallet are automatically part of your staking balance.

Below is a tool built by a member of the Cardano community that plugs pool parameters into the reward equation to generate expected reward rate. It is useful to compare pools against each other.
https://dynamicstrategies.io/crewardcalculator
https://hydra.iohk.io/build/790053/download/1/delegation_design_spec.pdf
https://iohk.io/en/blog/posts/2020/05/12/how-pledging-encourages-a-healthy-decentralized-cardano-ecosystem/
https://iohk.io/en/blog/posts/2020/11/13/the-general-perspective-on-staking-in-cardano/
