# Setup Redis in Docker

The following command is used to create and run conatiner for local Redis instance:

```Bash
docker run -d -p 6379:6379 -v <data-dir>:/data --name redis dockerFile/redis
```
