# firebase for OpenAgent

Manage Firebase through the official Firebase MCP server.

Install the release archive through OpenAgent Integrations → Plugins. This is an independent adaptation.

## Setup

- Node.js/npm and a Firebase account; firebase-tools 15.33.0 uses the active workspace.

Run /firebase:setup. Package state and credentials belong in the active OpenAgent home at plugin-data/firebase/. Never place secrets in plugin.json or commit them. Refresh the plugin after changing credentials.

## Verification

bun test tests

Bundled tests cover immutable artifacts, config conversion and service configuration and missing prerequisites. Runtime acceptance also verifies a real staged installation, slash-command catalog and integration_status. External account authentication, real provider operations and macOS permissions require the prerequisites above; package tests do not claim those credentials are available.

## 中文

通过官方 MCP 服务管理 Firebase。 安装发布包后运行 /firebase:setup 查看配置要求。凭据和状态保存在当前 OpenAgent 数据目录的 plugin-data/firebase/ 下，修改后刷新插件。

Upstream source and exact revision are recorded in provenance.json. Bundled source remains available for inspection.
