# docker-compose-memcached
Memcached server with Docker and Docker Compose

## Usage (start server)

On folder that contains `docker-compose.yml` type one of this.

```
// non detach mode
docker-compose up
```
or
```
// detach mode
docker-compose up -d
```

It will spin the Memcached latest version and expose port to host at `11211`.

## Usage (stop server)

To shutdown server without remove the container.

```
docker-compose stop
```

To shutdown server and remove the container.
```
docker-compose down
```

## How to connect to Memcached

To test connection, just type this.

```
telnet localhost 11211
```

If connected than you can type sample command like below.

```
stats
```

To exit type `exit`.

You can connect to your local Memcached server with any programming platform you use.

Enjoy your local Memcached server for any purpose you want, for me this setup is fine for testing purpose.
