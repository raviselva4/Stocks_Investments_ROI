# Stock_Investments_ROI

### Setup

1) Create a postgres database using pgAdmin4

2) Create an account with https://www.alphavantage.co/ and get an free API key for stock data download 
    (or) 
   You may also use backup dump file (data/stock_database_fullbackup.sql) from the data folder and restore the database to your local using pgAdmin tool. 
   (Data as of 07/09/2020)
    
3) Git clone the repository to your local

4) Create a "config.py" file and input the following:

    stock_api_key = "yourkey"
    db_host = "localhost"
    db_port = "5432"
    db_pass = "yourpassword"
    db_name = "stock"

5) Run Python Flask http://127.0.0.1:5000/sp500 to download latest S&P 500 stocks

6) Run Python Flask http://127.0.0.1:5000/sp500 to download latest stock data from alphavantage website
    (takes a day to download all 505 stocks with 20 years of data)

Okay, now you are ready to explore the stock trends and the prediction using our app, enjoy!!!



