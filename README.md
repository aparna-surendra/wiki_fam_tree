# wiki_fam_tree
## Objective: Construct a family tree for persons of interest using Wikipedia 
This code takes a csv file with names (in this instance, the world leaders list from the Open Sanctions website) and scrapes wikipedia to identify relatives. (The Wikipedia 'infobox'  does not have a standardised structure across pages) <br> 
It outputs a new csv file, 'wikipedia_family_tree.csv', with the following columns: 
<ul> 
<li> key (person of interest) </li>
<li> source (link to source wiki page)</li>
<li> relationship (first letter represents: 'Spouse', 'Partner', 'Children', 'Parent', 'Relatives','Family')</li> 
<li> name (of relative) </li> 
<li> wiki_link (for relative, if available) </li> 
<li> notes (any additional detail) </li>
</ul>

TO DO:
<ul> 
<li>More robustly extract family information (outside rule-based methods?) </li> 
<li>Extend to second and third-order relationships and manage duplicates </li> 
<li>Model family networks e.g. using visualisations </li> 
<li>This code works for prominent people (e.g. world leaders) - assess whether it extends to less prominent people (whose wiki pages may be differently structured) </li> 
</ul> 
