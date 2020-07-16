# STA9760 Project 2 Part 2---Insert Data into ElasticSearch

Start:

docker-compose up -d


This will start ElasticSearch and Kibana.

ElasticSearch: http://localhost:9200 Kibana: http://localhost:5601


Running python:

export APP_KEY={MY_TOKEN}

docker-compose run pyth python parking.py --page_size=1000 --num_pages=4


export curl output:

curl -X GET {localhost:9200/parking-violation-index} > output.txt


Shutting off:

docker-compose down
