

![Project_2__ETL___Extract,_Transform,_Load_ (3)](https://user-images.githubusercontent.com/96347335/159197388-4e665569-1810-4d18-a2af-f28355a1b851.png)

# ETL : Extract, Transform, Load:
__Extract:__ read the data, often from multiple sources/formats.

__Transform:__ clean and structure the data to suit business needs.

__Load:__ load the data into a database for storage that can be used for future analysis or business use.

##  Objective: 
##### We chose two data sources to analyze the bestselling books throughout several years for our project. 
__[Group Repo](https://github.com/JWatson1102/Project_2.git)__

### Members:

- Josh Watson
- Amy Castillon
- George Vallejo
- Mindy Garcia


With over a million new releases each year, the book industry can seem daunting when looking for a good read. However, finding the bestsellers, ratings, and book size can help customers decide if they should start that lengthy novel over their short weekend. 

***

## 1. Data sources:

> - __[New York Times API ](https://developer.nytimes.com/docs/books-product/1/routes/lists.json/get)__ 

> - __[Goodreads Books](https://www.kaggle.com/jealousleopard/goodreadsbooks?select=books.csv)__ 

> The two sources we extracted were in different formats. Goodreads data was extracted from Kaggle in CSV form. Our NYT data was extracted from an API in JSON format. Once we extracted the data from both sources, we then exported the data into CSV files. 


# Data Cleaning: CSV File
The original csv file (book.csv)looked as follows: 

![alt txt](Resources/Excel_screenshot.png)

The isbn-13, which would later become our book id, was in scientific notation and had to be converted into standard notation before uploading it into our database. Once the csv file was loaded and read into our database it resulted in the following table:

![alt txt](Resources/original_book_screenshot.png)

 The uploaded and read table contained information relating to over 11,000 books. The information included title, authors, publisher, ratings, etc. There were several columns that had to be removed (bookID,language_code,Unnamed:12) because they were not pertinent to the project. Once those columns were dropped, we renamed and reordered the remaining columns for better readablity and importance. We then set our ISBN-13 column to our index (unique identifier), as it is a number that is unique to a specific book. The resulting table was as follows:

 ![alt txt](Resources/final_book_screenshot.png)

 The resulting table provided a cleaner and more readable information tool.





