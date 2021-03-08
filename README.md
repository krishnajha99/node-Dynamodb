---
Skill Share API
---
http://localhost:3000/
http://localhost:3000/healthz
http://localhost:3000/api/articles

To build this sample locally, you can either build using Docker, or using NPM.

- Install [Docker](https://www.docker.com/get-started)
- Install [NodeJS](https://nodejs.org/en/download/)

## Setup

- To build using Docker, in the project folder, run `docker build -t skillshare-api .`
- To build using NPM, in the project folder, run `npm install`

## Running the api

- To run using Docker, run `docker run -it -p 3000:3000 skillshare-api`
- To run using NPM, run `npm start`

## Database setup

docker pull amazon/dynamodb-local

docker run -p 8000:8000 amazon/dynamodb-local

docker pull instructure/dynamo-local-admin

docker run -p 8000:8000 -it --rm instructure/dynamo-local-admin

docker run -d -p 127.0.0.1:8000:8000 amazon/dynamodb-local 

Dynamo DB Config:- <br />
aws dynamodb create-table --cli-input-json file:///Users/krjha/Documents/repo/mesj/cmpe282/config/tables/article.json --endpoint-url http://localhost:8000

docker run -d -p 127.0.0.1:8000:8000 instructure/dynamo-local-admin
