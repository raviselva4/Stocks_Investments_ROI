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
    (takes 2-3 hours to download all 505 stocks with 20 years of data)

Okay, now you are ready to explore the stock trends and the prediction using our app, enjoy!!!


### Technical Artifacts Leveraged

1) Python Flask         - app.py
2) Powered RESTful API  - https://www.alphavantage.co/query?
3) HTML                 - index.html, prediction.html
3) CSS                  - style.css
4) JS                   - app.js, app2.js
5) Database             - Postgres
6) Webscraping          - https://en.wikipedia.org/wiki/List_of_S%26P_500_companies
7) D3.js                - app.js, app2.js
8) Plotly               - Timeseris, Bar (vertical/horizantal), Funnel graph
9) Apex Charts          - New JS open source library
10) Menus/dropdowns     - Fulfilled

### Data Volume

20 years of Stock daily data (2.25 million rows)

### Visualiztion used

1) Dynamic Funnel Chart, Candel stick View, ROI views
2) Apex chart with Sector Performance













