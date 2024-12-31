java cCIV6782 Climate resilient water infrastructure design – Coursework brief
Part 1 – Document analysis (35 marks)
Please pick one of the following three research papers:
A. Quinn et al. (2018). Exploring how changing monsoonal dynamics and human pressures 
challenge multireservoir management for flood protection, hydropower production, and 
agricultural water supply. Link
B. Bertoni et al. (2019). Discovering dependencies, trade-offs, and robustness in joint dam 
design and operation: an ex-post assessment of the Kariba Dam. Link
C. Murgatroyd and Hall (2021): Selecting Indicators and Optimizing Decision Rules for Long Term Water Resources Planning. Link
State which documents you chose and answer the following questions. Please note the hard limit
of two sides of A4 for answering all questions (either manuscript or typed in Arial 11).
Q1. State which documents you chose for the document analysis, and present the characteristics of 
the case-study it contains:
a. Which geographic area does it deal with?
b. What is the key water infrastructure considered here?
c. What are key water uses and / or water-related risks considered here?
d. Is it a planning problem, an operational problem, or both?
e. What is according to you the main engineering issue tackled in this work?
Q2. How is the problem framed: what is the XLRM?
Q3. Is robustness well-defined? Please justify. If yes, how are metrics M used to define it? If not, 
please propose a way it could have been defined and justify why it would be appropriate.
Q4. What are the key trade-offs discovered in the paper? Please state two ways in which the 
existence of trade-offs makes the problem “wicked” in this case, and why. 
Q5. This question is about the uncertainties considered in this document.
a. How are “well-characterised” uncertainties modelled? Give an example.
b. How are sources of “deep” uncertainty modelled? Give an example.
c. Please name a source of uncertainty that could or should have been included, but is not.
Q6. This question is about the stakeholders identified in the document.
a. Can you name them, identifying which ones have competing interests and which ones 
have synergistic interests?
b. Are the interests of all stakeholders identified in the papers evaluated through a 
metric? Please justify your answer.
c. Is there a stakeholder that you can think of that is not represented in this study?
[Indicative marking scheme: Q1 7 marks, Q2 8 marks, Q3 6 marks, Q4 5 marks, Q5 5 marks, Q6 5 
marks]
Part 2 – Water resource system analysis (65 marks)
For this part, you will submit a Jupyter Notebook with your commented code, including answers to 
questions. There is no length limit but concision will always be regarded favourably, and lengthy 
text is worth no extra points. You can (and probably should) reuse and adapt code from the 
tutorials when relevant. 
Throughout your submission, please document any use of Large Language Models (LLMs; or 
alternatively, attach a statement on that use, < 300 words). Remember that use of Generative AI is 
allowed as long as it follows the University’s guidance.
Each of you will be working a different set of input data. The column / line numbers associated with 
your coursework will be communicated to you by email within the next week under the subject line 
“CIV6782 Coursework data”.
Task A: Operating current infrastructure (25 marks)
Here is a schematic of a reservoir system serving water for irrigation and producing hydropower. 
There are also minimum ecological flow constraints downstream (Figure 1). The different uses are:
I. Minimum ecological flows Qeco to be met all of the time.
II. Meeting the irrigation demand Dirr (variable monthly, see data) served through a shallow 
intake.
III. Meeting domestic demand Ddom (also variable monthly), served through a deeper intake.
IV. Producing fir代 写CIV6782、Python
代做程序编程语言m power Pf, i.e., a level of hydropower production to be met at least 99% of the 
time. This level is specified in your data sheet. Note that in this case it will be enough to 
meet a release target (i.e. enough to produce Pf if the reservoir is full).
Figure 1. a) System schematic; b) Reservoir section.
Q1. Assume a standard operating policy (SOP). Use tutorials and associated Python code, and 
adapt them to produce a water balance of the reservoir for the 70-year daily inflow time series you 
have been given. Your model should also output the following:
● For the four uses above, reliability, resilience and vulnerability.
● For uses I to III, volumetric reliability.
● Average annual hydropower production, as well as a time series plot of annual hydropower 
production.
Q2. Still using code from the tutorials, propose alternative management policies that lead to a 
higher hydropower production. In particular:
a) Is there a way to increase power production (compared with SOP hydropower production), 
without affecting other water uses?
b) What uses appear to be in conflict? In synergy?
Q3. In a few sentences, can you describe what you perceive to be the main qualitative differences 
between the Conowingo reservoir case used in the tutorial and this case?
Task B: Planning problem and robustness (40 marks)
Let us now assume we are looking into expanding irrigated area from the current surface. We 
assume we scale up the current mix of crops: this means the relative month-to-month consumption 
will not change (or said otherwise, if we expand irrigation by 20%, demand during all months will 
increase by 20%). We are considering irrigation expansion up to a doubling in withdrawn volumes.
We also consider the possibility to reduce firm power requirements by up to 50% to protect 
irrigation water supply despite irrigation expansion.
We assume the following objectives:
1. Irrigation volumetric reliability, to maximise.
2. Post-development irrigated surface area, to maximise.
3. Firm power requirement, to maximise.
4. Reliability of firm power production, to maximise.
Q1. Please carry out a multiobjective analysis of irrigation expansion. Choose an appropriate 
visualisation strategy. Comment the results, in particular (but not limited to):
a) What objectives are in conflict? 
b) What uses are impacted by the irrigation expansion, and which aren’t?
c) How does the choice of policy from Task A (SOP or more hydropower-friendly) impact 
irrigation expansion?
d) How would you select three solutions (irrigation expansion + operating policy) to carry out a 
vulnerability analysis?
Q2. Let us now do a vulnerability analysis of the three solutions you chose. We assume flows 
could decrease by up to 50% on average, with low flows particularly affected, and flow variability 
will increase. We also assume climate change can increase crop irrigation demand (by up to 20%) 
and that domestic water demand may increase by up to 50%.
a) Use the method from Tutorial 3 to generate a range of plausible flows for your analysis.
b) Please conduct the vulnerability analysis to see in which climates the volumetric reliability 
of the most vulnerable use, as defined in Task A, falls below 85%. Please comment on the 
suitability of different designs.
c) According to you, what potential impacts of climate change, both on streamflows and on 
irrigation demands, are being left out in this robustness assessment?
Q3. Now imagine a 50% expansion of irrigated surface area is agreed upon, and decreasing firm 
power requirements are envisaged as an adaptation measure as / if supply-demand conditions 
deteriorate. 
a) Please describe your approach to implementing this adaptation measure, as well as the 
trade-offs this involves. 
b) Propose an adaptation plan following this approach.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
