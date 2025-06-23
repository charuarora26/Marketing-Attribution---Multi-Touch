# Marketing Attribution - Multi-Touch

❓: Optimize Return on Marketing Spend (ROMS)

📝: Measure the effectiveness of all Marketing Channels

👩‍💻: Use Markov's Chain to identify the Marketing Channel with highest and lowest removal effect

📊: Divert Marketing $$ from the least performing channel to the most performing channel leading increase in conversion rate.

The above mentioned is the brief of the project in a STAR format. The markeitng team has seen a budget cut this year due to increased pressure on marketing effectiveness and therefore wants to re-allocate the reduced budget across difefrent channels. The VP of Marketing however wants to know which channel is the least performing of all. Based on the findings, they will decide to redirect the lowest performing channel's marketing budget to the one that leads to most conversions or split the budget across all remaining channels. 

Markov's Chain methodology is best suited for this business decision since it specifically let's us see how much the conversions will drop if we were to completely eliminate the lowest performing channel. This is primarily possible due to the removal effects derived from Markov's Chain algorithm. The other two hueristic models conventionally used by the Marketing team conventionally are-
1. First touch attribution
2. Last touch attribution

The python notebook here has the code for the above mentioned three methodolgies. Let us know look at the results from each of these algorithms. The images below show the performance of each channel for conversion based on the methodolgy used. 



<img width="498" alt="LTA" src="https://github.com/user-attachments/assets/d78da067-619e-4e87-9607-e7f98c2764d6" />
<img width="500" alt="MCA" src="https://github.com/user-attachments/assets/092c2fac-4d35-4689-b3db-26ba299ff294" />

<p align="center" width="500%">
    <img width="498" alt="FTA" src="https://github.com/user-attachments/assets/c7c9d915-d3ad-4a62-8c18-a7ac3be4c7d0" />
</p>


We can clearly see that Online Display has the lowest conversion based on First-touch as well as Last-touch Attribution. However, the business wants to see how much the conversion will drop if they were to completely eliminate Online Display. This is arrived at using the Markov's Chain Algorithm. The above visuals show that the contribution of Online Display is about 13% for conversion. However the removal effect will be different. The image below shows a code snippet that calculates the channels with the most and the least impacts. 

<img width="919" alt="Channels by Impact" src="https://github.com/user-attachments/assets/4fbfb37e-e3f0-487f-9b3b-09cdc456a6e6" />

We can clearly see that Facebook has the highest impact (~36%) for conversion and Online Display has the least impact (~16%) for conversion. Therefore, we can assume that if Marketing was to redirect it's budget from Online Display to Facebook, the conversions will likely still increase because Facebook guarantees higher conversion.





References

1. [https://github.com/AjNavneet/MultiTouch-Attribution-Marketing-Spend-Optimization/blob/master/lib/Attribution_modelling_and_Budget_Optimization.ipynb](https://github.com/AjNavneet/MultiTouch-Attribution-Marketing-Spend-Optimization/tree/master)
2. https://medium.com/@aditya2590/multi-channel-attribution-modelling-with-markov-chains-fbf3bdab2ca8
3. https://medium.com/@xiaotingkuangcu/machine-learning-based-multi-touch-attribution-models-f95e45f7ab0f


