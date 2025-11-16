# cAdvisor

cAdvisor（Container Advisor）是 Google 开源的容器资源监控和性能分析工具，为运行中的容器提供资源使用情况和性能特征的洞察。

## 功能特性

### 📊 实时监控

- **资源使用情况** - 实时监控 CPU、内存、文件系统和网络使用情况
- **性能指标** - 收集容器的性能数据和统计信息
- **历史数据** - 保留历史使用数据用于趋势分析

### 🔍 容器发现

- **自动发现** - 自动发现主机上所有运行的容器
- **层级视图** - 提供容器层级结构的可视化展示
- **实时更新** - 动态跟踪容器的启动和停止

### 📈 数据导出

- **Prometheus 集成** - 原生支持 Prometheus 格式的指标导出
- **多种存储后端** - 支持导出数据到 InfluxDB、Elasticsearch 等
- **REST API** - 提供 RESTful API 用于数据查询和集成

### 🖥️ Web 界面

- **实时仪表盘** - 直观的 Web UI 展示资源使用情况
- **容器详情** - 查看每个容器的详细指标和信息
- **易于使用** - 无需额外配置即可查看监控数据

## 使用说明

部署后，访问配置的端口即可查看 cAdvisor 的 Web 界面。

cAdvisor 会自动监控主机上所有运行的容器，无需额外配置。默认情况下，监控数据会保留 2 分钟的历史记录。

### 与 Prometheus 集成

cAdvisor 提供 `/metrics` 端点供 Prometheus 抓取。在 Prometheus 配置文件中添加：

```yaml
scrape_configs:
  - job_name: 'cadvisor'
    static_configs:
      - targets: ['cadvisor:8080']
```

## 文档

更多详细信息，请访问官方文档：https://github.com/google/cadvisor/blob/master/docs/storage/README.md

## 项目地址

- GitHub: https://github.com/google/cadvisor
- 官方文档: https://github.com/google/cadvisor/tree/master/docs
