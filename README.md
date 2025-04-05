# docker-files
Ready made docker files

## Prometheus

`docker run -p 9090:9090 -v $(pwd)/prometheus.yml:/etc/prometheus/prometheus.yml prom/prometheus`

## Grafana

`docker run -d -p 3000:3000 grafana/grafana`

Add Prometheus as a data source:

    URL for docker: http://host.docker.internal:9090 
    URL fro direct installaion (http://localhost:9090)