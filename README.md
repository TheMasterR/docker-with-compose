# docker-with-compose
Docker with compose minimal image.

```docker pull themasterr/docker-with-compose:latest```

## Example usage

```
docker run --rm -it -v ~/:/root/ -v /var/run/docker.sock:/var/run/docker.sock  -p 80:80 -p 443:443 themasterr/docker-with-compose:latest ash
```
- Will drop you in the container, and mount your docker socket && your home directory to container home dir
- you can use --priviledged when running the container, for all cap's
