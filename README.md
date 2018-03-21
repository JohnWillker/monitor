## Monitor

### Use:

```sh
    HOSTNAME=$(hostname) docker stack deploy -c docker-compose.yml prom
```

### Run ecs-exporter

```sh
    docker run -d -e AWS_ACCESS_KEY_ID=${AWS_ACCESS_KEY_ID} -e AWS_SECRET_ACCESS_KEY=${AWS_SECRET_ACCESS_KEY} -p 9222:9222 slok/ecs-exporter -aws.region="sa-east-1"
```

