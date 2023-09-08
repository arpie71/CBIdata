# Description of the CBI data files 

<h2>Data</h2>
This folder contains versions of the raw data in 3 file formats: <a href='cbi2021.dta'>Stata</a>, <a href='cbi2021.xlsx'>Excel</a>, and <a href='cbi2021.csv'>csv</a>. 

Each file contains the country name, Correlates of War country code, year, lvaw, lvau, and the 16 components of the CWN index. Additionally, we provide the scores for the 4 aggregated categories: CEO, policy, objectives, and other limitations on lending. 
<ul>
<li><b>CEO</b> is comprised of an equal weighting of the following four indicators: <i>term of office</i>, <i>who appoints</i>, <i>dismissal</i>, and <i>other offices</i>.</li>
<li><b>Policy</b> is a weighted average of 3 indicators. <i>Who formulates</i> and <i>role in budget</i> both have weights of .25 and <i>final authority</i> has a weight of .5.</li>
<li><b>Objectives</b> is just the single indicator <i>objectives</i></li>
<li><b>Other limitations on lending</b> is an unweighted average of 4 indicators: <i>type of lending limit</i>, <i>maturity of loans</i>, <i>interest rates</i>, and <i>primary market</i></li>
</ul>

The <b>lvau</b> variable is comprised of the unweighted average of 8 indicators: ceo, policy, objectives, other limitations on lending, advances, securitized lending, terms of lending, and potential borrowers. If one of the indicators is missing, the denominator is adjusted. For example, if advances is missing the denominator becomes 7 rather than 8. 

The <b>lvaw</b> variable is made up of the same 8 indicators, but each indicator is weighted separately. CEO has a weight of .2, policy and objectives have weights of .15 as does advances; other limitations of lending, securitized lending, and terms of lending have weights of .10; finally, potential borrowers has a weight of .05. When an indicator is missing, the denominator is adjusted by subtracting the weight of the missing indicator. For example, if advances is missing, the denominator becomes .85 rather than 1.

Complete details of the coding scheme are available in:  
Cukierman, Alex, Steven B. Webb, and Bilin Neyapti. 1992. Measuring the Independence of Central Banks and Its Effect on Policy Outcomes. <i>The World Bank Economic Review</i> 6(3): 353–98.

