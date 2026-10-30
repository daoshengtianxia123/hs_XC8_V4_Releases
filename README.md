# HS MCU Tools 安装包

这里公开发布 HS MCU Tools 的 VS Code 插件安装包。打开右侧 **Releases**，下载适合的 `.vsix` 文件，在 VS Code 中执行“扩展：从 VSIX 安装”。

## 安装包类型

- `ai-xc8-win64`：Windows x64 常规版，包含编译工具链和 AI 功能。
- `ai-lite`：跨平台精简版，AI 功能可用；编译器需要按本机平台配置。
- `ai-restricted-xc8-win64`：Windows x64 受限版，编译、下载及仿真操作不可执行。

## v0.2.97

修复 HS16F3211 等芯片导出 CCS 时的配置字顺序。第三个配置字现在保留频率加倍位，与 HSIDE v2.1.17 同工程生成的 CCS 一致。升级插件后须重新编译并重新打开新 CCS；旧 CCS 不会自动修改。
