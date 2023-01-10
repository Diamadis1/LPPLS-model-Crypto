# Project-5
Lppls model on full BITCOIN time series (trying to predict a bubble or a significant movement in the near future) 

Price/day in logarithmic scale
![image](https://user-images.githubusercontent.com/98957437/211603724-5d4f30b0-a402-4b30-97e6-5b3706a6dc24.png)
![image](https://user-images.githubusercontent.com/98957437/211603817-02f7801a-076b-439d-b702-39480756ed1c.png)

Time Series Logarithmic Returns of BTC to $USD
![image](https://user-images.githubusercontent.com/98957437/211603894-59055d70-bd0b-40b5-bc7e-2454b9868adc.png)

The effect of the various model parameters on the results was investigated. First the effect that the size of the rolling window w had on the predictive ability of the model was investigated. This was done by looking at the Confidence Indicators produced and their strength in historical BTC bubbles.

![image](https://user-images.githubusercontent.com/98957437/211604669-196b3797-9bc8-408a-ba37-6308818b3219.png)


4 sizes were selected for study, shown in Figure 3. In this figure we observe that as the rolling window grows, the number of confidence indicators in a given time period tends to increase, 
while the values of these indicators tend to fall. Although it is preferable in a given period when we expect a bubble to have several indicators, 

as it is not legitimate for the values of the indicators to be small as this makes it difficult to distinguish between possible bubbles and false positives of the model. For this reason, we considered w=120 as a first estimate optimal value

![image](https://user-images.githubusercontent.com/98957437/211604936-8246fb80-757e-49c5-979d-fac62c8f4071.png)

An example of such an indication is shown in Figure 2. So it would be expected, if the model is working well, that these indications would hold until our bubble bursts. In that chart, the green line shows the date where the forecast is made, the red line shows the earliest forecast date of t_c and the yellow line the latest forecast date.

![image](https://user-images.githubusercontent.com/98957437/211605240-0324c906-820e-480b-9c26-79997b403f62.png)
