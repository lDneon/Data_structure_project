# Data_structure_project

This project is designed to reinforce OOP system design and separation of concerns,  data structures + Big O thinking, and practical use of iteration/transformation methods to analyze real data.

**Air quality & Asthma rates**
**Thesis**: Cities in the U.S. with higher annual PM2.5 concentrations are associated with higher overall asthma prevalence rates.

Asthma prevalence is computed using adult estimates.

**Data:**

OpenAQ API: https://openaq.org/developers

CDC API: https://data.cdc.gov/resource/qnzd-25i4.csv?$query=SELECT%20year%2C%20locationname%2C%20datasource%2C%20category%2C%20measure%2C%20data_value_unit%2C%20data_value_type%2C%20data_value%2C%20data_value_footnote_symbol%2C%20data_value_footnote%2C%20low_confidence_limit%2C%20high_confidence_limit%2C%20totalpop18plus%2C%20totalpopulation%2C%20geolocation%2C%20locationid%2C%20categoryid%2C%20measureid%2C%20datavaluetypeid%2C%20short_question_text%20SEARCH%20%22asthma%22

**Sources:**

https://www.health.ny.gov/environmental/indoors/air/pmq_a.htm

https://pmc.ncbi.nlm.nih.gov/articles/PMC7503605/


**How to run** --> git clone <https://github.com/lDneon/Data_structure_project> 
cd <>

in terminal: pip install requests numpy --> then run python AirAsthma.py --> then follow CLI menu


**Data structures used + Big O notes**

**Most operations in this project are linear time O(n), while sorting operations for top polluted locations run in O(n log n).**

**Array/list:** I used listd to store cleaned asthma rows and raw API rows.The data is processsed through cleaning, filtering, and analysis.

*appending records (amortized O(1) because it does not rely on random input)

* filtering all records O(n)

**Dictionary:** To group PM2.5 readings by location and to look up asthma prevalence by location while joining the datasets.

*lookup by key (avarage O(1))

*grouped all rows O(n)

**Set:** removes duplicate locations and find the intersection of locations that appear in both datasets.

* check membership (O(1) average)

* deduplication across n items O(n)

**Methods :**
Collected PM2.5 air quality data from openAQ API and loaded asthma prevalence data from CDC dataset. while also applying a *what-if* filter by excluding extreme PM2.5 outliers. Other methods used was; removed null values, converted strings to numeric values, and standardized location names.


**Findings :**


**Test Evidence**


**Conclusion :** 



  
