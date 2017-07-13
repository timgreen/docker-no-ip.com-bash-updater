A simple Docker container for running the
[mdmower/bash-no-ip-updater](https://github.com/mdmower/bash-no-ip-updater) to update
the ip of an account on no-ip.com.

# How to use

First, create `config` file in the config dir. Then run with one of following methods.

## Fire and forget

    docker run -it --rm -v $(pwd)/config/config:/bin/config noip-updater:latest

## Cron job

    docker run -it --rm -v $(pwd)/config/config:/bin/config noip-updater:latest cron

## Docker compose

    docker-compose up
