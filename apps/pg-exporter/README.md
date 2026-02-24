# PG Exporter

postgres_exporter 是 Prometheus 的 PostgreSQL 指标导出器，由 prometheus-community 社区维护，支持多个 PostgreSQL 版本，提供全面的数据库可观测性。

## 功能特性

### 📊 全面的指标覆盖

- **PostgreSQL 指标** - 收集连接数、查询统计、复制状态、表/索引统计等核心指标
- **多版本支持** - 支持 PostgreSQL 9.4 及以上版本
- **自定义查询** - 通过 YAML 配置文件支持自定义 SQL 查询指标

### ⚙️ 灵活配置

- **连接字符串** - 支持标准 PostgreSQL DSN 格式
- **TLS 支持** - 支持加密连接
- **多数据库** - 可同时监控多个数据库实例

### 🔍 易于集成

- **Prometheus 兼容** - 标准 Prometheus metrics 格式
- **标准端口** - 默认监听 9187 端口
- **Docker 友好** - 官方提供 Docker 镜像

## 使用说明

部署后，Prometheus 可以抓取以下端点获取指标：

```
http://your-server:9187/metrics
```

### 与 Prometheus 集成

在 Prometheus 配置文件中添加：

```yaml
scrape_configs:
  - job_name: 'pg-exporter'
    static_configs:
      - targets: ['pg-exporter:9187']
```

### PostgreSQL 连接地址格式

```
postgresql://user:password@host:port/dbname?sslmode=disable
```

## 文档

更多详细信息，请访问项目主页：https://github.com/prometheus-community/postgres_exporter

## 项目地址

- GitHub: https://github.com/prometheus-community/postgres_exporter
- Docker Hub: https://hub.docker.com/r/prometheuscommunity/postgres-exporter
