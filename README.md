# ZCooler--an-Automatic-Intelligent-Air-Pressure-Laptop-Cooler
能够自动运行的智能笔记本风压式散热器，基于esp32设计，可通过蓝牙与电脑通信并进行自动开关和参数调节。

本开源为电脑程序、单片机程序部分

PCB设计请移步至嘉立创开源平台：https://oshwhub.com/tatzhao/bi-ji-ben-san-re-qi-2-0

机械建模设计请移步至Bamboo Lab：待更新

效果展示：https://www.bilibili.com/video/BV1M9aZz5Eke/


window程序：


功能特性

🔧 核心功能

实时硬件监控 - 监控CPU/GPU温度和功耗

智能风扇控制 - 支持自动、手动和自定义曲线控制

蓝牙连接 - 通过串口蓝牙与散热设备通信

RGB灯光控制 - 多种灯光模式和自定义颜色

自动连接机制 - 设备自动连接

🎛️ 控制模式

自动模式 - 根据温度自动调整风扇转速

手动模式 - 用户自定义固定转速

曲线模式 - 自定义温度-转速曲线

灯光模式 - 彩虹、单色、呼吸等多种效果

💾 系统集成

开机自启动选项

系统托盘最小化

内存优化管理

配置自动保存


系统要求

操作系统: Windows 10/11（目前仅在本人的笔记本上测试通过（WIN11）

.NET框架: .NET Framework 4.8

硬件: 支持蓝牙连接的智能散热设备

安装与使用
下载安装
从 Releases页面 下载最新版本

运行安装程序或解压便携版

启动ZCooler应用程序

首次使用
确保散热器设备已通电并处于可配对状态

进入电脑蓝牙界面配对设备

进入ZCooler程序

点击"刷新端口"按钮扫描可用蓝牙设备

选择正确的COM端口并点击"连接"

根据需要调整风扇和灯光设置

点击"保存"应用设置到设备

开发指南
项目结构
text
ZCooler/
├── Models/          # 数据模型
├── Services/        # 服务层（硬件监控、配置、蓝牙等）
├── Views/           # 用户界面
├── App.xaml         # 应用程序入口
└── MainWindow.xaml  # 主窗口

使用Visual Studio 2019或更高版本打开解决方案

还原NuGet包

构建并运行项目

依赖项
Hardcodet.Wpf.TaskbarNotification - 系统托盘支持

.NET Framework 4.8 - 运行时框架

配置说明
应用程序设置保存在 config.json 文件中，包含:

连接设置（端口、自动连接）

风扇曲线配置

灯光设置

应用程序偏好


许可证
本项目采用MIT许可证 - 详见 LICENSE 文件。

免责声明
本软件按"原样"提供，作者不对使用本软件造成的任何损害负责。使用前请确保了解散热设备的安全操作规范。
