---
layout: post
title: Not Easy to Become A Qualified Data Scientist
---

The word “Data Scientist” has been over used. From my understanding, a data scientist can be defined as:
He should be an expert in the file of Statistics (ie. Applied Regression, Multivariate analysis…), Modeling, Data Mining, Professional Tools/Language (ie. SAS, R, Python, Hadoop, SQL, Weka, Matlab, SPSS…), data visualization (Tableau, SAS…), and a good communicator and a Business savvy.
For the responsibility of the Data Scientist: 
He/She usually processes big volume of data, say gig bite. Excel can hardly handle that huge volume. 
He/She should know how to get/collect data, clearance, integrate, process, program…

Finally, to become a data scientist, you need to prepare to learn, all your life, all the time.

Thoroughly understand the business you are conducting, which includes: 
What’s your business about? 
How to generate profit? 
What are the penchants/habits of your customers/competitors/partners/distributors? 

This process is always been ignored by many data scientists/analysts. They believe they have enough skills at coding and statistics. Unfortunately, because of lacking the understanding of their business, they cannot even design a decent experiment. Say nothing about identifying confounders.

I recently read an example on Statistics (3rd Ed, by David Freedman, Robert Pisani, Roger Purves) about how NFIP study was biased against the vaccine. Experiment designers obviously ignored many effects of control group, and made the results of experiment less convincing. 

People might say: you don’t need to understand everything about your business which is impossible, but you need to communicate well with those business insiders to get suggestions from them. That could be correct. But many situations like this happen every day:
Data Scientist: “Our experiment failed because we ignored the factor that actions of readers using different devices are totally different.  Hey Jim, why didn’t you tell me that before we conduct the experiment? “
Jim: “You designed the experiment, but you didn’t ask me the influences of devices, how can I tell you something you didn’t ask? And how did I know whether you realized it would become a potential problem? ”


Another problem is: under many situations, experiments failed for reasons unknown.
An example is doing A/B tests before officially release a marketing plan/pricing strategy. It can also test are your website campaign pages effective.  

A B2B eCommerce company decided to expend their business by inviting more websites join their promotion alliance. “Put your products on our website for free, we sell you back the registered information or leads”. But they don’t know which pricing model to use: 1. First 5 pieces of information with 20% discount, 2. No discount.  So they decided to make A/B test. 

Imagination: Example from text book: 

Here is the formula: 

$$Z = \frac{P-P_c}{\sqrt{\frac{P (1-P)}{N}  + \frac{P_c (1-P_c)}{N_c}}}$$

Find 200 companies, send different offers, and use hypothesis test formula to see how significant the result is, then decide which pricing model is better.  Job done and everything is perfect!


Reality:   It’s easy to say and imagine, but not easy to do.

Their first step was to know who to invite and who to contact with. The analyst ran inquiry on their paid database and their own CRM system to find companies in B2B industries or manufacturers. Then she unified, cleaned, merged, and de-duped the company lists and generated a master list with more than 1000 potential partners. In order to find the appropriate contacts from each company, they asked help from their agent to append contact information with targeted job titles. Only 677 companies were found in their database and been appended with contact information, including name, email, title, business phone, cellphone, address, LinkedIn URL. For some small companies, there is only one contact; for the big ones, there are more than 200 contacts. Meanwhile, because the appended data was also not cleaned and de-duped, the data analyst cleaned the list again and chose at most 2 contacts from each company.

Next step was to pick up 200 companies to make this test. One most important principle of A/B test is: Experimental and control groups should be as similar as possible in order to limit other possible influential factors.  So they went through company size, business, location, industry, contact job position manually and carefully chose 200 companies for the tests, and set each company an authority file in their system.  As I mentioned before, some companies were from their CRM system, from where they can send out invitation emails. For the rest, they planned to do that under the help of agent. 

They prepared 2 versions of invitation letters with same wordings and format, but different offers.  All emails were sent simultaneously on Tuesday morning 10:00am. 

And they waited for response. They estimated there will be 20% of people replied. In fact, only 4 emails were clicked open but without any further action. What happened? Were the invitation emails went to junk files or been identified as spams?  Or the contact emails were not been used anymore? Or did we find the wrong companies or wrong people? They decided to call those contacts who clicked open the emails to find out what’s going on. And the problem was they cannot get through those phones, even they finally found the people, he/she said: “I don’t remember that email” or “We are not interested.”

Finally, the project postponed and they never got a chance to use the hypothesis test. 


