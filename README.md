# library_visits
The data collected to create these datasets are reused data that comes from three datasets on the California State Library: Public Library Statistics Portal. The data collected are from three "Ready Reports" that were created over a three-year time span to collect library vising stats. The data collected is intended for those who wish to see visiting trends in California's public libraries from 2016-2019. This reository was created for a University of Washington Winter 2021 Data Curation course (LIS 545). 
# Table of Contents 
# Naming
# Data Dictionary

| Variable | Variable Name | Measurement Unit | Allowed Values | Definition | 
|-----------|--------------|------------------|----------------|------------| 
| year_1 | Year the Data was Collected (1) | Numerical | 2016-2017, 2017-2018, 2018-2019 | This is the year span that the data was collected for visitor statistics. The year starts in July of the first year indicated and ends in the following year in June (one year of data over two year time-span). This variable is in the first dataset of three, which is why the "1" is included at the end of the variable to distinguish from the other "year" variables. | 
| ave_Pop_Area | Average Population Size of the Legal Services Area | Numerical  | Any number | This is the total average population size between 186 California public libraries listed in the original "2016-2017 Visits" "2017-2018 Visits" and "2018-2019 Visits" datasets found on the California Public Library Statisitcs Portal. From the original dataset "Figure is based upon the California Dept. of Finance, Demographic Research Unit E-1 report issued each May 1st. Adjustments made if necessary by CSL staff to reflect the boundary of each library service area." | 
| ave_Visits_Year | Average Library Visits per Year  | Numerical  | Any number | This is the total average number of people entering public libraries whatever purpose during the year-span specified. A note from the orginal dataset "NOTE: If an actual count of visits is unavailable, determine an annual estimate by counting visits during a typical week in October and multiplying the count by 52. A “typical week” is a time that is neither unusually busy nor unusually slow. Avoid holiday times, vacation periods for key staff, or days when unusual events are taking place in the community or the library. Choose a week in which the library is open its regular hours. Include seven consecutive calendar days, from Sunday through Saturday (or whenever the library is usually open)." | 
| ave_Visits_Week | Average Weekly Visits | Numerical | Any number | This is the total average number of people entering public libraries on a weekly basis during the year-span specified. | 
| year_2 | Year the Data was Collected (2) | Numerical | 2016-2017, 2017-2018, 2018-2019 | This is the year span that the data was collected for visitor statistics. The year starts in July of the first year indicated and ends in the following year in June (one year of data over two year time-span). This variable is in the second dataset of three, which is why the "2" is included at the end of the variable to distinguish from the other "year" variables. | 
| visits_Per_Cap | Visits per Capita | Numerical | Any number |This is the total average of vistis per capita to each public library during the year-span specified. | 
| visits_Per_Borrower | Visits per Borrower | Numerical  | Any number | This is the total average number of registered borrowers who visited a public library during the year-span specified. "Borrowers" means that a library user checked-out a library item/material to take outside of the library and the item/material will be returned at a later date. "Registered" means that the library user has a active library account with the specified public library. | 
| visits_Per_Hour | Vists per Hour Open | Numerical  | Any number | This is the total average number of visitors per hour. This statistic is also depended on each library's individual operational hours scudleds thus the "Open" has been added to the variable name. | 
| year_3 | Year the Data was Collected (3) | Numerical  | 2016-2017, 2017-2018, 2018-2019 | This is the year span that the data was collected for visitor statistics. The year starts in July of the first year indicated and ends in the following year in June (one year of data over two year time-span). This variable is in the third dataset of three, which is why the "3" is included at the end of the variable to distinguish from the other "year" variables.|
| librarian_Visits| Visits per Libraian FTE | Numerical  | Any number| This is the total average number of library visitors per librarian, who is a full-time employee (FTE). | 
| librarian_MLS_Visits | Visits per MLS Librarian FTE | Numerical  | AAny number| This is the total average number of library visitors per Masters of Library Studies (MLS) librarian, who is a full-time employee (FTE). | 
| staff_Visits | Visits per Staff FTE | Numerical  | Any number| This is the total average number of library visitors per library staff member, who is a full-time employee (FTE).This staff member is not a librarian, but has another library-related job title.| 

# Metadata Schema
  Schema Used: Project Open Data (DCAT-US Schema v1.1)
  
| Attribute | Value |
|-----------|-------------| 
| accessLevel | public |
| accrualPeriodicity | R/P1Y |
| fn | Marissa Rydzewski |
| hasEmail | mailto:rydzew@uw.edu |
| describedBy | public |
| description | This dataset collections the average number of library visitors that go to California public libraries between 2016-2019. Specific yearly data collected inculdes the averages of the population of legal service area, library visits, vists per capital, vistis per borrower, visits per hours open, and visits per week. The datasets in this repository was created for a Univeristy of Washington Winter 2021 Data Curation course (LIS 545).|
| accessURL | public |
| downloadURL| public |
| format | CSV |
| mediaType | CSV |
| identifier | public |
| isPartOf | public |
| issued | 20201-02-28 |
| keyword | "public library", "California", "visits", "borrower" |
| landingPage | public |
| language | en-us |
| license | none |
| modified | 2021-03-05 |
| publisher | Marissa Rydzewski |
| references | public |
| rights | This data is considered open source data and was collected from a state government library repository that is accessable to all. |
| temporal | 2016-07-01T00:00:00Z/2019-06-30T24:00:00Z|
| theme | public libraries, California, visits, borrower |
| title | California Public Library Visitors (Average) |

# License
  There are no licensing restrictions to use this data.
# Contact
  Marissa Rydzewski rydzew@uw.edu

