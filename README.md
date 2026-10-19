# @sfmc-bds/module-monitor

> 此模块已弃用，其能力已收编至 SFMC 平台 SDK 宿主。更新平台并重建、部署行为包后，无需安装或启用 monitor。
> 平台保留 `/c:status`、`tps.current`、`tps.status` 和 `monitor.metrics` 兼容入口，提供 TPS、在线人数、维度实体数、视距区块估算以及指标历史。
> 旧 `monitor.json` 和 `sfmc_monitor_*` 表不删除。新历史写入独立的 `runtime-metrics.sqlite`，避免参与业务模块事务。

Wave A official SFMC module: **monitor** (运行时监控).

## Develop

```bash
pnpm install
pnpm run typecheck
pnpm run test
```

Install into platform:

```bash
sfmc mod install monitor --from dir:. --link
```
