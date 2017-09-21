# NOS lite: Docker setup

Clone het project met submodules

```sh
git clone --recursive git@github.com:noslite/docker.git noslite-docker
cd noslite-docker
```

Installeer de dependencies

```sh
docker-compose run composer install
```

Start de service & server

```sh
docker-compose up
```

Ga naar [http://localhost:1234](http://localhost:1234).