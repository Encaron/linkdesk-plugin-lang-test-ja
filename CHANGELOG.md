# 更新日志

## v1.0.4（2026-09-15）

- 新增市场身份图 `resources/icon.svg`（Type-2 彩色身份图，E6#68a）——此前 `plugin.json` 没有 `icon` 字段，市场里显的是**统一默认彩块**
- 意象：两枚对开语言卡（与 lang-defaults 同族同构）+ 前卡一枚日之丸；刻意不写「あ」，SVG 里排文字会绑字体
- 形态照 [06-图标.md](https://github.com/Encaron/linkdesk/blob/electron/docs/02-Electron%E6%9E%B6%E6%9E%84/E6_%E6%8F%92%E4%BB%B6%E7%94%9F%E6%80%81%E4%B8%8E%E5%8F%91%E5%B8%83/03-%E6%8F%92%E4%BB%B6%E5%B8%82%E5%9C%BA/06-%E5%9B%BE%E6%A0%87.md)：SVG / 透明底 / 48×48 正方形 viewBox / 零 `<text>`（不绑字体）
- `@linkdesk/plugin-sdk` 升到 0.1.19（^0.1.14 → ^0.1.19）——SDK 0.1.16 之前的 `publish` 没有 E6#106 的身份图 URL 化：包内相对路径写进目录条目后，**未装用户看到的图标恒 404**

## v1.0.3（2026-09-14）

- 源码迁入独立仓（E6#99，L7 第 7.2 轮）——从壳仓 `Encaron/linkdesk` 抽出本插件子树，历史全保（hash 变）
- 随包 `plugin.json` 显式声明 `pluginId`（E6#98g）：插件身份不再靠目录名兜底，独立仓构建出的包名与身份稳定
- `$schema` 改指本仓 `node_modules/@linkdesk/plugin-sdk`（脱离壳仓后原相对路径指到仓外，编辑器补全/校验会失效）


## v1.0.2（2026-09-11）

- 补充 README 与更新记录：详情页「详情」页签显示说明，「更改日志」页签不再是空

## v1.0.1（初始版本）

- 日语测试语言包（E3c #42 单语言插件验证）——创建时版本号即 1.0.1，此前无更新记录
