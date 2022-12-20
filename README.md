# UnRAR

## Build
Via GitHub repository
```bash
$ docker build --tag alireaza/unrar:$(date -u +%Y%m%d) --tag alireaza/unrar:latest https://github.com/alireaza/unrar.git
```

## Run
```bash
$ docker run \
--interactive \
--tty \
--rm \
--env="TZ=$(cat /etc/timezone)" \
--mount="type=bind,source=$(pwd)/udocker,target=/home/udocker" \
--name="unrar" \
alireaza/unrar
```

