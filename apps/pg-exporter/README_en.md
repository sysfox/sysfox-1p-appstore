# PG Exporter

postgres_exporter is a PostgreSQL metrics exporter for Prometheus, maintained by the prometheus-community. It supports multiple PostgreSQL versions and provides comprehensive database observability.

## Features

### 📊 Comprehensive Metrics Coverage

- **PostgreSQL metrics** - Collects connections, query stats, replication status, table/index statistics, and more
- **Multi-version support** - Supports PostgreSQL 9.4 and above
- **Custom queries** - Supports custom SQL query metrics via YAML configuration

### ⚙️ Flexible Configuration

- **Connection string** - Supports standard PostgreSQL DSN format
- **TLS support** - Supports encrypted connections
- **Multiple databases** - Can monitor multiple database instances simultaneously

### 🔍 Easy Integration

- **Prometheus compatible** - Standard Prometheus metrics format
- **Standard port** - Listens on port 9187 by default
- **Docker friendly** - Official Docker image available

## Getting Started

After deployment, Prometheus can scrape metrics from:

```
http://your-server:9187/metrics
```

### Integration with Prometheus

Add the following to your Prometheus configuration:

```yaml
scrape_configs:
  - job_name: 'pg-exporter'
    static_configs:
      - targets: ['pg-exporter:9187']
```

### PostgreSQL Connection URL Format

```
postgresql://user:password@host:port/dbname?sslmode=disable
```

## Documentation

For more details, please visit the project page: https://github.com/prometheus-community/postgres_exporter

## Links

- GitHub: https://github.com/prometheus-community/postgres_exporter
- Docker Hub: https://hub.docker.com/r/prometheuscommunity/postgres-exporter
