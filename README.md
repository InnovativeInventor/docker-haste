## Docker-hastebin
This is a simple way to run [haste-server](https://github.com/seejohnrun/haste-server) using Docker. By default, CORS is enabled. To disable CORS, use the Docker and Compose files within the folder `no-cors`.

## To run this using Compose (recommended):
Clone this repository, then type in:
`docker-compose up`

## Running using Docker
To build this using Docker, clone this repository, then type in:
```
git clone
docker build -t haste-server .
docker run haste-server
```

or, you can use the prebuilt images on Docker Hub:

```
docker pull innovativeinventor/docker-haste
docker run innovativeinventor/docker-haste
```

## Extra notes
To completely rebuild via compose right before deployment, type in:
`docker-compose build --no-cache && docker-compose up -d`

## Credits & Contributions
[seejohnrun/haste-server](https://github.com/seejohnrun/haste-server)

Contributions are always welcome – and appreciated! Just submit a pull request, and I'll review it.
