# My OpenGL Game Engine

一款基于 OpenGL 开发的轻量级游戏引擎

## 项目简介

My OpenGL Game Engine 是一个正在开发中的游戏引擎项目，旨在学习现代游戏引擎架构和图形编程技术。该项目参考了 The Cherno 的游戏引擎开发教程，采用模块化设计，便于学习和扩展。

**项目状态：持续开发中**

## 核心特性

- **现代 C++17 架构**：使用最新 C++17 标准，采用面向对象设计
- **OpenGL 渲染**：基于 OpenGL 图形 API 的跨平台渲染系统
- **事件系统**：类型安全的事件分发机制，支持窗口、键盘、鼠标事件
- **模块化设计**：清晰的层次结构，便于理解和扩展
- **实时日志**：基于 spdlog 的彩色日志系统，支持多级别日志记录
- **ImGui 界面**：集成 Dear ImGui 提供交互式调试界面

## 技术栈

| 组件 | 技术 | 用途 |
|------|------|------|
| 开发语言 | C++17 | 引擎核心实现 |
| 图形 API | OpenGL | 跨平台图形渲染 |
| 窗口管理 | GLFW | 窗口创建与输入处理 |
| 日志系统 | spdlog | 高性能日志记录 |
| 界面系统 | ImGui | 交互式调试界面 |
| 构建系统 | Premake5 | 跨平台项目生成 |

## 项目结构

```
Hazel/
├── Hazel/             # 引擎核心库
│   ├── src/           # 源代码
│   │   ├── Hazel/     # 引擎模块
│   │   │   ├── Events/    # 事件系统
│   │   │   ├── ImGui/      # ImGui 集成
│   │   │   ├── Platform/OpenGL/  # 平台特定实现
│   │   │   ├── Application.h/cpp  # 应用基类
│   │   │   ├── Window.h         # 窗口接口
│   │   │   └── ...
│   └── vendor/        # 第三方依赖
│       ├── GLFW/      # 窗口库
│       ├── spdlog/    # 日志库
│       └── imgui/     # ImGui 库
├── Sandbox/          # 示例应用
│   └── src/          # 测试代码
├── premake5.lua      # 构建配置
└── README.md         # 项目文档
```

## 开发环境

- **操作系统**：Windows
- **编译器**：Visual Studio 2022
- **构建工具**：Premake5
- **图形库**：OpenGL

## 使用说明

### 构建项目

1. 确保已安装 Visual Studio 2022
2. 运行 `GenerateProjects.bat` 生成 Visual Studio 解决方案
3. 在 Visual Studio 中打开 `Hazel.sln`
4. 选择 Debug 或 Release 配置进行构建

### 运行示例

构建完成后，运行 Sandbox 项目即可启动示例应用。

## 学习参考

本项目基于以下教程开发：
- [The Cherno's Game Engine Series](https://www.youtube.com/playlist?list=PLlrATfBNZ98dC-V-N3m0Go4deliWHPFwT)

## 许可证

本项目仅供学习和教学目的使用。

## 致谢

特别感谢 The Cherno 提供的优质游戏引擎开发教程！
