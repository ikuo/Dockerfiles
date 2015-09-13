[MySQL](https://github.com/docker-library/docs/tree/master/mysql) 5.6 with charset fix.

cf. https://github.com/docker-library/mysql/pull/14#issuecomment-119345645

## Quick Run

```
$ docker run -it --rm --name mysql -e MYSQL_ROOT_PASSWORD= -e MYSQL_ALLOW_EMPTY_PASSWORD=yes -p 3306:3306 ikuo/mysql:5.6
$ mysql -uroot -h$(docker-machine ip default)
```

## Building

```
docker build -t $(whoami)/mysql:5.6 .
```
