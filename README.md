# grafana + prometheus

> Project to launch the Observability option to any Go api, that implements the [Go-Libs](https://github.com/zuluapp/go-libs).

## Steps

### Create and launch the docker container

```cmd
your-grafana-project-path > docker compose up -d
```

### Review the target status in Prometheus URL

- Open [`http://localhost:9090/targets`](http://localhost:9090/targets)
- Check that the host _`http://localhost:9090/metrics`_ has the state <span style="color: white; background-color: #28a745; padding: 2px 5px; border-radius: 5px;">UP</span>
