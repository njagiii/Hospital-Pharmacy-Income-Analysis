# Hospital-Pharmacy-Income-Analysis - A power BI based analysis of the hospital pharmacy income.
All columns were formatted correctly using power query i.e all names and IDs were formatted to text. \
In order to create a data model, dimension tables were derived from the three provided tables. The following dimension tables were created:-\
DimDate derived from the Visits Table containing Date details such as month, quarter and year. \
DimVisits derived from Visits Table containing visit_ID, diagnosis and department\
DimDrugs derived from Pharmacy_Transactions table containing Drug_ID, drug name and drug category\
DimPatients derived from Patients Table containing patient_ID, patient_name, gender, age\

Two Fact Tables were created, a FactsVisits table and a FactTransactions table. Both “visits” and “transactions” are business processes.\
A star schema was developed where all the dimensions tables were connected to the “FactVisits” table except the “DimDrugs” table which was connected to the “FactTransactions” table. Finally the FactTransactions table was connected to the FactVisits table. \
All the relationships were verified before visualization began.

# Key Insights
- Kiambu had the highest number of total diseases diagnosed thus more investment is required in Kiambu county for management of the diagnosed diseases.\
- Flu was the most prevalent disease with a total of 56 cases across all counties, followed by typhoid and diabetes respectively. Efforts need to be directed to the management and containment of flu, investment on medications such as flu vaccines for children and other medications needed for the management of flu need to be made the following year.\
- Kiambu recorded the highest total number of diabetes and typhoid cases while Kisumu recorded highest hypertension cases. In Uasin Gishu, the most prevalent disease was flu. County specific efforts are needed to manage the respective diseases especially for the lifestyle diseases such as diabetes and hypertension.\
- The inpatient department generated the highest revenue at Ksh94,759, followed closely by the emergency department thus increasing inpatient capacity would be necessary as well as equipping the emergency department to be able to handle more cases. \
- The age group between 60 to 90 years consume more medications (total of 43-44 medications) compared to the other groups. Patients aged 41 to 50 consume least number of medications (total of 25 medications).\
- Some diagnoses such as flu and hypertension have higher total number of hospital stay days compared to the pharmacy revenue they generate. Malaria has the least number of hospital stay days with a total of 41 days.\
- More effort is required to manage flu and avoid its spread, especially in Uasin Gishu to reduce its prevalence.\
- Early and homemade remedies and management should be encouraged since hospitalization due to flu generates little capital and reduces the hospital’s capacity to admit more patients with diseases that generate more income.\
- Malaria treatments generated the highest revenue for the pharmacy that year. This means that stocking more malaria meds is necessary.\
- August which generated the highest pharmacy revenue and patient visits recorded the highest income came from hypertension medicines. 



