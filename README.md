# grafana + prometheus

> Project to launch the Observability option to any Go api, that implements the [Go-Libs](https://github.com/zuluapp/go-libs).

## Steps

### Create and launch the docker container

```cmd
your-grafana-project-path > docker compose up -d
```

### Review the target status in Prometheus URL

- Open [`http://localhost:9090/targets`](http://localhost:9090/targets)
- Check that the host _`http://localhost:9090/metrics`_ has the state <img align="center" width="35" alt="image" src="https://user-images.githubusercontent.com/113373447/192590706-2ec095c0-1efd-4139-9b14-594551637ddf.png">
