{\rtf1\ansi\ansicpg1252\cocoartf2822
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\froman\fcharset0 Times-Roman;}
{\colortbl;\red255\green255\blue255;\red52\green52\blue52;\red255\green255\blue255;\red0\green0\blue0;
}
{\*\expandedcolortbl;;\cssrgb\c26667\c26667\c26667;\cssrgb\c100000\c100000\c100000;\cssrgb\c0\c0\c0\c87059;
}
\paperw11900\paperh16840\margl1440\margr1440\vieww25860\viewh14820\viewkind0
\deftab720
\pard\pardeftab720\sa240\partightenfactor0

\f0\fs28 \cf2 \cb3 \expnd0\expndtw0\kerning0
The exercise is to use the coupon data to infer what features play a role in deciding whether drivers accept coupons. \cf2 \
\pard\pardeftab720\sa240\partightenfactor0
\cf2 #Problem 1:\
The first problem looks into bar coupons and evaluates the effect of different user attributes on the bar coupon acceptance rates. Below sections explain key observations and the next steps.\
#Key Observations\
The analysis demonstrates a strong correlation between bar frequency, age, income, and the acceptance rate of bar coupons.  The key findings can be summarized as follows:\
* **Overall Bar Coupon Acceptance is Low:** The overall acceptance rate for bar coupons is relatively low (41.03% for the "Bar" cohort, compared to 56.84% for all coupons). This suggests that bar coupons may not be as effective as other types of coupons.\
* **Bar Frequency is a Strong Predictor:** The most significant factor influencing coupon acceptance is the frequency of bar visits.  Individuals who go to bars more frequently have substantially higher acceptance rates.  This holds true across various age and passenger demographics.\
* **Age and Bar Frequency Interact:**  While bar frequency is the primary driver, age interacts with this factor.  Younger individuals (under 30) who frequently visit bars show a very high acceptance rate, comparable to older individuals who meet similar criteria (non-widowed, no children as passengers).\
* **Income and Restaurant Preferences Matter:**  Lower income and frequent use of cheap restaurants are strongly associated with lower coupon acceptance rates.  This highlights the importance of targeting specific income brackets with tailored offers.\
* **Family Status and Occupation Influence:** The presence of children as passengers and occupations in farming, fishing, or forestry are negatively correlated with coupon acceptance. This might be due to limited disposable income or incompatibility with bar visits.\
#Visualisation\
I plotted histograms for various columns to understand the kind of values each column held. The plots are present under the DataVisualizations folder.\
I plotted bar plots to compare the acceptance rates for each set of cohorts separately. \cf2 The plots are present under the DataVisualizations folder, their names begin with \'93Bar\'94.\cf2 \
#Nest Steps\cf2 \
\pard\pardeftab720\sa240\partightenfactor0
\cf2 * **Targeted Marketing Campaigns:** Focus marketing efforts on individuals who frequent bars, particularly younger adults (under 30).  Segmentation by income level is also crucial, tailoring offers to high-income individuals who frequent bars and potentially offering different incentives to lower-income groups.\
* **Refine Coupon Design:** Consider adjusting the value or type of bar coupon to make it more appealing to a wider audience, especially those with lower incomes or families.  For example, offering discounts on food items in addition to drinks might improve acceptance among families who might not otherwise use bar coupons.\
* **A/B Testing:** Conduct A/B testing with different coupon designs, values, and target audiences to further optimize campaign effectiveness.  Experiment with different messaging to better appeal to specific demographics.\
* **Further Research:** Investigate the underlying reasons for the low overall acceptance rate of bar coupons.  Qualitative research (surveys, interviews) could provide valuable insights into consumer preferences and perceptions.\
* **Consider Alternative Incentives:** Explore offering incentives other than just discounts. Loyalty programs, bundled offers with other services, or exclusive events could be more appealing.\
**Limitations:**\
The analysis relies on observational data and correlations.  Causation cannot be definitively established.  Further research would be needed to definitively prove the causal relationships between the factors identified and coupon acceptance. \cf2 \
\pard\pardeftab720\sa240\partightenfactor0
\cf2 #Problem 2:\
The second problem looks into coffee house coupons and evaluates the effect of contextual attributes\cf4 \cb3 \outl0\strokewidth0 \strokec4  \cf2 \cb3 \outl0\strokewidth0 on the coffee house coupon acceptance rates. Coffee House Coupons show an interesting observation, their acceptance and non-acceptance rates are almost equal. I wanted to understand the effects of contextual attributes on the acceptance rates to understand the right context to target drivers. The below sections explain the key observations and the next steps.\
\pard\pardeftab720\sa240\partightenfactor0
\cf2 #Key Observations\
The data shows the acceptance proportion for different cohorts.  Comparing them\
**1) All vs Coffee House:**\
* **All:** 56.8% acceptance rate.\
* **Coffee House:** 49.9% acceptance rate.\
The "All" cohort has a significantly higher acceptance rate than the "Coffee House" cohort (a difference of almost 7 percentage points). This suggests that coffee house coupons have lower acceptance rate when compared to acceptance rate for all coupons\
**2) Age <25 vs Age >25:**\
* **Age <25:** 55.0% acceptance rate.\
* **Age >25:** 48.1% acceptance rate.\
The younger cohort (age <25) shows a higher acceptance rate than the older cohort (age >25) by approximately 7 percentage points.\
**3) GEQ5min vs GEQ15min vs GEQ25min:**\
* **GEQ5min:** 49.9% acceptance rate.\
* **GEQ15min:** 45.4% acceptance rate.\
* **GEQ25min:** 34.5% acceptance rate.\
There's a clear trend here: as the minimum time spent in traveling increases, the acceptance rate decreases.  The difference between 5 minutes and 25 minutes is substantial (a 15.4 percentage point drop). This suggests that longer durations spent traveling are negatively correlated with acceptance.\
**4) Direction_same vs Direction_opp:**\
* **Direction_same:** 53.1% acceptance rate.\
* **Direction_opp:** 49.2% acceptance rate.\
Those traveling in the same direction have a slightly higher acceptance rate than those traveling in opposite directions (a difference of around 4 percentage points).\
**5) Morning vs Afternoon vs Evening:**\
* **Morning:** 54.2% acceptance rate.\
* **Afternoon:** 54.8% acceptance rate.\
* **Evening:** 41.5% acceptance rate.\
The evening shows a considerably lower acceptance rate compared to the morning and afternoon.  Morning and afternoon have very similar acceptance rates.\
**6) Sunny vs Rainy vs Snowy:**\
* **Sunny:** 50.4% acceptance rate.\
* **Rainy:** 52.2% acceptance rate.\
* **Snowy:** 43.2% acceptance rate.\
Rainy weather shows a slightly higher acceptance rate than sunny weather. Snowy weather has a significantly lower acceptance rate than both sunny and rainy weather.\
**7) 1Day vs 2Hour:**\
* **1Day:** 58.4% acceptance rate.\
* **2Hour:** 43.2% acceptance rate.\
There's a large difference in acceptance rates between those with a 1-day timeframe and those with a 2-hour timeframe.  The longer timeframe (1 day) has a much higher acceptance rate probably because the drivers can plan better to use the coupons.\
**In summary:**  Several factors consistently show a negative correlation with acceptance rates: longer wait times (GEQ15min, GEQ25min), evening time, and snowy weather. Conversely, shorter wait times (implied by the "All" cohort and others), younger age, and rainy weather show relatively higher acceptance rates.  The differences in acceptance rates between some categories are quite substantial, suggesting these factors are significant predictors of acceptance.\cf2 \
#Visualisation\
I plotted histograms for various columns to understand the kind of values each column held. The plots are present under the DataVisualizations folder.\
I plotted bar plots to compare the acceptance rates for each set of cohorts separately. The plots are present under the DataVisualizations folder, their names begin with \'93Coffee House\'94.\
\pard\pardeftab720\sa240\partightenfactor0
\cf2 # Next Steps\
\pard\pardeftab560\slleading20\pardirnatural\partightenfactor0

