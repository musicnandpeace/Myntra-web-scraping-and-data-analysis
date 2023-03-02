# Myntra-web-scraping-and-data-analysis
This project aims at collecting and analysing the material composition of the most popular clothing items on India’s largest online fashion store, Myntra.



## Motivation:
![Newspaper Clip](https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/images/Screenshot%202023-03-02%20at%2010.28.19%20PM.png)

Did you know as much as 35% of all microplastics in the marine environment are fibres from synthetic clothing, largely a result of fast fashion. These fabrics are durable, cheap and easily available, but many of them are made through wasteful, chemically-intensive or ethically harmful processes.
Additionally, the fashion industry is responsible for 20% of global wastewater, while also releasing 50 billion plastic bottles’ worth of microplastics into the environment each year. So on our part we can be more mindful of our purchasing behavior based on the material fibre composition of the clothing items.

As an initiative, this projects attempts at reflecting the most popular trends or shift in material composition from natural to artificial or synthetic. 


![Production energy by fibres](https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/images/Screenshot%202023-03-02%20at%2010.31.26%20PM.png)

---
## Objective: 

To analyze the material composition of the most popular clothing items on India’s largest online fashion store, Myntra.

## Data requirement:

To maintain the uniformity of data, clothing items need to be collected across both genders. Features including: clothing category, brand, price, rating, rating counts, material info, wear type and product description will help us in understanding the consumer behavior better in relation to the clothing material.

## Data collection:

A web scraper https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/scrapper/Web_driver_myntra_clothings.ipynb created using selenium has been used to scrape the above information (features) of top 1000 most popular clothing items in the below categories:

1. women_kurta_kurti_suits,
2. women_shorts_skirts, 
3. women_dresses, 
4. women_ethnic_tops, 
5. women_western_trousers, 
6. women_sarees, 
7. women_western_tops, 
8. women_western_tshirts, 
9. women_sweaters_sweatshirts, 

10. men_trackpants
11. men_kurta_sets, 
12. men_tshirts,
13. men_casual_trousers, 
14. men_kurta_kurtasets, 
15. men_sweatshirt_jackets, 
16. men_sherwani_jackets_dhotis, 
17. men_formal_shirts, 
18. men_casual_shirts, 

## Date of collection: 

The 18000 records fetched are dated from 27th January 2023 to 30th January 2023. It is like a snapshot of the popular clothing items in the above listed categories between these dates.

## Data pre processing:

Compile raw data: https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/raw_data/step%201%20compile%20raw%20data.ipynb

Data Cleaning: https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/raw_data/Step%202%20Data%20Preparation.ipynb

-Encoding categorical columns 

-Handling missing values – Missing values in the columns rating and rating_count filled using KNN imputer.

-Data manipulation - Creation of new columns based on existing columns like material columns namely (cotton, polyester, viscose etc) using material info scrapped into material_info column.

https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/Data%20Preprocessing.ipynb

## Data Analysis and Visualization:
Find the jupyter notebook here: https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/blob/main/Exploratory%20Data%20Analysis.ipynb
(Plotly graphs may not get rendered in github environment, so check out the inference image analysis here https://github.com/musicnandpeace/Myntra-web-scraping-and-data-analysis/tree/main/inference%20images-analysis)

## Reference 
Check out link to understand categorisation of fibres into natural, artificial and synthetic :
https://www.swicofil.com/commerce/products
