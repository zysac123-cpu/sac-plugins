# sac-plugins

Plugin market index (format 1) for the SAC DeepSeek Harness plugins.

## 索引地址

```
https://raw.githubusercontent.com/zysac123-cpu/sac-plugins/main/plugin-index.json
```

在 DeepSeek Harness 里：**设置 → 插件 → 发现 → 添加索引源**，粘贴上面的地址。

## 收录的插件

| 包 | 说明 |
|---|---|
| [`sac-skills-catalog`](https://www.npmjs.com/package/sac-skills-catalog) | 技能库：把当前会话的 skills 按功能域自动归类，可搜索、看说明、复制 `/命令` |
| [`sac-translate-selection`](https://www.npmjs.com/package/sac-translate-selection) | 划词翻译：聊天记录里选中文字，就近点「翻译」即出译文（需启用官方实验包「推理翻译」） |

## 维护

`plugin-index.json` 用官方 `@deepseek-ai/dsh-plugin-market-index` 的 `parseMarketIndex`（format 1）生成并校验；图标以内嵌 base64 data URI 提供，不依赖外部图片。

发新版本时：在 `plugins[].versions` 追加或替换版本条目，`publishTimestamp` 填该版本在 npm 上的发布时间（Unix 秒），重新校验后提交。
