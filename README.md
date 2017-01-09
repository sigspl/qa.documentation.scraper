# Use Docker to run this service


First, need to build the base image (subfolder) with Scrapy; then run build.sh to build image and run container.
Currently, Catalogue scraping is scheduled for once in a week Saturday morning.

To start scraping manually, run:

```docker exec qa.documentation.scraper /app/fiware/run.sh.```

System saves data to /app/fiware/items.json.

Manual export of the results file: 

```docker cp qa.documentation.scraper:/app/fiware/items.json .```


