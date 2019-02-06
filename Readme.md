# Phoenix Build Image
Built from the official Elixir images, but with npm added for installing front
end dependencies.

## Features

Erlang is installed, Elixir is installed, NodeJS is installed.

## Usage
```
docker run -d parobus/phoenix:latest
```

## Updating

This image is based off the [official images](https://github.com/c0b/docker-elixir).

To upgrade copy the most recent `Dockerfile` to another, and then change the FROM
statement, or the NPM install statement.

1 - `docker build <target dir>`
2 - `docker tag <resulting image> parobus/phoenix:<target>`
3 - `docker tag <resulting image> parobus/phoenix:latest`
4 - `docker push parobus/phoenix:<target>`
5 - `docker push parobus/phoenix:latest`

Note you will need to be logged in as some with DockerHub priviledges.
