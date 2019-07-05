# wiki_fam_tree
## Sri Lankan state-owned enterprises - scraping management information from CSE.lk 
Data on state-owned enterprises (SOEs) is surprisingly sparse. This code scrapes the Colombo Stock Exchange website to collect board of director data for listed SOEs, to assist an SL-based civil-society organisation. The resulting CSV file will feed into a larger project, a database for politically-exposed persons. 

The output CSV file has the following columns: 
<ul> 
<li> <i>Name</i>: Scraped from respective company's CSE.lk profile </li>
<li> <i>Role</i>: E.g. Board Member, CEO, Chairperson. </li>
<li> <i>Notes</i>: Additional detail on role </li> 
<li> <i>Company_Name</i>: Name of company, as searched for.  </li> 
<li> <i>CSE_Name</i>: Name of company, as listed on Colombo Stock Exchange. </li> 
<li> <i>CSE_Symbol</i>: Company symbol, as listed on Colombo Stock Exchange. For each company, the data is scraped from www.cse.lk/home/company-info/CSE_symbol/company-profile. </li>
<li> <i>Retrieved</i>: Day/Month/Year. Date the data was scraped. </li> 
<li> <i>Check_Needed</i>: Boolean, True/False. If the Company_Name does not exactly match CSE_Name, this is True. Flags row for an additional manual check. </li> 
</ul>

This preliminary code serves as a proof-of-concept, and runs on a list of 17 plantation companies to produce 'regional_plantation_companies.csv'. 

TO DO:
<ul> 
<li>Clean code (object-oriented; better manage global/local variables) </li> 
<li>Create a CSV file with names of all SOEs. In this version, I have manually entered the list of company names (and I only have a hard-copy of the 300+ SOEs). Scrape Treasury page? </li> 
<li>Create a CSV file with all CSE company symbols. Currently, there is no comprehensive list of companies and their correspondng CSE symbol. This code searches the CSE website and identifies the symbol through the auto-complete drop-down menu, which limits fuzzy-matching options. </li> 
</ul> 
