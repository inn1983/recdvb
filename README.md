# recdvb - DVB Signal Recorder

`recdvb` 是一个用于录制数字电视广播（DVB）信号的工具。它支持从 DVB 设备接收信号，并将其录制为文件。该项目包含多个 C 语言源文件和头文件，用于处理信号接收、解码和录制。

## 功能

- 接收 DVB 信号
- 解码 DVB 信号
- 录制信号为文件
- 支持频道切换
- 检查信号强度和质量

## 构建步骤

1. 确保已安装必要的依赖项（如 `autoconf`, `make`, `gcc` 等）。
2. 运行以下命令以生成配置脚本并构建项目：

   ```bash
   ./autogen.sh
   ./configure
   make
   ```

3. 构建完成后，可执行文件将生成在项目目录中。

## 使用方法

1. 运行 `recpt1` 命令以开始录制信号。例如：

   ```bash
   ./recpt1 [频道号] [录制时长] [输出文件]
   ```

   示例：

   ```bash
   ./recpt1 23 60 output.ts
   ```

   这将录制频道 23 的信号 60 秒，并保存为 `output.ts` 文件。

2. 使用 `recpt1ctl` 命令控制录制过程。

## 依赖项

- `autoconf`
- `make`
- `gcc`
- DVB 设备驱动

## 许可证

本项目遵循 [GNU General Public License](COPYING)。

## 贡献

欢迎提交问题和拉取请求以改进项目。

## 联系方式

如有问题，请联系项目维护者。