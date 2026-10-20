# 修改声明 / Modification Notice

本文件是 MiniCreation 就 Apache License 2.0 上游作品所作修改的显著声明，随每个
发行包提供；源代码交付时也应一并提供。

## 上游作品

| 项目 | 内容 |
| --- | --- |
| 上游名称 | DeepWrite |
| 上游仓库 | https://github.com/swjybky/deepwrite |
| 商用基线 | v1.6.4 |
| 基线提交 | `69858fb1ae60a1fcc84b71122f945b1c86949049` |
| 基线快照 | https://github.com/swjybky/deepwrite/commit/69858fb1ae60a1fcc84b71122f945b1c86949049 |
| 基线许可证 | https://github.com/swjybky/deepwrite/blob/69858fb1ae60a1fcc84b71122f945b1c86949049/LICENSE |
| 基线日期 | 2026-10-08 |
| 上游许可证 | Apache License 2.0 |
| 许可证全文 | `LICENSES/Apache-2.0.txt` |

该基线中的 `LICENSE` 为 Apache License 2.0 标准全文，SHA-256 为
`c71d239df91726fc519c6eb72d318ec65820627232b2f796219e87dcf35d0ab4`。
上游 v1.6.4 的仓库树中没有 `NOTICE` 文件；其 `package.json` 未声明 `author` 或
`license` 字段，源文件中也未见逐文件版权头。上游后续的许可证变更不影响本基线
已经授予的 Apache-2.0 权利；相关证据由 MiniCreation 留存。本发布仓库仅提供安装包
与更新清单，不包含源代码。

## 修改声明

MiniCreation 是以 DeepWrite v1.6.4 为基础修改形成的衍生作品，不是上游原样副本。

- 修改起始日期：2026-10-09
- 本文件更新日期：2026-10-20
- 截至 2026-10-18，相对于基线提交，共有 2,247 个文件发生变化：1,883 个修改、
  11 个重命名、339 个新增、14 个删除。统计命令为
  `git diff --name-status v1.6.4`。
- 修改性质包括：产品更名与品牌替换；桌面端进程边界和工程结构重构；渲染层界面
  与交互重写；智能体、工具、契约、本地存储和更新通道的增删改；文档、构建、
  打包和测试调整；依赖升级。

在 MiniCreation 的私有源码仓库中，所有在 v1.6.4 中已存在、且内容发生变化并仍
保留的文件，均为 Apache License 2.0 意义上的修改文件；新增文件不在此列。其修改
日期以该源码仓库对应提交日期为准。除本文件外，随包 `NOTICE` 也载明上游名称、
版本、提交和修改事实。

## 文件级修改声明

所有在 v1.6.4 中存在、内容发生变化并保留至今，且格式支持注释的文本文件，均已在
文件顶部加入以下显著声明：

```text
Modified by MiniCreation from DeepWrite v1.6.4 (Apache-2.0); see NOTICE and MODIFICATIONS.md.
```

声明使用目标文件的原生注释语法：TypeScript/JavaScript 使用 `//`，Vue/HTML/Markdown
使用 `<!-- -->`，CSS 使用 `/* */`，YAML/Shell/PowerShell 使用 `#`。对接近源码行数
门禁上限的大文件，声明以行内块注释置于首行，避免因增加一行而突破既有预算。当前
工作区共 1,876 个文本文件带有该声明。

以下 18 个修改文件因格式限制无法承载注释，故由本文件集中记录，并在 `NOTICE` 与
安装包中随附本文件：

- JSON（11）：`apps/desktop/package.json`、
  `apps/desktop/src/utilities/fixtures/device-sync-ledger.json`、
  `apps/desktop/src/utilities/fixtures/device-sync-mobile.json`、
  `apps/desktop/tsconfig.node.json`、`apps/desktop/tsconfig.web.json`、
  `package.json`、`packages/contracts/package.json`、
  `packages/pi-runtime-adapter/package.json`、
  `packages/pi-runtime-adapter/tsconfig.json`、
  `packages/shared/package.json`、`update.json`。
- 图片（5）：`apps/desktop/build/icon.ico`、`apps/desktop/build/icon.png`、
  `apps/desktop/src/renderer/public/app-icon.png`、
  `docs/images/agent-manuscript.png`、`docs/images/workspace-overview.png`。
- 标准许可证文本（1）：`LICENSE`。该文件本身即许可条款，添加声明会改变标准文本。
- 生成锁文件（1）：`pnpm-lock.yaml`。该文件由包管理器生成，任何手工声明都会被
  下次安装覆盖。

`pnpm lint:apache-notices` 会以 v1.6.4 基线提交为基准，检查所有修改/重命名文本文件
是否带有上述声明；缺失时失败。新增或修改基线文件后，可运行
`pnpm fix:apache-notices` 自动补齐。该检查在缺少基线提交的浅克隆中会明确跳过，不会
把“无法检查”误报为通过。

## 分发要求

当前对外分发的是二进制安装包，源代码仓库保持私有。本发布仓库只包含安装包、更新
清单与许可材料，不包含源代码。根据 Apache License 2.0 第 4 条，分发本作品时须
同时提供：

1. `LICENSES/Apache-2.0.txt`（许可证全文）；
2. `NOTICE`（上游署名与第三方许可证说明）；
3. 本文件（修改声明）。

由于文件级声明已经写入源码，未来以源代码形式对外分发时，无需再逐文件补写声明；
但仍须随源码提供上述三份文件，并保留各文件顶部的声明。不得删除文件头声明，也不得
仅依赖 Git 提交历史来满足第 4(b) 条。

本文件不改变 Apache License 2.0 的许可条件，也不对上游权利人施加额外限制。

## English Summary

MiniCreation is a modified work based on DeepWrite v1.6.4 (commit
`69858fb1ae60a1fcc84b71122f945b1c86949049`, dated 2026-10-08), licensed under
the Apache License 2.0. Modifications began on 2026-10-09. As of 2026-10-18,
2,247 files differ from the baseline (1,883 modified, 11 renamed, 339 added,
14 deleted).
The changes include rebranding, architecture and process-boundary refactoring,
UI and interaction rewrites, agent/tool/contract/storage/update changes,
documentation and build changes, and dependency upgrades.

Every file that existed in the baseline and still exists with different content
is a modified file for purposes of the Apache License 2.0; newly added files are
not. All 1,876 modified text files that can carry comments now start with a
prominent change notice in their native comment syntax. The 18 files whose
formats cannot carry comments (11 JSON files, 5 images, the standard `LICENSE`
text, and the generated `pnpm-lock.yaml`) are recorded centrally in this file.
`pnpm lint:apache-notices` verifies the file-level notices against the baseline
commit, and `pnpm fix:apache-notices` repairs missing ones.

When distributing the work, include `LICENSES/Apache-2.0.txt`, `NOTICE`, and this
file. If the source code is ever distributed, retain the file-level notices; do
not rely on Git history alone to satisfy Section 4(b).

This notice does not alter the terms of the Apache License 2.0.
