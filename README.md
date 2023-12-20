# klantenboek-hj-zandhuis
Data from the 1907 customer registration of village blacksmith H.J. Zandhuis (1884-1938) in Wijhe (NL)

## Source
In my family a customer registration has survived of blacksmith Harm Jan Zandhuis (1884-1938) in [Wijhe](http://www.wikidata.org/entity/Q3164650), a village in the province of Overijssel in the Netherlands. The fact that the registration starts halfway May and Zandhuis' age (22) at the time of creation (1907), suggest that it is the year he started to work on his own account. He and his descendends kept this customer registration as a souvenir, because it probably was the oldest one in a series where newer ones were thrown away.

The registration contains an index were the names of customers are alphabetically entered, with a reference to the page were the work he did for this customer was registered. On the page the date, work/product and price is notated.

TBD: Add picture

## Data
This dataset contains two tables, one with an overview of the customers ([klanten](data/klanten.csv)) and one with the work and product that HJ Zandhuis sold (['werkzaamheden'](data/werkzaamheden.csv)). Based on the available data (sometimes only a familyname) I try to find more information on the customer in the population registration of the municipality of Wijhe. This is added to the first table. The second table contains the work the blacksmith has done, the date and the price in Dutch guilders (note that in 1907 prices could have half cents, so three decimals are needed). This table refers to the customer in the first table through the pagenumber ('fol').

TBD: create a third table with a structured vocabulary of the things he handled and the handling itself (eg. 'paard' and 'beslaan', or 'wagen' and 'repareren'). This in order to standardize the werkzaamheden and use that for analysis.

## Analysis
I use [python/pandas in a Jupyter Notebook](analysis.ipynb) to get some insight on the work of a blacksmith in a Dutch farm village, early twentieth century.
