# Earnings Call Transcripts Extraction
Aws2.ipynb notebook is used to extract all the earnings call Transcripts.
The various steps performed in this notebook includes:
### 1)Extracting all the tickers
We make an API call to fetch the data of Sp500 from http://en.wikipedia.org/wiki/List_of_S%26P_500_companies
We parse and extract the data and dump it into a pickle file sp500tickers.pickle
We converted tickers into list data type. Converted this ticker list into data frame and then to a csv file.
### 2)Retrieving ids for all tickers
#### 2.1)Extracting ids
We make an API call to https://seeking-alpha.p.rapidapi.com/transcripts/v2/list and get the list of ids
#### 2.2)Extracting name of the transcript
We extract the name of the sp500
#### 2.3)Extracting transcripts from ids
We exttract transcripts from the ids
