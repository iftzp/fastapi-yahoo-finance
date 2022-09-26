# FastAPI Yahoo Finance

This repo contains the code used to create a web API using FastAPI which returns data scraped from Yahoo Finance.

Make sure you have FastAPI and uvicorn[standard] installed (an ASGI server)
To run the code:
```
uvicorn main:app --reload
```

Then, you can query the current information regarding any stock symbol listed on Yahoo Finance:
For example, Apple:

http://127.0.0.1:8000/v1/AAPL/summary/

or Amazon:

http://127.0.0.1:8000/v1/AMZN/summary/

The API uses BeautifulSoup to scrape data from the webpage associated with the symbol on Yahoo Finance.
Endpoints can be adjusted in scrape.json.
