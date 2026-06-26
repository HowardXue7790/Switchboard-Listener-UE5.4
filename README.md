# UE 5.4 Switchboard 独立运行包

本仓库用于在脱离完整 Unreal Engine 安装的情况下，独立运行 UE 5.4 的 Switchboard 和 Switchboard Listener。

English version: [README.en.md](README.en.md)

## 包含内容

- `StartSwitchboard.bat`: 启动 Switchboard。
- `StartSwitchboardListener.bat`: 启动 Switchboard Listener。
- `Engine/`: Switchboard 运行所需的 UE 5.4 相关文件。

## 快速开始

1. 下载或克隆本仓库。
2. 双击运行 `StartSwitchboard.bat` 启动 Switchboard。
3. 双击运行 `StartSwitchboardListener.bat` 启动 Switchboard Listener。

## 首次启动说明

首次启动 Switchboard 时，程序会在以下目录创建 Python 虚拟环境：

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python
```

创建完成后，虚拟环境脚本中的以下文件会写入当前机器的绝对路径：

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python\Scripts\activate.bat
```

## 迁移到其他电脑

如果将本仓库拷贝到其他电脑使用，请先删除以下目录，再在新电脑上启动 Switchboard：

```text
.\Engine\Extras\ThirdPartyNotUE\SwitchboardThirdParty\Python
```

Switchboard 会在新电脑上重新创建 Python 虚拟环境，避免旧机器的绝对路径导致启动异常。

## 运行要求

- Windows
- UE 5.4 Switchboard 相关运行文件已包含在仓库中
