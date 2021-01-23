  
  
Below is a list of frequently asked questions within Cardano community channels across social media. If you see something not answered, please raise an issue/PR using the icon in top right corner :smile:

#### I delegated to a pool in epoch `n` , when will I receive rewards? :id=reward-schedule
For any change in delegation, the rewards are reflected after 3 epoch transitions (thus, after `15-20 days`). Checkout details below for how it works:
- An Epoch in cardano is 5 days long. Any change in Delegation is captured in snapshot at end of the epoch (at 1st epoch transition).
- The snapshot captured is considered *live* at the next (2nd) epoch transition. This means the pool you delegated to would reflect your delegation in `n+2` epochs, to qualify for chance to make blocks proportional to its stake (which would now include your delegation).
- The blocks made by pool qualifies for rewards, which is calculated at next epoch transition (thus, calculation occurs at `n+3`).
- Finally, The rewards are then paid out at the end of next epoch `n+3`.
Thus, if you delegated in epoch `n` your rewards will be with you by the start of epoch `n+4` (technically, it will be at the end of epoch `n+3`).
The visual representation of the above explaination is as per below (using `n=213` in the example):

  ![Rewards Schedule](https://raw.githubusercontent.com/cardano-community/support-faq/images/docs/images/rewards-schedule.jpg)

#### Do we miss rewards when changing delegation to different pool? :id=change-delegation
No.
If you're changing to a different pool twice within an epoch, only the last change will be captured at epoch snapshot.
If you change delegation from pool `P1` to `P2`, you still receive rewards from  to pool `P1` until [reward schedule](#reward-schedule) for `P2` starts.

#### How do I monitor my rewards? Yoroi or Daedalus does not show epoch-wise rewards distribution :id=monitor-rewards
Yoroi does show rewards history, now also available as part of Export to CSV. In case you are not able to show the rewards history in the format you'd like in wallets, there are multiple ways to monitor your rewards, you can use add any of your wallet addresses (it doesnt matter which one, pick a random address from your Wallet > Receive tab) and track rewards history using any one of the below:
- via browser in [pooltool] or [cardanoscan]
- get notifications via [PoolTool Mobile App](https://pegasuspool.info/) on your mobile
- get telegram notifications via [ADAstat](https://t.me/AdaStatBot)

#### I did not receive my rewards in spite of waiting as per the schedule. What should I look for? :id=missing-rewards
First point of contact is ideally your pool operator. Most of the pool operators do provide a way for you to contact them. But few pointers to check the cause yourself :
- If you're expecting rewards in epoch x, check the blocks made by pool in x-2 (refer to schedule [above](#reward-schedule) for details).  You can use any of the [pool explorers](explorers.md#list) and check the pool history for blocks made at epoch level.
- If the pool did make blocks, but you did not receive rewards, verify the pool parameters - if the fixed cost fee (default minimum is 340 ADA) for pool is higher than rewards it gives back, a delegator may not receive rewards.
- If the operator himself did not receive any rewards, that may indicate an issue with his pool setup, best to notify them as early as possible.

#### Do I need to withdraw rewards and stake again? :id=withdraw-rewards
The rewards you earn are automatically staked to the pool as part of your delegation. This goes true for any new funds received/depleted from the wallet as well. Currently your wallet itself is delegated to a pool, any changes occured in epoch `n` will thus, be automatically captured as part of snapshot and incur updated rewards at epoch `n+4`. **The only time you may need to withdraw your rewards is when you're moving all your funds to different wallet/exchange. 

[pooltool]: https://pooltool.io
[cardanoscan]: https://cardanoscan.io
[adapools]: https://adapools.org
