# VS Code Profile (No Copilot)

基于 VS Code 官方 Profile 模板，移除了 GitHub Copilot 相关扩展的配置文件集合。

## 背景

VS Code 最新版本已内置 GitHub Copilot，导致官方模板中包含的 Copilot 扩展（如 `github.copilot`、`github.copilot-chat` 等）在导入时可能产生冲突，使 Profile 无法正常生效。

本仓库的 `.code-profile` 文件均来自 VS Code 官方模板，移除了部分扩展（见下方详情），其余配置保持不变。

## 包含的 Profile

| Profile | 说明 | 扩展数 | 移除的扩展 |
|---------|------|--------|-----------|
| [angular.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/angular.code-profile) | Angular 开发 | 14 | - |
| [data-science.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/data-science.code-profile) | 数据科学 / Jupyter | 18 → 17 | `github.copilot` |
| [doc-writer.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/doc-writer.code-profile) | 文档写作 / Markdown | 11 | - |
| [java-general.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/java-general.code-profile) | Java 通用开发 | 8 → 6 | `visualstudioexptteam.intellicode-api-usage-examples`、`visualstudioexptteam.vscodeintellicode` |
| [java-spring.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/java-spring.code-profile) | Java Spring Boot | 12 → 10 | `visualstudioexptteam.intellicode-api-usage-examples`、`visualstudioexptteam.vscodeintellicode` |
| [nodejs.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/nodejs.code-profile) | Node.js 开发 | 11 | - |
| [python.code-profile](https://raw.githubusercontent.com/Back-T0/code-profile/master/python.code-profile) | Python 开发 | 22 → 20 | `github.copilot`、`github.copilot-chat` |

## 使用方法

1. 下载需要的 `.code-profile` 文件
2. 打开 VS Code，进入 **File > Preferences > Profiles**（或使用命令面板搜索 `Profiles`）
3. 点击 **Import Profile...**，选择下载的文件
4. 导入后即可使用

## 官方模板来源

- VS Code 官方文档：[Profile Templates](https://code.visualstudio.com/docs/configure/profiles#_profile-templates)
- VS Code 官方模板列表（JSON）：https://main.vscode-cdn.net/core/profile-templates.json
