# orange-field

Fieldsbrew 的 **bottle 优先** 核心 tap（`orangereds` 自建）。

- 定位：formula 同时提供 `[source]` 与 `[bottle]`；安装时优先用预编译 bottle，失败自动回退源码构建。
- 来源：由 `fb convert` 从 Homebrew `homebrew-core` 转换生成。
- 适用：Fieldsbrew（`fb`）——面向 Intel Mac 的包管理器，默认前缀 `/opt/fieldsbrew`。

## 用法

```sh
fb tap orangereds/orange-field
fb search <name>
fb install <name>
```

## 状态

仓库当前为骨架：`Formula/` 目录待生成。

## 与 seeds 系 tap 的关系

- `orange-field`（本仓库）：bottle 优先，能省编译时间。
- `orange-seed`：纯源码，所有配方只有 `[source]`，没有 `[bottle]`。
