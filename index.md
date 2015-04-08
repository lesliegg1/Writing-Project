---
title       : Halibut fishing in Seward, AK
subtitle    : A writing project presentation
author      : Leslie Gains-Germain
framework   : io2012    # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme: tomorrow
widgets : [bootstrap, quiz, mathjax] # {mathjax, quiz, bootstrap}
mode        : standalone
knit        : slidify::knit2slides

---



<style>
#slide-1 img{float:left;margin:auto; padding:8px;}
</style>

<center>
<img src="~/Documents/WritingProject/presentation/images/maphang2.jpg" alt="fish" style="width: 850px;"/>
</center>





--- .class1 #id1 bg:darkcyan

<br><br><br><br><br><br><br>

<link href='http://fonts.googleapis.com/css?family=Amatic+SC:700' rel='stylesheet' type='text/css'>

<font style="font-family: 'Amatic SC', cursive;font-size:72pt!important"; color:red color=ivory>

<center>
"We travel farther for smaller fish" </center> </font>



--- .class1 #id1 bg:grey
## Questions of Interest
<font size=5 color:inherit>
Data from Alaska Department of Fish and Game
</font>

<font size=6 color=aliceblue> **Question 1**: Is there evidence that the distance Seward charter boats travel to fish for bottomfish has changed over the years 1993-2014?  </font>
<center>
<font size="6" color=gold>
Logbook Data <br>
<br>
Interview Data 
</font>
</center>

<br><br>
<font size=6 color=aliceblue> **Question 2**: Is there evidence of a change in the mean length of halibut caught by Seward fishermen over the years 1994-2013? </font>
<br>
<center>
<font size="6" color=gold>
Biological Data
</font>
</center>

--- &vcenter
## Data Reference

<ol>
<li>
ADF&G Saltwater Logbook Database [Intranet]. 2004–2013. Anchorage, AK: Alaska Department of Fish and Game, Division of Sport Fish (cited 4/2/2015). Custom query details available upon request from ADF&G, Division of Sport Fish, Research and Technical Services.</li>
<br>
<li>
ADF&G non-confidential data. 1993-2014. Homer, AK: Alaska Department of Fish and Game, Division of Sport Fish. Personal communication, Scott Meyer.</li>
<br>
<li>
ADF&G non-confidential data. 1994-2013. Homer, AK: Alaska Department of Fish and Game, Division of Sport Fish. Personal communication, Scott Meyer.</li>
</ol>

---
## Logbook Data 2004-2013

<center>
<img src="~/Documents/WritingProject/presentation/images/logpage.png" alt="map" style="width: 900px;"/>
</center>

---

<center>
<img src="~/Documents/WritingProject/presentation/images/statchart.png" alt="map" style="width: 850px;"/>
</center>



---

<center>
<img src="~/Documents/WritingProject/presentation/images/twodmap.png" alt="map" style="width: 800px;"/>
</center>

<!---![twodmap](twodmap.png)--->





---

<center>
<img src="~/Documents/WritingProject/presentation/images/twodmapindareas.png" alt="map" style="width: 800px;"/>
</center>



---
## Logbook: 2004-2013

![plot of chunk logplot](assets/fig/logplot.png) 

---
## Interview Data 1993-2014

<center>
<img src="~/Documents/WritingProject/presentation/images/jacksparrow.jpg" alt="jack" style="width: 300px;float:right; padding: 10px; padding-top:initial"/>
</center>

<ul style="list-style-type:circle">
<li>Two days a week randomly selected for interviews </li>
<li>Effort spread across the four harbor cleaning stations </li>
<li>Each boat is asked:</li>

<ul style="list-style-type:persian">
<li>Did you catch bottom fish today?</li>

<li>If yes, record trip type</li>

<li>Identify the primary statistical area where the majority of bottomfish were caught.</li>
</ul>
</ul>

<br>


|abbreviation |description                                                                     |
|:------------|:-------------------------------------------------------------------------------|
|H            |halibut exclusively                                                             |
|B            |any combination of bottomfish (halibut, rockfish, lingcod, Pacific cod, sharks) |
|B+S          |any combination of bottomfish and salmon (e.g. halibut+coho)                    |

---
## Interview 1993-2014

![plot of chunk intplot](assets/fig/intplot.png) 



---
## Comparison- Cape Cleare

![plot of chunk compare](assets/fig/compare.png) 



---

## Fitted Probabilities and 95% Pointwise CIs

![plot of chunk fitplots](assets/fig/fitplots.png) 

---

The odds of fishing in Cape Cleare in $2014$ are estimated to be $2.43$ times the odds of fishing in Cape Cleare in $1993$, with a $95\%$ confidence interval from $1.22$ to $4.92$ times. 

The odds of NOT fishing in Resurrection Bay in $2014$ are estimated to be $2.78$ times the odds of NOT fishing in Resurrection Bay in $1993$, with a $95\%$ confidence interval from $1.32$ to $5.82$ times.

