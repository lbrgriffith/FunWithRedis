# Setup Redis in Docker

##Offical Redis Docker Image

[Docker](https://hub.docker.com/_/redis)
```Bash
docker pull redis
```

The following command is used to create and run conatiner for local Redis instance:

```Bash
docker run -d -p 6379:6379 -v <data-dir>:/data --name redis dockerFile/redis
```
If you enable persistence, Redis will store data on the VOLUME /data, which can be used with `--volumes-from some-volume-container` or `-v /docker/host/dir:/data`.

# Using .NET with Redis
In order to access Redis from .NET, you will need a .NET Redis Client.
You can find  .NET Redis [clients](https://redis.io/clients#c-sharp) can be found in the C# section of the Redis Clients page.

Reference: [Redis with .NET](https://docs.redis.com/latest/rs/references/client_references/client_csharp/)
