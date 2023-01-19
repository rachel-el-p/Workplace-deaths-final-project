# How and Where Did People Die On The Job in the U.S.?
I scraped and analyzed workplace death cases recorded by the Department of Labor's Occupational Safety and Health Administration (OSHA). The folders contain notebooks, maps, and Datawrapper visualizations. 
---------
There are a total of 6,500 cases on the website. I removed two as they were repeated
cases, and analyzed 6,498 cases. Scraping the union status required an additional step of
going into each case and extracting the information, and I managed to get 6,433 cases, which I believe is still sizable:

## Number of Cases 

Workplace deaths in the U.S. have been falling since 2019, according to cases inspected by
the Department of Labor's Occupational Safety and Health Administration (OSHA)
between January 2017 and November 2022.

![OSHA fatilities cases by year](https://user-images.githubusercontent.com/116761949/211128514-9a095ba3-deee-4d43-ae56-fd25be4c1e56.png)

However, this could also be due to the pandemic, when some companies stopped worked and their
workers stayed home. Or that OSHA has not updated the table to include more recent cases. OSHA 
states on its website that the information is not comprehensive and is updated when the data becomes available.

The number of workplace deaths on OSHA's website do not tally with the [Bureau
of Labor Statistics' (BLS) data](https://www.bls.gov/news.release/cfoi.htm). For example, BLS' data showed there were 5,190 fatal work injuries in 2021, up from 4,764 in 2020. In 2019, there were 5,333 deaths.

Jordan Barab, a former deputy assistant secretary at OSHA who worked at the agency between 2009 and 2017 and writes the [workplace safety "Confined Spaces" blog](https://jordanbarab.com/confinedspace/), told me there are several reasons why OSHA's count is lower than BLS'.

Public employees in 23 of the 50 states — excluding the District of Columbia, and U.S. territories — are not covered by the agency, and these include workers who work in public hospitals, water treatment plants, and on highways.
Situations that are under the police's jurisdiction are also not investigated by OSHA. For example, a shooting
at a convenience store would be turned over to law enforcement. Agencies like the Federal Aviation Administration and the Department of Energy also handle their own cases.
Furthermore, self-employed workers such as ride-hailing drivers and delivery workers are not under OSHA's jurisdiction. </p>
    
## How Workers Died 

Most workers died by falling or being struck by objects. Covid-19 related deaths were not counted in this analysis.

![OSHA fatilities how they died](https://user-images.githubusercontent.com/116761949/211128525-6b6a6063-bc6c-4b37-a3f4-f49a488e7459.png)

Barab said that both OSHA and BLS hardly count deaths that stem from work-related illnesses — OSHA has a separate 
table for COVID-19 deaths but these number only 2,137 — and this is an issue, though he understands it is difficult to trace
as the death could occur many years after the cause, say cancer 20 or 30 years after exposure to asbestos. 
[A report](https://aflcio.org/reports/death-job-toll-neglect-2022#:~:text=4%2C764%20workers%20were%20killed%20on,the%20job%20than%20all%20workers.) published in 2022 by the trade union AFL-CIO, the largest labor union organization in the U.S., said that an estimated 120,000 workers 
die each year from occupational diseases, or about 340 workers a day. 

## Where Workers Died

Texas, California, and Florida had the most number of workplace deaths during this period,
but these are also the three largest states by population in the country. After accounting
for population, Oregon, North Dakota, and Wyoming were the three states with the highest rate
of workplace deaths per population. 


![OSHA fatilities death per state absolute figures](https://user-images.githubusercontent.com/116761949/211128472-3c923c91-bc7b-4f0a-bd54-5d13597e6971.png)


![OSHA fatilities deat per state rate](https://user-images.githubusercontent.com/116761949/211128439-5ae8f038-350f-45d4-8a78-e476a16c4c0a.png)

Only states were mapped — U.S. territorities were not. OSHA also investigates deaths in territories. 
There were 46 cases in Puerto Rico, just above New  Mexico's 43, and below Nebraska's 48. 
The Virgin Islands, Guam, American Samoa, and Northern Mariana Islands had six, five, four, and two cases respectively. Curiously, Washington state had only four cases.

It is hard to say why certain states have a higher rate than others, Barab said, given the relatively
small number of deaths relative to the state's population. This means there is a lot of volatility in the rate and a couple more or
fewer deaths can change the rate drastically. 

## Workers' Union Status

To scrape each case's union status, I used BeautifulSoup to extract the information.

Nearly 90% of workers who died were not unionzed. This is not surprising. [A report](https://illinoisepi.files.wordpress.com/2021/11/ilepi-pmcr-unions-and-construction-health-and-safety-final.pdf) published by the Illinois Economic Policy Institute in November 2021 — and [cited by OSHA](https://blog.dol.gov/2022/05/11/the-connection-between-unions-and-worker-safety) —
found that union worksites had 34% fewer violations per OSHA inspection 
than non-union ones. And while unions represented 14% of the construction industry workers, 
their employers made up only 5% of the industry’s OSHA violations. Unions help to negotiate
safety protocols, ensure their workers are not being put in risky situation, and help workers to
file and bring up grievances. 


![BVRD3-most-cases-involved-non-unionized-workers](https://user-images.githubusercontent.com/116761949/211128577-4399988a-8ae8-4d3b-8689-0c8c63139a72.png)
