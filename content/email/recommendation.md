/*
Title: Before & After: Technical Recommendation
*/





### Technical Recommendation Email


## Before

**Subject: Omniture vs. Engine Performance Variance Questions** 

Hey J--

Over the last few weeks we have been in the process of verifying all of the scripting that was placed/fixed in the last deploy and part of that has been comparing what Omniture is seeing versus what the engines are recording. So since the March 2nd deploy I have been recording both tracking sources figures every few days and I am seeing some odd things that I wanted to bring to your attention and, most importantly, get your opinion on.

Let me first say that right after the deploy I conducted multiple conversion tests and each one of my tests have tracked accurately in both Engine and Omniture. This fact makes the below items even more confusing.

**Tracking off in the First Week of Performance**

As I recorded the first few days’ worth of data (March 2nd through March 7th), I saw some odd things coming through. We’ve talked in the past about how these tracking sources record sales differently (Engine is day of click and Omniture is day of conversion), we were seeing the Engine track roughly 22% more sales than Omniture was seeing (127 in engine vs. 104 in Omniture) for the main US/Canada campaigns (tracking code would be an advanced search for “any” “KNC- express ppc” & “KNC- xilinx ppc”). Now the sales data wouldn’t seem too strange, but knowing that Google would be actively attributing sales back to the February (based off of day of click tracking), Omniture should actually be considerably higher in sales knowing that all of Omniture sales would have happened actually in that time span. 

**Tracking off for Month to Date** 

Performance (Average Revenue per Sale)
Yesterday I ran performance figures for month to date (up to 5pm on 18th, so some of the figures have probably increased slightly since I ran the reports) and the data shows that the variance between Omniture and Engine tracking sales in the first week-ish of the month is no longer present when looking at a larger picture of the month, though we are still seeing some other items that we’d like to bring to your attention. Even though I have gone in and scoured the sales confirmation page to the best of my ability for any issues and haven’t found any, we are currently seeing Omniture report a significant amount higher revenue per sale for conversions that occurred in March to date. Omniture is reporting $305.48 average revenue per sale and the Engines are seeing $188.29 for the main US/Canada campaigns. Knowing that I have conducted multiple conversion tests which have tracked accurately in the engine & Omniture, I am just at a loss at for how this could be happening.

Also, in general the Average revenue per sale being seen in Omniture is pretty low compared to previous months with the same budgets and strategy. As I mention above, March to date is seeing $305.48 average revenue per sale, while December saw $451.71, November saw $402.45 & October saw $497.30. These variances may not seem like a lot been when this is across the 418 sales that Omniture is seeing in March so far (US/Canada campaigns), it quickly adds up.

Additionally, from March 1 till March 18, the engines are currently showing just over 14,300 clicks and Omniture was only seeing 9,100. Could this be a sign that Omniture is not implemented on every page? I have literally zero experience with implementing Omniture, so I have no idea if that is even a valid hypothesis, but I figured it couldn’t hurt to ask.


**Significant Difference in Co-Op/ Business Unit Performance** 

March to date is seeing some extremely varied performance across all of our campaigns when comparing Engine vs. Omniture (and a lot of the time it is not showing that omniture is reporting higher than engine. I have listed some of the most significant examples & their omniture tracking codes below:

US/Canada:

* Engine: 385 Sales, $72,490.96 revenue
* Omniture:418 Sales, $127,690 revenue
* (tracking code would be an advanced search for “any” “KNC- express ppc” & “KNC- xilinx ppc”)

Analog Devices:

* Engine: 7 Sales, $485.25 revenue
* Omniture: 8 sales, $113.00 revenue
* (tracking code would be a search for “knc - adi ppc”)

TE Connectivity:

* Engine: 30 Sales, $5,027.78 revenue
* Omniture: 3 Sales, $641 revenue
* (tracking code would be a search for “knc -TE ppc”)
 
Texas Instruments:

*   Engine: 21 Sales, $2,666.50 revenue
*   Omniture: 11 sales $186.00 revenue
* (tracking code would be a search for “knc-TI ppc”)

So in order to validate our engine data I have a process where I go through the source codes where the scripting is implemented and look for specific parameters in the code to validate that it’s been implemented correctly. Is there any formal Omniture verification process that you have, or could possibly, go through to verify the implementation is accurate?

I know that it’s a lot of information to digest and I am sure you will have some follow up questions, so please let me know where I can clarify and what add’l info I can provide!


Side note: Chris and I are still very interested in what Adobe’s Adlens product has to offer. On one of our reporting calls yesterday we asked Steve if Adobe had provided pricing yet, and he said to talk to you about where that conversation was going. At the end of the day, if Adlens’ price is right we might just want to leverage that tool (& thus scripting) for all of its added capabilities and interesting attribution abilities.


Thanks for your thoughts on all of this in advance, it is greatly appreciated!

## After


**Subject: Are we sure Omniture is correctly implemented in all web pages?**

Hey J--

Engine appears to be tracking 22% more sales than Omniture. This is strange because Omniture should skew higher due to the differences in the way Omniture and Engine track sales. (Point of Conversion v. Point-of-Click)

In addition, I'm seeing strange variances in average revenue per sale. And wildly varied performance reporting from Omniture to Engine. I've attached a spreadsheet showing the discrepancies for first week, business unit and month-to-date performance. 

The only think I can think of is that Omniture isn't correctly implemented in all of the site pages. Can you look into this?

Thanks very much, 

--J