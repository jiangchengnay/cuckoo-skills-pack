# 全能技能包（cuckoo-skills-pack）

为 [Cuckoo Code](https://github.com/wangyongpeng90/cuckoo-code) 提供一组通用开发技能。

## 包含技能

| 技能 | 用途 |
|---|---|
| `code-review` | 代码审查：正确性、边界、安全、性能、可读性 |
| `commit-message` | 生成 Conventional Commits 规范的 Git 提交信息 |
| `explain-code` | 用清晰的中文解释代码逻辑 |
| `refactor` | 重构建议并安全实施 |
| `security-check` | 安全自查：注入、密钥泄露、路径穿越 |
| `write-tests` | 编写单元测试，优先覆盖失败路径 |
| `generate-docs` | 生成函数注释 / README / API 文档 |
| `debug-assist` | 系统化排查报错、定位根因 |

## 安装

**方式一（推荐）**：在 Cuckoo Code 的「插件」页搜索 `cuckoo-plugin`，找到本插件点击安装。

**方式二（手动）**：把本仓库克隆到 `~/.cuckoo/plugins/cuckoo-skills-pack`：

```bash
git clone https://github.com/jiangchengnay/cuckoo-skills-pack.git ~/.cuckoo/plugins/cuckoo-skills-pack
```

安装后在插件页**启用**即可。

## 特性

- **纯提示词，零执行**：不含任何可执行代码，启用时**不会**弹出"含可执行内容"的安全警告。
- **开箱即用**：装完即生效，无需配置。
- **无依赖**：不依赖任何外部服务。

## 许可

MIT
