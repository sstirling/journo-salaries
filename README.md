# Journalism Salaries Data

This repository will be an effort to clean and standardize the [Real Journalism Salaries](https://www.cjr.org/cjr_outbox/google-doc-journalism-media-pay.php) spreadsheet, created by [Sarah Kobos](https://twitter.com/skobos/status/1194322736685998081), that has been making its rounds.  

If you'd like to submit your anonymous salary data, you can do so here: [Submission Form](https://docs.google.com/forms/d/e/1FAIpQLScws3_GjSHH7LGPdm7r82u1Nj5apstZHD5fiMu6zL_UO9gqRw/viewform)

If you'd like to see the raw data as it comes in you can do so here: [Salary data](https://docs.google.com/forms/d/e/1FAIpQLScws3_GjSHH7LGPdm7r82u1Nj5apstZHD5fiMu6zL_UO9gqRw/viewform)

## Cleaning Process

*New data last appended: 8:30 a.m. Nov. 15, 2019* 

*N=1224*

New, standardized columns will always be added at the end of the data so new information can be appended to the bottom. A file of the original data will also be kept here. 

* Nov. 13: I have created a numerical salary column, a numerical experience column and roughly cleaned employer column. I'll build out a broader data dictionary as I go.  

* Nov. 15: Removed several troll entries, appended another 400 or so data slots. Further refined title_category column.  

If you have suggestions/criticisms, you can ping me at stephenstirling@gmail.com.  Totally open to outside contributions as well.     

## Data Dictionary 

I'll add to this as I do more work:

| id                | unique id                                                                                                                   |
|-------------------|-----------------------------------------------------------------------------------------------------------------------------|
| title             | original title column                                                                                                       |
| employer          | original employer column                                                                                                    |
| salary            | original salary column                                                                                                      |
| gender            | original gender column                                                                                                      |
| years_exp         | original years experience column                                                                                            |
| Location          | original location column                                                                                                    |
| duties            | original "job duties" column                                                                                                |
| comments          | original "prev salaries/titles/etc" column                                                                                  |
| employer_clean    | column standardizes publication names removing words like "the" and various minor permutations                              |
| base_salary_clean | Changes all salaries to numerical values, where possible. Only base salaries included. Bonuses, if specified, not included. |
| sal_flag          | rows where base salary calculation not available for various reasons (non-usd, hourly)                                      |
| years_exp_clean   | numerical version of years exp column                                                                                       |
| location_forgeo   | beginning of standardized location column that would be fit to geocode. Non-specific locations eliminated                   |
| title_category    | first pass at standardizing 'title' column. Grouped many positions, but needs more work.                                    |
