# parking-lot-manager
Reposotory contains two Java projects, for loading (ingesting) and for reading the data.

First project has called 'loader', and it's a simple Java app which communicates with Elasticsearch. 
When the app has started, it loads the CSV file with the information about parking lots, and ingest them to the Elasticsearch. 
When process has completed, the app exits with code 0.

Second project has called 'api', and it's a simple Spring Boot app which communicates with Elasticsearch.
The app has 2 endpoints:

  1. Get the closest parking lot for provided cooridinates
  2. Get the number of parking lots for provided coordinates and radius 
    
