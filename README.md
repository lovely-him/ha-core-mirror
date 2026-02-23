# ha-core-mirror

Mirror Home Assistant Core container images for Orange Pi 3B (orangepi3b).

## 原理

将 HA 官方 `ghcr.io/home-assistant/odroid-m1-homeassistant` 镜像通过 `skopeo copy` 复制到 `ghcr.io/lovely-him/orangepi3b-homeassistant`。同架构 Core 镜像功能完全相同，仅 label 不同。

## 使用方法

1. 打开 [Actions](../../actions) 页面
2. 选择 "Mirror HA Core Image"
3. 点击 "Run workflow"
4. 填写 `core_version`（如 `2026.2.3`），勾选 `mirror_landingpage`
5. 等待完成

## 镜像映射

| 源 | 目标 |
|----|------|
| `ghcr.io/home-assistant/odroid-m1-homeassistant:{version}` | `ghcr.io/lovely-him/orangepi3b-homeassistant:{version}` |
| `ghcr.io/home-assistant/odroid-m1-homeassistant:landingpage` | `ghcr.io/lovely-him/orangepi3b-homeassistant:landingpage` |
