# Unity_socket_Repo
# Unity Socket通信框架

这是一个基于Unity实现的Socket通信框架，包含服务端(SocketServer)和客户端(SocketClient)两部分，通过TCP协议进行网络通信。

## 功能特点

- 完整的连接管理
- 数据封装与解析
- 心跳包检测机制
- 断线重连功能
- 服务端多客户端连接支持
- 自动心跳超时检测

## 项目结构

- SocketServer：服务端实现
- SocketClient：客户端实现
- 共享组件：
  - DataBuffer.cs：数据缓冲区管理
  - SocketDataPack.cs：数据包封装和解析
  - SocketEvent.cs：通信协议事件定义

## 运行说明

1. **创建Unity项目**：
   - 创建两个新的Unity项目，分别命名为SocketClient和SocketServer
   - 推荐使用Unity 2021.3或更新版本

2. **导入代码**：
   - SocketClient项目：复制`SocketClient/Assets/Scripts`下的所有文件到新项目的Assets/Scripts目录
   - SocketServer项目：复制`SocketServer/Assets/Scripts`下的所有文件到新项目的Assets/Scripts目录

3. **场景设置**：
   - 在每个项目中创建新场景
   - 创建空物体并添加Main.cs脚本作为组件

4. **运行测试**：
   - 首先运行SocketServer项目
   - 然后运行SocketClient项目
   - 两个项目都需要在Unity编辑器中运行

## 注意事项

- 确保两个项目使用相同的Unity版本
- 默认使用本地连接（127.0.0.1:6854）
- 需要在Unity编辑器中运行以便查看调试信息
