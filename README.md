# How and Where Did People Die On The Job?
I scraped and analyzed workplace death cases recorded by the Department of Labor's Occupational Safety and Health Administration (OSHA). The folders contain notebooks, maps, and Datawrapper visualizations. 
---------
As my semester one final project, I used Playwright to scrape the OSHA website where the agency lists the [cases of workplace deaths it inspected](https://www.osha.gov/fatalities), and analyzed them using pandas and regex. Data between January 2017 and November 2022 was available. 6498 rows were analyzed, as I removed two repeat cases (there were 6,500 cases when I last scraped the data on January 6, 2023). COVID-19 related deaths are not included.

![OSHA fatilities cases by year](https://user-images.githubusercontent.com/116761949/211128514-9a095ba3-deee-4d43-ae56-fd25be4c1e56.png)

![OSHA fatilities how they died](https://user-images.githubusercontent.com/116761949/211128525-6b6a6063-bc6c-4b37-a3f4-f49a488e7459.png)


While Texas, California, and Florida had the most number of workplace deaths during this period, these are also the three largest states in the U.S. If you look at the number of deaths per state population, Oregon, North Dakota, and Wyoming had a higher rate. Only states were mapped — U.S. territorities were not. 


![OSHA fatilities death per state absolute figures](https://user-images.githubusercontent.com/116761949/211128472-3c923c91-bc7b-4f0a-bd54-5d13597e6971.png)


![OSHA fatilities deat per state rate](https://user-images.githubusercontent.com/116761949/211128439-5ae8f038-350f-45d4-8a78-e476a16c4c0a.png)


To scrape each case's union status, I used BeautifulSoup to extract the information. I managed to compile 6,433 cases, which showed that nearly 90% of all cases involved non-unionized workers. 


![BVRD3-most-cases-involved-non-unionized-workers](https://user-images.githubusercontent.com/116761949/211128577-4399988a-8ae8-4d3b-8689-0c8c63139a72.png)


The number of workplace deaths have been falling since 2019, but this could be due to the pandemic, when many companies stopped worked and workers stayed home. The number of cases do not tally with the total number of workplace deaths recorded by the Bureau of Labor Statistics (BLS). For example, in 2021, BLS reported 4,764 fatal work injuries in 2021. OSHA’s data only showed 970. OSHA has said on its website that the information is not comprehensive.  
