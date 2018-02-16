# Elixir Dockerfile

1. First, build this image
```
cd elixir-dockerfile
docker build .
```

2. And then, list all the built images
```
docker images
```

3. Get the ID of the image you just built and tag it with a tag name (in this example, using `latest`). Note: `latest` is the default tag used by a Dockerfile to pull content, so it's better to not change it.
```
docker tag 67de4c9459bc dsignr/elixir-docker:latest
```

4. Now, login into Docker HUB.
```
docker login
```

5. Push it!
```
docker push dsignr/elixir-docker
```

## Legacy documentation:

This Dockerfile enables you to create your own [Elixir](http://www.elixir-lang.org) and [Erlang OTP](http://www.erlang.org/) docker image using the latest version of both.

This Dockerfile is based on the [phusion/baseimage](https://registry.hub.docker.com/u/phusion/baseimage/) docker image which is designed to overcome some issues using base Ubuntu in a Docker container.
