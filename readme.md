# NOS lite: Docker setup

## Clone het project met submodule

```sh
git clone --recursive ...
```

## Installeer de dependencies

```sh
docker-compose run composer install
```

## Start de service & server

```sh
docker-compose up
```

Ga naar [http://localhost:1234](http://localhost:1234).