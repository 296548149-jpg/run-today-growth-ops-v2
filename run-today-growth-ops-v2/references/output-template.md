# Output Template

Use this template for a full 超脑俱乐部日报. Adapt wording to the day's facts, but keep the section order.

Do not include a standalone `信息充分性与去重说明`, `信息不足项`, `选题比例`, `核验`, `核验信息`, or `核验时间` section in the user-facing report. Keep verification, deduplication, and insufficiency details in internal notes or the final automation/Triage summary.

Do not include memory-card breakdowns or generate memory-card images for this workflow.

```text
【超脑俱乐部日报｜M月D日】

把信息变成判断，把判断变成表达。

今天的信息很多，您不用全部记住。
只需要从五件事里，带走几个能帮您判断世界、理解人性、稳定表达的记忆点。

一、今天五件值得理解的事

事件一：XXX

类别：全球形势 / 国内生活

发生了什么：
XXX

思考点：
XXX

矛盾点：
XXX

讨论点：
XXX

反常识看法：
XXX

经济学视角：
XXX

政治学视角：
XXX

历史学视角：
XXX

核心记忆点：
XXX

事件二：XXX

类别：全球形势 / 国内生活

发生了什么：
XXX

思考点：
XXX

矛盾点：
XXX

讨论点：
XXX

反常识看法：
XXX

经济学视角：
XXX

政治学视角：
XXX

历史学视角：
XXX

核心记忆点：
XXX

事件三：XXX

类别：全球形势 / 国内生活

发生了什么：
XXX

思考点：
XXX

矛盾点：
XXX

讨论点：
XXX

反常识看法：
XXX

经济学视角：
XXX

政治学视角：
XXX

历史学视角：
XXX

核心记忆点：
XXX

事件四：XXX

类别：全球形势 / 国内生活

发生了什么：
XXX

思考点：
XXX

矛盾点：
XXX

讨论点：
XXX

反常识看法：
XXX

经济学视角：
XXX

政治学视角：
XXX

历史学视角：
XXX

核心记忆点：
XXX

事件五：XXX

类别：全球形势 / 国内生活

发生了什么：
XXX

思考点：
XXX

矛盾点：
XXX

讨论点：
XXX

反常识看法：
XXX

经济学视角：
XXX

政治学视角：
XXX

历史学视角：
XXX

核心记忆点：
XXX

二、今日 GitHub 热门应用

推荐应用：XXX

仓库链接：直接跳转仓库的链接

应用场景：
XXX

解决的核心痛点：
XXX

没有它：
XXX

使用它：
XXX

适合谁：
XXX

不适合谁：
XXX

三、今日哲学观点

哲学观点：
XXX

搭配的经济学观点：
XXX

生活化故事：
XXX

今天可以带走的一句话：
XXX

四、每日口才训练

原文依据：
作品 / 作者 / 版本 / 版权状态说明

短摘录或主题：
XXX

朗读训练稿：
XXX

朗读提示：
停顿：XXX
重音：XXX
气息：XXX
节奏：XXX

五、每日深度哲思

来源：
作品 / 作者或思想传统 / 章节或出处说明

哲思主题：
XXX

历史上的这个想法：
XXX

为什么有趣：
XXX

留给今天的思考：
XXX

你可以问自己：
XXX

大鱼-超级策划合伙人

联系微信：renzhiribao666
```

Copyright handling for the speaking section:

- Prefer public-domain original texts and cite them.
- For copyrighted or uncertain texts, use only a short compliant excerpt and write an original practice passage inspired by the idea.
- Never fill the 300-character training block with a long verbatim passage from a copyrighted modern edition or translation.

Daily deep philosophy reflection requirements:

- Must share one interesting philosophical thought from history, such as Theseus' ship, Zhuangzi's butterfly dream, Plato's cave, Aristotle's friendship, the Stoic dichotomy of control, Augustine on time, Hume on self, Kant on autonomy, Nietzsche's eternal recurrence, or another verifiable classic idea.
- Internally verify thinker or tradition, work title, book/chapter/section when available, and whether the content is a paraphrase or a short compliant excerpt.
- Do not write this section as emotional encouragement, slogan, advice, or moral preaching.
- Explain the thought in clear Chinese, connect it to ordinary modern life, and end with 1-2 open questions that guide users to think actively.
- Verify the source before finalizing. If it cannot be verified, choose another source or record the limitation internally and in the automation/Triage summary only; do not show `待核验` in the user-facing report.

Final review requirements:

- Confirm the five events follow the required ratio internally: exactly 1 `全球形势` item and exactly 4 `国内生活` items.
- Do not display the topic ratio explanation in the user-facing report.
- Confirm each domestic item is close to ordinary users' life, choices, costs, work, family, learning, consumption, public services, or community discussion.
- Confirm every event includes a concrete `思考点`, a real `矛盾点`, and an open-ended `讨论点`.
- Confirm the local history deduplication index was read before topic selection. At minimum compare against prior daily reports under `reports/` and `outputs/` matching daily growth report names.
- Confirm today's news event subjects, GitHub repository, philosophy viewpoint, economics pairing, speaking-practice source theme, deep-philosophy theme, and core memory points do not repeat prior daily reports.
- If a candidate item repeats a prior report, replace it. If no verified new replacement is available, record the insufficiency internally and report it only in the automation/Triage summary; do not add a standalone `信息不足项` or `信息充分性与去重说明` section to the daily briefing.
- Recheck every factual claim, source link, date, GitHub metadata item, classic quote, source attribution, and copyright/public-domain note before finalizing.
- Check that event titles, summaries, analysis angles, memory points, GitHub scenarios, philosophy takeaway, speaking practice, and daily deep philosophy reflection do not repeat the same wording or conclusion.
- Rewrite duplicates before output. Template labels may repeat; substantive content may not. This applies both within today's report and against historical daily reports.
- Final Markdown and Word files must not display source webpage URLs, verification labels, verification status, verification time, GitHub metadata verification summaries, or `待核验` notes, except for the GitHub recommendation's direct repository link. Keep other webpages and verification details in internal notes only, unless the user explicitly asks to include them.
- Final Markdown and Word files must end with the exact attribution block: `大鱼-超级策划合伙人` and `联系微信：renzhiribao666`.
