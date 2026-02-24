# PG Exporter

PG Exporter is an advanced PostgreSQL & pgBouncer metrics exporter for Prometheus, providing 600+ metrics covering everything you need for PostgreSQL observability.

## Features

### 📊 Comprehensive Metrics Coverage

- **600+ metrics** - ~3K time series per instance
- **Full coverage** - Monitor PostgreSQL (10-18+) and pgBouncer (1.8-1.25+) in a single exporter
- **Self-monitoring** - Rich metrics about the exporter itself for complete observability

### ⚙️ Highly Customizable

- **Declarative config** - Define almost all metrics through YAML configs
- **Dynamic planning** - Define multiple query branches based on different conditions
- **Fine-grained control** - Configure timeout, caching, skip conditions per collector

### 🔍 Smart Discovery

- **Auto-discovery** - Automatically discover and monitor multiple databases within an instance
- **Version compatibility** - Supports PostgreSQL 10-18+ (9.x via legacy config bundle)
- **Extension support** - timescaledb, citus, pg_stat_statements, and more

### 🏥 Health Check APIs

- **HTTP health endpoints** - Comprehensive endpoints for service health and traffic routing
- **Role-aware** - Distinguishes primary and replica health status
- **Hot reload** - Reload configs without process restart

## Getting Started

After deployment, Prometheus can scrape metrics from:

```
http://your-server:9630/metrics
```

### Integration with Prometheus

Add the following to your Prometheus configuration:

```yaml
scrape_configs:
  - job_name: 'pg-exporter'
    static_configs:
      - targets: ['pg-exporter:9630']
```

### PostgreSQL Connection URL Format

```
postgres://user:password@host:port/dbname?sslmode=disable
```

## Documentation

For more details, please visit the official documentation: https://pigsty.io/docs/pg_exporter

## Links

- GitHub: https://github.com/pgsty/pg_exporter
- Official Documentation: https://pigsty.io/docs/pg_exporter
- Docker Hub: https://hub.docker.com/r/pgsty/pg_exporter
