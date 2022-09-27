# grafana + prometheus

> Project to launch the Observability option to any Go api, that implements the [Go-Libs](https://github.com/zuluapp/go-libs).

## How can I launch this? 🤔

### Create and launch the docker container

```cmd
your-grafana-project-path > docker compose up -d
```

### Review the target status in Prometheus URL

- Open [`http://localhost:9090/targets`](http://localhost:9090/targets)
- Check that the host _`http://localhost:9090/metrics`_ has the state <img align="center" width="35" alt="image" src="https://user-images.githubusercontent.com/113373447/192590706-2ec095c0-1efd-4139-9b14-594551637ddf.png">

### Configure Prometheus in Grafana

- Open [`http://localhost:3000/datasources`](http://localhost:3000/datasources)
- Click on <img align="center" width="143" alt="image" src="https://user-images.githubusercontent.com/113373447/192591398-0254b810-556c-4e98-b978-efba2f56ed1e.png">
- Click on _Prometheus_
<img width="335" alt="image" src="https://user-images.githubusercontent.com/113373447/192591637-4d93a569-da96-415d-bead-76486390ad9b.png">
- Write `http://host.docker.internal:9090` in the URL configuration section
<img width="542" alt="image" src="https://user-images.githubusercontent.com/113373447/192591748-9e815c40-658d-4370-b74f-7433ef6baf8d.png">
- Click on _Save & Test_ <img align="center" width="109" alt="image" src="https://user-images.githubusercontent.com/113373447/192591903-a4f61979-eef9-480e-8665-c89216587137.png">
- This confirmation should have been shown
<img width="246" alt="image" src="https://user-images.githubusercontent.com/113373447/192592149-088eaf8b-73aa-4647-afd8-41c78d961930.png">

## How to use it? 🤓

> To learn more about it, you can go to the [Grafana official website](https://grafana.com/docs/grafana/latest/getting-started/build-first-dashboard/).

## License

Copyright © 2022, [Zulu](https://www.zulu.io/).
