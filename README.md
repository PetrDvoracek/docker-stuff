# docker-stuff
Some notes about the Docker

## Docker-compose

Useful if you have several processes each one in different container. Docker-compose creates network for communication between them. Run with

```
sudo docker-compose up
```

in this example, two services starts on ports [5000, 5001], 5000 is a website which uses a REST API on 5001. The REST API is reachable from the container at http://product-service as seen in website/index.php, *product-service* is the name of the service in docker-compose.yml.