![plot of chunk confintgraphs](assets/fig/confintgraphs.png) 




---
### **Question 2**: Is there evidence of a change in the mean length of halibut caught by Seward fishermen over the years 1994-2013?</li>

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1.png) 

---
## Biological Data 1993-2013
<center>
<img src="~/Documents/WritingProject/presentation/images/jacksparrow.jpg" alt="jack" style="width: 300px;float:right; padding: 10px; padding-top:initial"/>
</center>

<br>
<ul>
<li> Three days a week randomly selected for biological sampling </li>
<li> Boats selected (non-random) and entire catch is studied </li>
</ul>

<br><br>


|port   |sector  |    date| age| length|sex | statarea| length.in|area       |
|:------|:-------|-------:|---:|------:|:---|--------:|---------:|:----------|
|Seward |Charter | 5261994|  11|  120.0|F   |   495938|     47.24|resbay     |
|Seward |Charter | 5261994|  NA|  128.0|F   |   475934|     50.39|capecleare |
|Seward |Charter | 5261994|  13|   85.0|M   |   475934|     33.46|capecleare |
|Seward |Charter | 5261994|  13|   85.5|M   |   475934|     33.66|capecleare |
|Seward |Charter | 5271994|  11|  126.5|F   |   485935|     49.80|junken     |
|Seward |Charter | 5271994|  11|   95.8|F   |   475934|     37.72|capecleare |


---

<center>
<img src="~/Documents/WritingProject/presentation/images/biomap.png" alt="map" style="width: 800px;"/>
</center>



---
## Average fish lengths plotted over time

<br>

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2.png) 

--- 
In the waters around Cape Junken, there is strong evidence of a relationship between mean fish length and time over the years $1994$ to $2013$ (p-value$<0.0001$ from t-stat$=-5.370$ on $18$ df).








![plot of chunk plots2compare](assets/fig/plots2compare.png) 


---

The mean fish length in Cape Junken in $2013$ is estimated to be $6.8$ inches shorter than the mean fish length in Cape Junken in $1994$, with a $95\%$ confidence interval from $4.35$ to $9.29$ inches shorter.


![plot of chunk results3](assets/fig/results3.png) 


---

<center>
95% CI for change in fish length 1993-2014 in Cape Cleare <br><br>
OLS-black dashed line (-9.40, 1.37) <br>
</center>

<center>
WLS-blue line (-10.40, -2.27)  <br>
</center>

<center>
Mixed Effects-red line (-9.35, -0.18)
</center>

![plot of chunk el](assets/fig/el.png) 



---
## Scope of Inference

<br><br><br><br>
<font size=6>
Technically does not extend to all Seward boats/fish, 
BUT....
</font>
<br>
<br>
<br><br><br>
<font size=6>
No causal
</font>

---.class1 #id1 bg:#CBE7A5
<br>
<br>
<br><br><br>
<center>
<font size=7>
**Questions?**
</font>
</center>

--- 
## Comparison - Resurrection Bay

![plot of chunk compareres](assets/fig/compareres.png) 

---
## Comparison - Patton Bay

![plot of chunk comparepatton](assets/fig/comparepatton.png) 

--- 
## Quasibinomial Logistic Regression

![plot of chunk binlog](assets/fig/binlog.png) 
<br>

<!--<center>$logit(p_{i})=\beta_0+\beta_1year_i$</center>-->

<!--<center>$i \in (1993, 1994,..., 2014)$</center>-->

<center>
<ul style="list-style-type: circle; width:686px; margin:auto">

<li>Each area modeled separately</li>

<li>Assumptions</li>
<ul style="list-style-type:persian">
<li> Independence </li>
<li> Linearity </li>
<li> Outliers </li>
</ul> </ul>

</center>


--- .dontcount
## Results

There is moderate evidence that the log odds of fishing at Cape Cleare changes over time, assuming a linear trend over years $1993$ to $2014$ (p-value$=0.02479$ from drop-in-deviance F-stat$=5.89$). 

<br>


|           | YEAR coef|     SE| F-stat| Pr(>F)|
|:----------|---------:|------:|------:|------:|
|capecleare |    0.0404| 0.0161|  5.891| 0.0248|
|resbay     |   -0.0463| 0.0171|  7.351| 0.0134|
|nuka       |    0.0188| 0.0385|  0.238| 0.6309|
|patton     |    0.0760| 0.0200| 12.532| 0.0021|


--- .dontcount
## Mixed Effects Model
Each area modeled separately

<br>
<br>

<center>$length_{i}=\beta_0+\beta_1year_i+\alpha_{i}+\epsilon_{i}$</center>

<center>$\epsilon_{i} \overset{iid}{\sim} N(0, \sigma^2)$</center>
<center>$\alpha_{i} \overset{iid}{\sim} N(0, \sigma^2_{\alpha})$</center>
<br>
<center>$i \in (1994, 1995,...,2013)$</center>

---

![plot of chunk test](assets/fig/test.png) 
