---
layout: page
title: Regime Switching Time Series Forecast
description: An Investigation on Markov-Switching Vector Autoregression Model for Interest Rate Prediction
img: assets/img/4.jpg
importance: 2
category: projects
---

Recent years have seen unprecedented high volatility in interest rates. After the 2008 financial crisis, interest rates remained at a low level, until the Fed hiked rates in 2016 in response to the expanding economy and expected inflation (Gillespie, 2016). The news was viewed as somewhat bullish at the time, and the interest rate started to go upward ever since then. In March 2020, the Fed slashed rates to zero and launched a massive $700 billion QE program (Quantitative Easing) to provide liquidity to the market amid COVID19 (Liesman, 2020). Interest rates stabilized around zero once again, until surging inflation resulted from the pandemic declared a “war” on the Fed. On May 5th 2023, the Fed raised interest rates for the 10th time since 2022, to a 16- year high. All eyes have been on Fed’s next move; the market is also eager to know when the hike is going to end and how the rates could have been predicted.

In this paper, we aim to forecast the behavior of interest rates by analyzing their trend and the volatility of returns using Markov-Switching Vector Autoregressive model (MS-VAR). We assume there’s a latent variable called “market regime,” and that interest rate series behave differently as regime changes. We implemented two variants, MSMH(2)-AR(0) and MSH(2)- AR(1), to estimate the parameters characterizing the time series under each regime, and to forecast the upcoming regime. Understanding the transition among regimes shed light on the level of increase or decrease in interest rate, and the magnitude of volatility we should expect when making inferences into the future.

    ---
    In this paper, we investigated the MS-VAR family by implementing two of its variants, the 
    MSMH(2)-AR(0) and the MSH(2)-AR(1) model, to predict 3-month T-bill rate behavior under 
    binary market regimes. We deployed both a “rate trend model” where the market shifts 
    between the upward regime and "downward regime", and a “return volatility model” where 
    the market takes on either a high-volatility regime or low-volatility regime. Both 
    MSMH(2)-AR(0) and MSH(2)- AR(1) models provide satisfying retrospective forecasts when 
    tested with historical data, effectively capturing rate behavior. MSMH(2)- AR(0) gives 
    more granular predictions for the trend-focused model, while MSH(2)-AR(1) provides more
    meticulous predictions. Both suggest, that the current market regime is upward and likely 
    to persist in the near future. In addition, MSMH(2)-AR(0) predicts much more persistence 
    in both regimes, backing up its granular forecast results. In contrast, the MSH2- AR1 
    model implies more frequent shifts in the market regime and thus more shifts in forecasts. 
    For the volatility-focused model, both MSMH(2)-AR(0) and MSH(2)-AR(1) yield similar 
    parameter estimates and nearly identical predictions. The low volatility and high 
    volatility regimes are expected to persist for 5 days and 2.25 days respectively. Both 
    models predict that the current market regime is "low volatility" and likely to persist.
    ---
    

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/4.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
   
</div>
