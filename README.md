<p align="center">
   <img src=https://github.com/yeagercmbpd/Identifying_Victim_Clusters_In_Baltimore_CIty_Police_Data/blob/main/patch.png>
<div align="center">
   <figcaption></figcaption>
</div>
</p>

Identifying Victim Clusters in Baltimore City Police Data
---
Utilizing KMeans clustering and crime data for segmentation of the victim population of Baltimore City

---
### Overview and Project Goals
The purpose of this analysis is to attempt to detect hidden groupings within crime victim data from Baltimore City. We will then assess the information from these groupings as well as join demographic info to creat victim profiles. These profiles will help police target individuals for crime prevention efforts, assist in crime investigation, and proactive deployment of resources.

---
### Repository Navigation
<pre>
Technical Notebook: <a href=https://github.com/yeagercmbpd/Identifying_Victim_Clusters_In_Baltimore_CIty_Police_Data/blob/main/Detecting%20Victim%20Groupings%20in%20Baltimore%20Crime%20Data.ipynb>Technical Notebook/Report</a>

</pre>
---

## The Data
The primary dataset which will be used in this analysis is the victim based part 1 crime table, produced by the Baltimore City Police Department. [https://data.baltimorecity.gov/api/views/wsfq-mvij/rows.csv?accessType=DOWNLOAD](https://data.baltimorecity.gov/api/views/wsfq-mvij/rows.csv?accessType=DOWNLOAD). It reports crimes based upon each victim, rather than occurance, and thus each row can be thought of as a victim. The dataset at the time I accessed it consisted of almost 280,000 records and 22 columns. Due to its volume, I decided to focus on the most recent year of data. The data is maintained by the department and updated frequently for accuracy. 

Features are reported in various formats, including continuous  and categorical. 

In the second half of the analysis a shapefile containing census data for each neighborhood within Baltimore is joined to this crime data. It was compiled using data from the most recent 2010 census and is part of a program managed by the city known as 'vital signs'
[https://data.baltimorecity.gov/api/views/2ktz-dadz/rows.csv?accessType=DOWNLOAD](https://data.baltimorecity.gov/api/views/2ktz-dadz/rows.csv?accessType=DOWNLOAD)

---

## Summary

**Part 1: Crime data only**

  Clusters found with moderate density and variation. Looking strictly at the data available within this set did not yield much in the way of insight.
   
**Part 2: Incorporating demographic data into the victim data**

   Much more distinct clusters identified. interesting patterns which fall in line with outside analysis identified. Basic victim profiles could be generated.
   
## Lessons Learned / Looking Forward
Dimensionality reduction became neessary to complete the analysis and model upon adding all of the additional features within the census based data set.
Having access to individual victim information rather than generalizing it basd on census data would lead to an incredibly more specific result and allow for a very powerful clustering model. 
  
---
## PackagesandCredits
<pre>
By : <a href=https://github.com/yeagercmbpd>Christopher Yeager</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Jupyter
Libraries    : pandas, numpy, matplotlib, sklearn, seaborn,yellowbricks,geopandas
</pre>
