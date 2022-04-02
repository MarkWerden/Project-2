# Project 2: Dogecoin vs Bitcoin

![image](https://user-images.githubusercontent.com/95598645/161183803-f2d26a7c-4fb3-441c-9d5e-be6b8ef28edf.png)

### What is Dogecoin?
Dogecoin is a cryptocurrency created by software engineers Billy Markus and Jackson Palmer, who decided to create a payment system as a joke, making fun of the wild speculation in cryptocurrencies at the time. It was introduced on December 6, 2013, and quickly developed its own online community. Elon Musk frequently mentions or talks about Dogecoin on his Twitter account, boosting its popularity a significant amount in recent years. The dataset used provides the history of daily prices of Dogecoin. The data starts from 17-Sep-2014. All the column descriptions are provided. Currency is USD.

### What is Bitcoin?
Bitcoin is a digital currency created in January 2009. It follows the ideas set out in a whitepaper by the mysterious and pseudonymous Satoshi Nakamoto.1 The identity of the person or persons who created the technology is still a mystery. Bitcoin offers the promise of lower transaction fees than traditional online payment mechanisms and, unlike government-issued currencies, it is operated by a decentralized authority. The dataset used provides the history of daily prices of Bitcoin. Currency is USD

## Datasets Used:
- Bitcoin Dataset: https://www.investing.com/crypto/bitcoin/historical-data
- Dogecoin Dataset: https://www.kaggle.com/datasets/varpit94/dogecoin-data

# Cleaning steps:
1. Drop unnecessary columns
2. Drop unnecessary rows and focus on dates 03/26/2021 - 03/25/2022
3. Convert date column on the bitcoin dataset from string to datetime
4. Rename columns so they match between the two sets
5. Added a column for blockchain symbols
6. Merge datasets
7. Set date as index
8. Converted all string values to float values

# Findings
- The “Bitcoin Historical Data” data source includes 365 records with day-by-day information about bitcoin’s opening price, closing price, highest price, lowest price, volume, and change percent from March 26, 2021, to March 25, 2022.
- The “Dogecoin Data” data source includes 1,598 records with day-by-day information about dogecoin’s opening price, closing price, adjusted closing price, highest price, lowest price, and volume from November 9, 2017, to March 25, 2022.
- Conducted an analysis which determined that the Pearson's correlation between Bitcoin prices and Dogecoin prices was 0.13 for the year.
- ![image](https://user-images.githubusercontent.com/95598645/161396269-c99b575a-f439-4899-913c-7d77186bb30e.png)
- ![image](https://user-images.githubusercontent.com/95598645/161396277-fc20b552-c971-4df6-8cec-2d57cdde4ce3.png)
- ![image](https://user-images.githubusercontent.com/95598645/161396285-9ad3af60-88a1-4b88-8750-e35ffbe3721c.png)

## Loading
- We chose to load the data through a relational database (SQL) considering that the data we were working with was structured and static.

