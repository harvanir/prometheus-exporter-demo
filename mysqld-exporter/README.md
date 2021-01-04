# Prometheus MySQL Server Exporter

## Setup

### SQL (sql/script.sql)

- Modify the sql script according to your needs
- Run the sql script

### Run exporter

Execute command:

```shell
./run-mysqld-exporter
```

### Testing

Browse exporter web page: [metrics](http://localhost:9104/metrics)

### Add prometheus job scrape configs (prometheus/prometheus.yml)

Copy all yml key value to your prometheus.yml file, start from key <code>- job_name</code>

### Grafana integration

Add to your grafana dashboard by importing json: grafana/MySQL-xxx.json

### Stop exporter

Execute command:

```shell
./down-mysqld-exporter
```