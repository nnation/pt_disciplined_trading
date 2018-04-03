# Background and Settings
## Thought Process Behind Settings
1. **Buy on evidence of good behavior.** I.E. EMAGAIN on a longer outlook (1 hour candles). When PT 2.0 comes out, look forward to buying on RSI as an indicator.

2. **Until PT 2.0 comes out, no buying on a downtrend (yet).** Feel free to change things up in settings.analyzer.json if you want to buy on a downtrend

3. **DCA with great depth.** DCA depth is much greater to prevent rapid consumption of capital. This will require patience. If you look at pairs that don't perform well, at least some of them still get good pumps that will allow the situation to break out of the DCA. But these pumps happen serendipitously and you'll need to wait them out or panic sell.

4. **Patience.** Some pairs will be held for 1 or 2 days. In other cases, a pair will be held for up to weeks.

## Global Settings
Bearish settings are based on a 3 hour anchor. This seems to be a good metric for determining overall health of a market. Bullish settings also require an anchor on 1 hour performance. This is because the bullish settings introduce additional risk, so we use an additional metric to ensure the bullish trend is consistent.

### New Coin
Too much risk. Remove if you want to try to jump on a pump.

### Downtrend
So the EMAGAIN setup buys when there's been an established trend of positive price action. If there's a significant dip, we avoid buying in because it could be indication that the run is over.

### High Risk Pump
These coins are showing very high increases in value. The chance that they will crash is too great to risk.

# FAQ
**Q:** Will this work with BTC?

**A:** Yes. You will need to update the below two properties in your PAIRS.properties.

    market = BTC
    ALL_max_trading_pairs = [your value here, see next question]
    ALL_min_buy_volume = [your value here, recommend 400-700]

**Q:** What should I set ALL_max_trading_pairs to?

**A:** You'll need to determine what your max trading pairs is based on your comfort levels, balance, DCA levels, and risk acceptance. As of this FAQ, I have 0.85 ETH. I can trade up to 18 pairs at a time. Your max trading pairs will be based on (1) your assumption of how many pairs will enter the various DCA levels (2) the **depth** of the DCA levels (3) ALL_max_cost_percentage. The true limiting factor on the number of pairs you run is your DCA setup. The current DCA setup is "deep" and so allows for a large number of pairs to be traded as the likelihood of DCA3 and DCA4 is less likely. Please take a look at my a helper spreadhseet I made availabe on [GoogleDocs](https://docs.google.com/spreadsheets/d/1pjx3M85yikbTD2DcVoZ22OkHuMWRHobwDwxa3R-SWuk/edit?usp=sharing).

**Q:** Why do you use ALL_max_cost_percentage instead of ALL_max_cost?

**A:** Bottom line up front: to make sure you're compounding. Longer explanation: if you use percentage, then each time you buy it will take into account previous gains/losses. If you're making gains, subsequent buys will be larger and will in theory return greater net gains.

**Q:** I've had a pair in the pairs log for X number of days, what's up with this?
**A:** You'll have that. This is the diciplined trading setup...meaning you'll need to be patient. Allow the DCA levels to do their thing and allow the market to do what it does. If you don't feel good about a pair, then by all means change your DCA depth. If you have success with different DCA setups (i.e., you don't overextend your balance) then please share =D

**Q:** What will the sales look like?
![Sales Log Example](https://i.imgur.com/lCreMNg.jpg)
