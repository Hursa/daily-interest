# daily-interest

HappyHabit「发现」页的内容仓库。生产方是每天一次的定时任务，消费方是 app。

**唯一的约定在 [`docs/contract.md`](docs/contract.md)。** 两边各自怎么实现都行，
但目录、文件名、字段、时序以那份为准，改它 = 改契约，两边要同时跟。

```
manifest.json        索引。app 每次先读它，而且只读它列出的东西
discover/*.json      一天一个文件
docs/contract.md     契约
```

> app 只信 `manifest.json`。没有列在 `days` 里的文件，就当它不存在——
> 所以未完成的草稿可以安全地留在 `discover/` 里。

## 当前状态

`discover/2026-08-05.json` 是第一期，**四条正文已完成并通过校验，但配图未解决，
因此尚未写入 `manifest.days`**。原因和解法见 `docs/contract.md` 末尾「未决:配图」。
