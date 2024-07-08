You can make \$ by buying prediction feeds, and using it as an input — as “alpha” — to your trading approach.

<figure><img src="../.gitbook/assets/predictoor/progression_of_a_trader.png" alt=""></figure>

Typical steps as a Trader:
1. **Play with dapp, and trade.** First, go to [predictoor.ai](https://test.predictoor.ai/) to build intuition: observe the free feed, perhaps buy a few feeds, and watch them change over time. In a second window, have Binance open. Employ a baseline trading strategy: when a new Predictoor prediction pops in, buy if “↑”, and sell or short if “↓”; exit the position 5 min later.  
1. **Run a trader bot.** Follow the steps in the [Trader README](https://github.com/oceanprotocol/pdr-backend/blob/main/READMEs/trader.md). You’ll start by running simulations with AI-powered predictions. It follows the baseline trading strategy: when a new Predictoor prediction pops in, it buys if “↑”, and sells if “↓”. Then you’ll do run a trader bot on a remote testnet with fake tokens. Finally, you’ll do it on mainnet with real tokens on a real exchange.
1. **Improve & extend.** Improve trading performance via more sophisticated trading strategies. This is a universe all of its own! Extend to >1 prediction feeds (Predictoor has many). Wash, rinse, repeat.  

The actions as a trader offer a single yet powerful way to earn: **trading revenue.** Buy low and sell high! (And the opposite with shorting)  

  

⚠️ You will lose money trading if your \$ out exceeds your \$ in. Do account for trading fees, order book slippage, cost of prediction feeds, and more. Everything you do is your responsibility, at your discretion. None of this blog is financial advice.  

## Early Earnings Benchmarks

Predictoor aims to make it easy for people to make \$ doing predictions (as predictoors), and taking actions against those predictions (as traders).

Before we started building Predictoor, we first asked: _can we predict ETH (etc) up/down with accuracy?_ Then we conducted intensive AI/ML research towards this question. The results of this investigation were positive 😎. TBH, we were surprised at the degree of market inefficiency.

Our next question was: _with these predictions, can we make \$ trading?_ Again, we conducted intensive AI/ML research, and again found positive results 😎😎.

Here we share some results of that research — a glimpse of how deep the rabbit hole goes — to inspire would-be predictoors and traders in their own work. The model was trained on data from January 1, 2021 to June 30, 2023, with simulated results the first 24 days of July 2023. A “baseline” trading strategy was used:

The image below shows simulated returns as a function of order size, for BTC/USDT on Binance. Duration = 7000 ticks x 5m/tick = 24.3 days of trading. It simulates spread effects. It assumes 0% fees. Note how the size of the order affects the return. This is because BTC/USDT is not very liquid; therefore larger amounts cause slippage.

Simulated returns vs time of BTC/USDT trading on Binance. Trade size has an impact.
The image below has the same experimental setup, but for BTC/USDT pair. The size of the order does not affect the return, because BTC/USDT is more liquid than BTC/USDT.

<figure><img src="../.gitbook/assets/predictoor/simulated_returns_btc_usdt.png" alt=""><figcaption>Simulated returns vs time of BTC/USDT trading on Binance. Trade size has little impact.</figcaption></figure>


