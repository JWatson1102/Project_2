
![Project_2__ETL___Extract,_Transform,_Load_](https://user-images.githubusercontent.com/96347335/159197171-782fdd63-11ad-4e94-be0d-3957035a5731.png)


Many critical and valuable data are available these days, but it is often dispersed among multiple data sources and not well organized. **Extracting** the data from its sources, **transforming** it by cleaning or reformatting it, and **loading** or storing the resulting data into a well-designed database is critical for data-driven organizations. 


With over a million new releases each year, the book industry can seem daunting when looking for a good read. However, finding the bestsellers, ratings, and book size can help customers decide if they should start that lengthy novel over their short weekend. 


![books](https://user-images.githubusercontent.com/96347335/158924336-bb99a6a0-4e0e-4d35-801e-0eed9b82787c.jpeg)

# Data Cleaning: CSV File
The original csv file (book.csv)looked as follows: 

![alt txt](Resources/Excel_screenshot.png)

The isbn-13, which would later become our book id, was in scientific notation and had to be converted into standard notation before uploading it into our database. Once the csv file was loaded and read into our database it resulted in the following table:

![alt txt](Resources/original_book_screenshot.png)

 The uploaded and read table contained information relating to over 11,000 books. The information included title, authors, publisher, ratings, etc. There were several columns that had to be removed (bookID,language_code,Unnamed:12) because they were not pertinent to the project. Once those columns were dropped, we renamed and reordered the remaining columns for better readablity and importance. We then set our ISBN-13 column to our index (unique identifier), as it is a number that is unique to a specific book. The resulting table was as follows:

 ![alt txt](Resources/final_book_screenshot.png)

 The resulting table provided a cleaner and more readable information tool.





