# Harness Textbook

把交付写成可追溯、可验证、可回退的过程。执行 Unix 哲学：一文一责，事实一处。

## 快速开始

- 入口：[00.index.md](00.index.md)
- 学习序：`00` `01` `10` `11` `12` `13`，然后 `20`–`23`、`30`–`33`、`40`–`44`
- 执行序：`12` → `40`–`44`；需要对质退出码或 Hook 时再打开 `22`、`23`

## 文件清单

| 区间 | 组 | 职责 |
|------|----|------|
| 00–09 | meta | 入口与公约 |
| 10–19 | idea | 思想的唯一定义 |
| 20–29 | layer | 四层防线的操作面 |
| 30–39 | artifact | Specs、模板、知识图谱 |
| 40–49 | role | 五角色契约卡 |

逐篇一句话见 [00.index.md §1](00.index.md)，命名、元信息与引用句法见 [01.convention.md](01.convention.md)。

## 使用约定

- 学习只读本套；运行时读 `.harness/` 与 `.agents/`，不得反向引用本目录。
- 事实只在其 `defines` 归属文件定义一次，别处一律用 `[id]`、`[id §n]` 引用。
- 执行角色只有 `dispatcher`、`planner`、`plan-reviewer`、`developer`、`verifier`。
- 本套不含某一 Web 框架或浏览器驱动的操作手册，也不含运行时实现与示例业务代码。

## 仓库

```bash
git remote add origin https://github.com/whosneo/harness_textbook.git
```
