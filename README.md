# DevOps Assignment 1 - AWS API Gateway
## Level 1 - Manual Setup via AWS Console
## Invoke URL

Base URL:
https://i0rxuq66m5.execute-api.ap-south-1.amazonaws.com/v1
## Route 1: /json/{todo}

Backend:
https://jsonplaceholder.typicode.com/{todo}

Example curl:

curl -k https://i0rxuq66m5.execute-api.ap-south-1.amazonaws.com/v1/json/todos/1
## Route 2: /weather

Backend:
https://api.open-meteo.com/v1/forecast

Required Query Parameters:
- latitude
- longitude
- hourly (optional)

Example curl:

curl -k "https://i0rxuq66m5.execute-api.ap-south-1.amazonaws.com/v1/weather?latitude=10&longitude=76&hourly=temperature_2m"
## Route 3: /countries/{name}

Backend:
https://restcountries.com/v3.1/name/{name}

Example curl:

curl -k https://i0rxuq66m5.execute-api.ap-south-1.amazonaws.com/v1/countries/india

## CORS

CORS is enabled for all routes and allows requests from all origins.

