## Data Documentation

### Cleaned Data Set 1

Data Set: merged_data

This data set spans from 2007 - 2021. It contains data from 6 different Colleges/Institutions in Washington State and includes columns of combined Statewide data. 


#### Source Links

1. https://data.wa.gov/education/PCHEES-Dashboard-Degrees-Awarded/krsk-s76t/data_preview

2. https://data.wa.gov/education/PCHEES-Dashboard-Degrees-by-Major/uc69-gudu/about_data

3. https://zircon.datausa.io/api/data?University=377564&measures=Graduation Rate,Number Of Finishers&drilldowns=Gender,IPEDS Race&Number Of Finishers>=5

4. https://zircon.datausa.io/api/data?University=377555&measures=Graduation Rate,Number Of Finishers&drilldowns=Gender&Number Of Finishers>=5&IPEDS Race=nonresident

5 . https://zircon.datausa.io/api/data?University=236948&measures=Graduation Rate,Number Of Finishers&drilldowns=Gender,IPEDS Race&Number Of Finishers>=5


#### Variables Explained

**Academic_Start_Year** - Academic Start Year refers to the year the school year this data set is referring to started. For example "2007" is referring to the 2007-08 school year. This column is integer value data. 

**Institution** - Institution refers to the Institution in Washington State that this data set is referring to. There is an addition value called "Statewide" in that column that refers to data for the entire state. Otherwise, the other Washington Institutions covered in this data set are: Central Washington University, Western Washington University, University of Washington, The Evergreen State College, Eastern Washington University, and Washington State University. This column is character value data.

**Degree_Type** - Degree Type refers to if this degree is a Graduate degree, an Undergraduate degree, a STEM degree or Not a STEM degree. These values are represented by four values: Graduate_STEM, Graduate_NonSTEM, Undergraduate_STEM, and Undergraduate_NonSTEM. This column is character data. 

**Number_of_Degrees** - Number of Degrees refers to how many degrees were granted for all the characteristics labeled in the row. This column is integer data. 

**Demographic** - Demographic refers to the Race/Ethnicity of the row. Unknown values were listed as "Unknown" in the original data set. This could refer to unreported data. The value "Total" refers to combined data for all the demographic values. The value "Other" is a placeholder we placed in the data for Race/Ethnicity categories with very little data. 


#### Rows and Columns

There are 2308 rows and 5 columns in this data set.  

There are 392 rows that report Demographics as "Unknown" from the original data set that are kept in this merged data set. There are 58 rows grouped under the "Other" category. Most of these values were attributed to the "Non-Resident Alien" demographic, but we decided to omit that because it wasn't comparable across all universities, and it was a status not a Race/Ethnicity. Otherwise, all the data is present in all the other rows. 


### Cleaned Data Set 2

Data set: UW_merged_data

This data spans from 2012 - 2021 for the University of Washington. We combined the number of degrees granted from all three campuses of the University of Washington to add a "Total_Degrees" Column that refers to the total number of degrees a demographic has received that year. This helped us calculate data to accurately represent what proportion of each Race/Ethnicity group gets a STEM/Non-STEM degree. There are 72 Total Degree values with NA data so we omitted them when we graphed them in order to prevent misrepresenting the trends. 