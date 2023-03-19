# US Unemployment ETL
Here the objective was to collect unemployment data from the US and load it into an SQL database. So to accomplish this, I found a dataset from Kaggle that gave the unemployment demographic of the US from 2010 to 2020. Some examples are that it gave a percentage of those with diplomas, the race, and whether they are male or female depending on the date. The same Kaggle source also provided a separate dataset of the unemployment percentages of each state in the US from 2010-2020. Afterward, I then collected another dataset which I obtained from DataHub. This dataset went from 1940-2010 and provided the population employed, population unemployed, agricultural ratio, etc.       
When these were all collected I then created a notebook to begin the next step. First I made sure to establish a connection to the MySQL database. Once that was done I created the database unemployment_usa using MySQL.connector library.     
![image](https://user-images.githubusercontent.com/89541481/226152148-9473f5f1-6792-4d34-9336-7d8fa9eefdcd.png)    

Then with each dataset, I made any modifications needed to ensure they were ready to upload. The readied datasets would then be loaded into the database as separate tables.     
![image](https://user-images.githubusercontent.com/89541481/226152172-92d49f7d-1351-461e-b81e-83f886d8d11a.png)    

The final step I made was to merge the unemployment demographic dataset with the 1940-2010 dataset by the year. This gave me a dataset only in 2010 with information from both. This was then loaded into the MySQL database after it was cleaned. That led to the end of the objective as the ETL process was officially completed.    
![image](https://user-images.githubusercontent.com/89541481/226152102-d4890912-b776-452a-bd51-d180c20a8f06.png)    

Technologies and Tools
- Python
- MySQL
- Pandas
- MySQL Connector

## Source
[Kaggle](https://www.kaggle.com/datasets/aniruddhasshirahatti/us-unemployment-dataset-2010-2020?resource=download)    
[DataHub](https://datahub.io/core/employment-us#readme)
