# cassandra-prometheus
Official Cassandra image plus Prometheus JMX Exporter.  Inspiration came from https://github.com/oleg-glushak/cassandra-prometheus-jmx
and https://www.robustperception.io/monitoring-cassandra-with-prometheus.

## Usage
See Official cassandra image for usage.  https://hub.docker.com/_/cassandra

Beyond those directions, this image adds a prometheus metrics endpoint at http://localhost:7070/metrics.  

e.g.
```
docker run -p 7070:7070 --rm -it ryanwalls/cassandra-prometheus:0.3.11
```

Load metrics by navigating to http://localhost:7070/metrics.