\fs26 \cf0 \cb1 \kerning1\expnd0\expndtw0 Based on analysis of coupon acceptance rates, here are some recommendations to improve acceptance rates:\
\
* **Focus on younger demographics (<25):**  This group shows significantly higher acceptance rates. Tailor marketing and coupon offers specifically to appeal to this age group. Consider using platforms and messaging styles popular with younger demographics.\
\
* **Prioritize same-direction trips:**  While the difference isn't massive, focusing on drivers traveling in the same direction as their destination could slightly improve overall acceptance.  This could involve targeted advertising or location-based coupon delivery.\
\
* **Morning/Afternoon campaigns:**  Concentrate marketing efforts during the morning and afternoon, as these periods show significantly higher acceptance rates than the evening.\
\
* **Reduce wait times/travel times:**  This is a major factor. Explore ways to reduce the travel time associated with redeeming the coupon, such as offering coupons closer to the driver's current location or partnering with coffee shops in high-traffic areas. This relates heavily to the GEQ5min, GEQ15min, GEQ25min categories, which demonstrate a strong negative correlation between wait time and coupon acceptance.\
\
* **Longer validity periods:** The 1Day vs 2Hour comparison highlights the importance of longer validity periods. Offering 1-day or even longer validity periods will significantly increase the chances of redemption.  Drivers need time to plan accordingly.\
\
* **Weather-based adjustments:**  The data clearly shows lower acceptance rates in snowy conditions.  Consider offering different or enhanced incentives during snowy weather to compensate for the decreased willingness to travel for a coupon.  Alternatively, temporarily suspend coupon offerings during extremely inclement weather.\
\
* **Time-of-day adjustments:**  While morning and afternoon are better, the evening's low acceptance suggests adjustments.  Perhaps a different type of offer (e.g., a smaller discount but more convenient location) might be more suitable for the evening.\
\
By implementing these recommendations, we can significantly increase the effectiveness of your coupon campaigns and achieve higher acceptance rates.  }