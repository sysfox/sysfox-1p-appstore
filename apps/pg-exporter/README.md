# PG Exporter

PG Exporter 是 Prometheus 的高级 PostgreSQL & pgBouncer 指标导出器，提供 600+ 个指标，覆盖 PostgreSQL 可观测性所需的一切。

## 功能特性

### 📊 全面的指标覆盖

- **600+ 指标** - 每个实例约 3000 个时间序列
- **完整覆盖** - 单个导出器同时监控 PostgreSQL（10-18+）和 pgBouncer（1.8-1.25+）
- **自监控** - 丰富的导出器自身指标，实现完整可观测性

### ⚙️ 高度可定制

- **声明式配置** - 通过 YAML 配置定义所有指标
- **动态规划** - 基于不同条件定义多个查询分支
- **细粒度控制** - 按收集器配置超时、缓存、跳过条件等

### 🔍 智能发现

- **自动发现** - 自动发现并监控实例内的多个数据库
- **版本兼容** - 支持 PostgreSQL 10-18+（通过旧版配置包支持 9.x）
- **扩展支持** - timescaledb、citus、pg_stat_statements 等

### 🏥 健康检查

- **HTTP 健康端点** - 用于服务健康和流量路由的全面接口
- **角色感知** - 区分主库和从库的健康状态
- **热重载** - 无需重启即可重新加载配置

## 使用说明

部署后，Prometheus 可以抓取以下端点获取指标：

```
http://your-server:9630/metrics
```

### 与 Prometheus 集成

在 Prometheus 配置文件中添加：

```yaml
scrape_configs:
  - job_name: 'pg-exporter'
    static_configs:
      - targets: ['pg-exporter:9630']
```

### PostgreSQL 连接地址格式

```
postgres://user:password@host:port/dbname?sslmode=disable
```

## 文档

更多详细信息，请访问官方文档：https://pigsty.io/docs/pg_exporter

## 项目地址

- GitHub: https://github.com/pgsty/pg_exporter
- 官方文档: https://pigsty.io/docs/pg_exporter
- Docker Hub: https://hub.docker.com/r/pgsty/pg_exporter
