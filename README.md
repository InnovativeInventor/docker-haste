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
The images on Docker Hub are only built when I push to this repo, so if you want the latest version of docker-haste, either build it yourself or tell me to trigger a build on Docker Hub(make an issue).

To completely rebuild via compose right before deployment, type in:
`docker-compose build --no-cache && docker-compose up -d`

To explore the files in your docker container, type in:
`sudo docker exec -it dockerhaste_hastebin_1 sh`

## Credits & Contributions
[seejohnrun/haste-server](https://github.com/seejohnrun/haste-server)

Contributions are always welcome – and appreciated! Just submit a pull request, and I'll review it.
