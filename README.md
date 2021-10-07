# Bookinfo Review Service

Review service has been developed on Java

## License

MIT License

## How to run with Docker

```bash
# Build Docker Image for review service
docker build -t reviews .

# Run review service on port 8082
docker run -d --name reviews -p 8082:8082 --link ratings:ratings -e ENABLE_RATINGS=true -e RATINGS_SERVICE=http://ratings:8080/ reviews
```

## How to run with Docker Compose

```bash
docker-compose up
```

## Website

[Opsta (Thailand) Co., Ltd.](https://www.opsta.co.th)
