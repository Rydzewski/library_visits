# library_visits
The data collected to create the three CSV dataset tables are reused data that comes from three visitor datasets on the California State Library: Public Library Statistics Portal (links to these datasets can be found in the "Metadata Schema" section under "references"). The data collected are from three visitor "Ready Reports," each report collects various library vising stats over a one-year timespan. Stats collected indlude hourly, weekly, annually, and per capita visits, vits per borrower, and which employees were visited. The data collected is intended for those who wish to see visiting trends in California's public libraries from July of 2016 to June of 2019. This information is open sourced data. 

This dataset was created for a University of Washington Winter 2021 Data Curation course (LIS 545). 

Note: Raw data was intentionally not added because only three spreadsheets were permitted for this project and there was no manipulation of data (other than separating the data within three tables and changing the variable names to align with a more standardized naming convention). All data can be found on the California Staate Libary: Public Library Statistics Portal (it is unknown if the data here is considered "raw" but for this project I am assuming that it is). 

# Table of Contents 

[Naming](#naming)

[Normalization](#normalization)

[Data Dictionary](#data-dictionary)

[Metadata Schema](#metadata-schema)

[License](#license)

[Contact](#contact)

# Naming

Naming the files for this repository should follow this format: 

```
average_visitordata
```

The "average" indicates the average number of a certain visitor satistics between all 186 California public libraries.

The "visitordata" indicates the specificed visitor data that is being collected between all 186 California public libraris. 

The file name should follow the camel case capitilzation type where the first letter in the first word is lowwercase and the first letter in all subsequent words are capitlaized. This follows the Project Open Data (DCAT-US Schema v1.1) guidelines which are being used for this repository's metadata schema. 

Example: *average_Visits_Per_Employee* 

This example notes that the data being collected is the average of all data collected for 186 California public libraries and the data collected is the visits per library employee.

The naming convention does not include the title of the California Public Libraries Portal because it is too long for a file name. Years are also not indicated in the file name because they are a variable that could be continually updated. If additional years or different types of visitor data are added, these additions should be noted in the metadata schema (where necessary) and additional variables need to be added to the Data Dictionary. 

# Normalization 

  The data being collected follows general normalization guidlines. 
  1. Formatting of all cell rows and columns are aligned. 
  2. All datasets have been cleaned so that there are no blank values, no dublicate variables, all numeric imputs have the same amount of digits as the other numberic imputs within a dataset, and that the value constraints within the Data Dictionary (below) are met in each dataset. 
  3. Data from the orginal souces (raw data) have been separated into three datasets so that varying data characteristics not collected in one dataset.
  4. The enrichment process was proformed by having a data dictionary and a metadata table included to improve the use of the data. 
  5. All datasets' variables use the camel case method which aligns with the fild naming convention listed in the above section (the POD v1.1 metadata schema used also follows this method for their feild names).  
  6. Editing and careful consideration was used to follow text normalization (spelling, vocabulary, puncutation, syntax) 

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
| describedBy | https://github.com/Rydzewski/library_visits.git|
| description | This dataset collections the average number of library visitors that go to California public libraries between 2016-2019. Specific yearly data collected inculdes the averages of the population of legal service area, library visits, vists per capital, vistis per borrower, visits per hours open, and visits per week. The datasets in this repository was created for a Univeristy of Washington Winter 2021 Data Curation course (LIS 545).|
| accessURL | https://github.com/Rydzewski/library_visits/blob/main/average_Population_Visits.csv |
| downloadURL| https://github.com/Rydzewski/library_visits.git |
| format | CSV |
| mediaType | CSV |
| identifier | https://github.com/Rydzewski/library_visits |
| issued | 20201-02-28 |
| keyword | "public library", "California", "visits", "borrower" |
| landingPage | https://github.com/Rydzewski/library_visits |
| language | en-us |
| license | none |
| modified | 2021-03-05 |
| publisher | Marissa Rydzewski |
| references | https://www.countingopinions.com/pireports/report.php?a7dca24c2a944fd8668331da6177a763&live, https://www.countingopinions.com/pireports/report.php?1f4ee471448420e9f39aa1584b57f1f0&live, https://www.countingopinions.com/pireports/report.php?0dc7d5b0b4ab96c42274f83c5ddf40f4&live, https://ca.countingopinions.com/index.php?page_id=3 |
| rights | This data is considered open source data and was collected from a state government library repository that is accessable to all. |
| temporal | 2016-07-01T00:00:00Z/2019-06-30T24:00:00Z|
| theme | public libraries, California, visits, borrower |
| title | California Public Library Visitors Stats (Average) |

# License
  There are no licensing restrictions to use this data.
# Contact
  Marissa Rydzewski rydzew@uw.edu

