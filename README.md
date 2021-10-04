# Reviews service

## How to run docker.
```bash
# Build Docker Image for reviews service
docker build -t reviews .

# Run reviews service on port 8082
docker run -d --name reviews -p 8082:9080 reviews
```
* Test with path `/reviews/1` and `/health`

## How to run with Docker Compose

```bash
# rm all ps
docker rm -f $(docker ps -aq)
# run
docker-compose up
# build
docker-compose up --build
```