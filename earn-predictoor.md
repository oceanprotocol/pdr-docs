
If you have background in AI, ML, data science or statistics (and these overlap!) then you’re well suited to become a predictoor to make \$.

<figure><img src="../.gitbook/assets/predictoor/progression_of_a_predictoor.png" alt=""></figure>

Typical steps as a Predictoor:
1. **Play with predictoor.ai.** Go to [predictoor.ai](https://predictoor.ai) to build intuition: observe the free feed, perhaps buy a few feeds, and watch them change over time.
1. **Run a predictoor bot.** Follow the steps in the [Predictoor README](https://github.com/oceanprotocol/pdr-backend/blob/main/READMEs/predictoor.md). You’ll start by running simulations with AI-powered predictions. Then you'll run a predictoor bot on a remote testnet staking fake OCEAN. Finally, you’ll do it on mainnet staking real OCEAN.
1. **Optimize the bot.** Improve model prediction accuracy via more data and better algorithms. Extend to predict >1 prediction feeds (Predictoor has many). Wash, rinse, repeat.  

The actions as a predictoor give the following ways to earn:  
* **Feed sales.** At an epoch, sales revenue (minus fees) for that epoch goes to predictoors. It’s distributed pro-rata by stake among the predictoors who predicted the true value correctly. The revenue for an epoch is the fraction of sales, spread uniformly across subscription length. A price of 3 OCEAN, 5m epochs, and 24h (1440m) subscriptions gives a revenue of (# subscribers) * (3 OCEAN) * / (1440m / 5m).
* **Stake reshuffling.** At an epoch, incorrect predictoors have their stake slashed. This slashed stake is distributed to the correct predictoors pro-rata on their stake.
* **Predictoor Data Farming.** This amounts to additional earning for predictoors. [Here are details.](https://docs.oceanprotocol.com/data-farming/predictoordf)

**On Prediction Accuracy.** Don’t expect to be 100% accurate in your up/down predictions. Marginally better than 50% might be enough, and be skeptical if you’re greatly above 50%, you probably have a bug in your testing.

**On Amount to Stake.** How much should a predictoor stake, to maximize revenue and bound risk? If you stake more, you can earn more, _but only to a point_. Earnings are bounded by sales of the feeds. So if you stake too much, you will lose $. [This blog post](https://blog.oceanprotocol.com/rewards-mechanisms-of-ocean-predictoor-6f76c942baf7) provides equations that bound how much to stake, along with general tips.

{% hint style="warning" %}
You will lose money as a predictoor if your \$ out exceeds your \$ in. If you have low accuracy you’ll have your stake slashed a lot. Do account for gas fees, compute costs, and more. Everything you do is your responsibility, at your discretion. None of this blog is financial advice.
{% endhint %}

