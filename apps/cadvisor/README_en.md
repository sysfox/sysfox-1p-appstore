# cAdvisor

cAdvisor (Container Advisor) is an open-source tool by Google that provides resource usage and performance monitoring for running containers.

## Features

### 📊 Real-time Monitoring

- **Resource usage** - Real-time monitoring of CPU, memory, filesystem, and network usage
- **Performance metrics** - Collects performance data and statistics for containers
- **Historical data** - Retains historical usage data for trend analysis

### 🔍 Container Discovery

- **Auto-discovery** - Automatically discovers all running containers on the host
- **Hierarchical view** - Provides visualization of container hierarchy
- **Real-time updates** - Dynamically tracks container start and stop events

### 📈 Data Export

- **Prometheus integration** - Native support for Prometheus format metrics export
- **Multiple storage backends** - Supports exporting data to InfluxDB, Elasticsearch, and more
- **REST API** - Provides RESTful API for data querying and integration

### 🖥️ Web Interface

- **Real-time dashboard** - Intuitive web UI displaying resource usage
- **Container details** - View detailed metrics and information for each container
- **Easy to use** - View monitoring data without additional configuration

## Getting Started

After deployment, access the configured port to view cAdvisor's web interface.

cAdvisor automatically monitors all running containers on the host without additional configuration. By default, monitoring data is retained for 2 minutes of history.

### Integration with Prometheus

cAdvisor provides a `/metrics` endpoint for Prometheus to scrape. Add the following to your Prometheus configuration:

```yaml
scrape_configs:
  - job_name: 'cadvisor'
    static_configs:
      - targets: ['cadvisor:8080']
```

## Documentation

For more details, please visit the official documentation: https://github.com/google/cadvisor/blob/master/docs/storage/README.md

## Links

- GitHub: https://github.com/google/cadvisor
- Official Documentation: https://github.com/google/cadvisor/tree/master/docs
