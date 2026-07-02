---
name: run-today-growth-ops-v2
description: Generate a Chinese daily briefing named 超脑俱乐部日报 for users with cognitive anxiety or growth anxiety. Use when Codex needs to search current news, select exactly five verifiable events with one global-situation item and four domestic China items close to users' daily life, analyze each event with thinking points, tension points, discussion points, and multi-disciplinary lenses, recommend one trending GitHub application with a direct repository link, explain one philosophy viewpoint plus one economics idea through a life-like story, create around 300 Chinese characters of speaking practice from public-domain classics or short compliant excerpts, and end with a daily deep philosophy reflection that shares an interesting historical philosophical thought and guides users to think actively.
---

# Run Today Growth Ops V2

## Overview

Produce a calm daily briefing named `超脑俱乐部日报` for users who feel overloaded by news, knowledge, and self-improvement pressure. The goal is not to make users feel behind; the goal is to help them build judgment, memory, expression, and a little steadiness.

Use a service tone: concrete, warm, low-pressure, intellectually sharp, and easy to read on mobile. Avoid slogans, anxiety marketing, exaggerated certainty, and "must learn today" pressure.

When drafting a full daily briefing, read `references/output-template.md` before writing so the structure stays consistent. Do not generate memory-card breakdowns or memory-card images for this workflow.

## Required Inputs

Use the user's date and timezone when available. If not provided, use the current local date and state it.

If current news or GitHub popularity is required, use live search when available. Do not rely on memory for "latest", "today", "hot", star counts, recent updates, or current events.

If search is unavailable, ask for source materials, choose another verifiable item, or record the insufficiency internally for the automation/Triage summary; do not invent news, repository names, star counts, licenses, or source links.

Important output boundary: verification details are internal. Do not print source webpages, source URLs, verification labels, verification status, verification time, or "待核验" notes in the final user-facing Markdown or Word files unless the user explicitly asks for them. The GitHub recommendation is the exception only for the direct repository link so users can jump to the project.

## Daily Uniqueness Requirement

Every run must produce a daily briefing whose substantive news and content are new relative to prior daily reports in this project.

Before selecting topics, build a local deduplication index from existing files matching:

- `reports/daily-growth-report-*.md`
- `reports/brain-club-daily-*.md`
- `reports/superbrain-club-daily-*.md`
- `outputs/wechat-daily-growth-report-*.md`

Use the full available history when it is quick to read; otherwise read at least the most recent 30 daily reports. Compare against prior event titles, event summaries, core memory points, GitHub recommendations, philosophy viewpoints, economics concepts, speaking-practice source themes, and daily deep philosophy themes.

Hard rule: do not repeat the same news event, GitHub repository, philosophy viewpoint, economics pairing, speaking-practice source theme, daily deep philosophy theme, or core memory point from a prior daily report. If a major ongoing story must be covered, only use a genuinely new development with a new title, new factual basis, new analysis angle, and new core memory point; otherwise choose a different event.

If the available source material is too thin to satisfy both factual verification and non-repetition, do not recycle old content or fabricate facts. Keep the insufficiency reason in internal notes and final automation summary, not as a standalone section in the user-facing daily briefing.

## Workflow

1. Gather current material.
   - First read the local deduplication index described in `Daily Uniqueness Requirement`; keep a short internal list of disallowed prior topics, repositories, philosophy themes, speaking-practice themes, and deep-reflection themes.
   - Search current news from credible sources and choose exactly five events from the last 24 to 48 hours when possible.
   - Use a fixed topic ratio: exactly one event should be related to `全球形势`, such as geopolitics, global economy, international technology governance, global climate/systemic risk, or major cross-border coordination.
   - The other four events must be domestic China news that ordinary users can connect to daily life, such as work and employment, consumption and prices, education, housing, healthcare, transport, public services, local governance, technology products, culture, lifestyle, family decisions, or community life.
   - Reject candidate events that substantially duplicate previous daily reports, even if the source is newly republished or the wording is different.
   - Do not let international affairs dominate the five events. If a domestic event has a global background, foreground how it affects Chinese users' life, choices, costs, opportunities, or public discussion.
   - Use at least one source link per event. Cross-check high-risk or highly consequential claims with a second source.
   - Search GitHub Trending, GitHub search, releases, or another verifiable GitHub source for one popular application-level repository.
   - Reject any GitHub repository that has already appeared in a prior daily report; choose a different application-level repository or record the insufficiency internally if no verifiable new candidate is available.
   - Gather source material for the philosophy, speaking practice, and daily deep philosophy reflection sections. Any direct quote, classic reference, book/chapter/section claim, author attribution, translation status, or copyright/public-domain status must be checked against a credible source. If it cannot be verified, choose another source or record the insufficiency internally; do not show "待核验" in the user-facing report.
   - Reject philosophy, economics, speaking-practice, and deep-reflection themes that repeat prior reports; adjacent authors are acceptable only when the viewpoint, source passage, story, and takeaway are clearly different.

2. Filter for the target audience.
   - Choose events that help users understand how the world works and how daily life is being shaped, not events that only create fear.
   - For domestic news, prioritize items close to users' practical concerns: earning money, spending money, raising children, learning, working, commuting, healthcare, housing, local services, digital tools, family decisions, and community conversations.
   - Avoid graphic disasters, celebrity conflict, unverified scandals, medical claims, investment promises, minors' privacy, and high-conflict political agitation.
   - Political science analysis should explain institutions, incentives, coalitions, legitimacy, rules, and governance capacity. Do not write partisan persuasion or mobilization.
   - Economics analysis should explain incentives, costs, externalities, trade-offs, scarcity, information asymmetry, coordination, or opportunity cost. Do not provide investment advice.

3. Analyze each of the five events.
   - `类别`: mark whether the item is `全球形势` or `国内生活`.
   - `发生了什么`: one clear factual summary.
   - `思考点`: the question or judgment this event should trigger for ordinary readers.
   - `矛盾点`: the real tension between different goals, groups, costs, rules, or expectations. Avoid inventing conflict where none exists.
   - `讨论点`: one open-ended question suitable for community discussion. Do not write a forced conclusion or a yes/no slogan.
   - `反常识看法`: the hidden reversal or non-obvious lesson; avoid cheap contrarianism.
   - `经济学视角`: one real incentive or trade-off.
   - `政治学视角`: one institutional or governance mechanism.
   - `历史学视角`: one historical echo, pattern, or caution. Do not claim history repeats mechanically.
   - `核心记忆点`: one short sentence users can remember and retell.

4. Recommend one GitHub application.
   - Pick a real, useful, currently verifiable repository that solves one specific pain point for ordinary users, creators, operators, students, or small teams.
   - Internally verify the repository URL, star count, license, latest update/release status, and verification time when available. If a metadata field cannot be verified, keep that limitation in internal notes and the automation/Triage summary only.
   - In the final user-facing output, show only the repository name/owner and a direct clickable repository link. Do not show verification summary, stars, license, latest update/release, verification status, or verification time unless explicitly requested.
   - Explain `应用场景`, `核心痛点`, `没有它会怎样`, `用了它会怎样`, `适合谁`, and `不适合谁`.
   - Keep it practical. Do not turn the section into a long tutorial.

5. Explain one philosophy viewpoint with one economics idea.
   - Choose one recognizable philosophy viewpoint from Chinese or global philosophy.
   - Pair it with one economics idea that naturally relates to the viewpoint.
   - Convert both into a life-like story with ordinary scenes such as work, family, saving money, learning, choosing a project, or speaking in public.
   - End with a clear takeaway, not a lecture.

6. Write the speaking practice section.
   - Produce around 300 Chinese characters for oral practice.
   - Prefer public-domain classics, original Chinese classics, or public-domain translations.
   - If using a copyrighted or uncertain-copyright source, including many modern editions or translations, include only a short compliant excerpt and write an original practice passage inspired by the idea.
   - Cite the work and author/source. Do not provide long verbatim copyrighted passages.
   - Make the passage positive, philosophical, and suitable for reading aloud. Add brief delivery cues: pause, emphasis, breath, and rhythm.

7. End with `每日深度哲思`.
   - Choose one interesting philosophical thought from history, such as Theseus' ship, Zhuangzi's butterfly dream, Plato's cave, Aristotle's friendship, the Stoic dichotomy of control, Augustine on time, Hume on self, Kant on autonomy, Nietzsche's eternal recurrence, or another verifiable classic idea.
   - Internally verify the source: thinker or tradition, work title, book/chapter/section when available, and whether the reference is a paraphrase or a short compliant excerpt.
   - Do not include webpage URLs in the final user-facing output unless requested.
   - The final section should share the historical thought in clear Chinese, explain why it is interesting today, and end with 1-2 open questions that guide users to think actively.
   - Do not write it as emotional encouragement, slogan, advice, or moral preaching.
   - Keep it intellectually curious, concrete, and readable on mobile.

8. Run the final verification, duplication, and artifact pass.
   - Re-check every factual or source-based item: news claims, source links, dates, GitHub metadata, philosophy attribution, speaking-practice source, and daily deep philosophy reflection source.
   - Any item that cannot be verified must not be presented as confirmed. Prefer replacing it with a verifiable item. If replacement material is insufficient, keep the insufficiency in internal notes and the automation/Triage summary only; do not display "待核验" in the user-facing report.
   - Re-run the local history deduplication check against prior reports before finalizing. Treat semantic repeats as duplicates, not only exact string matches.
   - Verify that none of today's five event titles, event subjects, GitHub repository, philosophy viewpoint, economics concept pairing, speaking-practice source theme, daily deep philosophy theme, or core memory point repeats a previous daily report.
   - Check for duplicate content across all sections: event titles, event summaries, analysis angles, core memory points, GitHub pain/scenario wording, philosophy takeaway, speaking practice, and daily deep philosophy reflection.
   - Remove or rewrite repeated wording, repeated conclusions, and repeated examples unless the repetition is a necessary label in the template.
   - Do not finalize while unresolved duplicates remain, including duplicates against previous daily reports.

## Output Rules

- Write in Chinese unless the user asks otherwise.
- The daily briefing name must be `超脑俱乐部日报`; use the title format `【超脑俱乐部日报｜M月D日】`.
- Add this one-sentence slogan directly under the title: `把信息变成判断，把判断变成表达。`
- Final output must include only the normal daily briefing document. Do not include a memory-card breakdown or generate memory-card images.
- End every user-facing daily briefing with this exact attribution block:
  `大鱼-超级策划合伙人`
  `联系微信：renzhiribao666`
- Use short paragraphs and clear section headings.
- Keep source webpage links and all verification details out of the final Markdown and Word files. Source links, verification status, verification time, GitHub metadata checks, and insufficiency notes may be kept in internal notes or scripts, but the user-facing output should not display them except for the direct GitHub repository link.
- Do not include `核验`, `核验信息`, `核验时间`, `已复核`, `待核验`, stars/license/update verification metadata, or similar verification labels in the user-facing daily briefing unless the user explicitly asks for them.
- Do not include a standalone `信息充分性与去重说明`, `信息不足项`, or similar insufficiency note in the user-facing daily briefing. Keep those details in internal notes or the final automation/Triage summary.
- Do not display the topic ratio explanation in the user-facing daily briefing, even though the internal selection must still satisfy exactly one `全球形势` item and exactly four `国内生活` items.
- Include source and citation information for philosophy, speaking-practice excerpts, and the daily deep philosophy reflection. Do not expose source webpage URLs unless requested.
- Keep the analysis sharp but not academic. Translate concepts into everyday language.
- Avoid dense tables in user-facing copy.
- Do not label the user as sick or weak. Say "容易认知过载", "成长压力大", or "信息太多时".
- Do not pressure users to read every item, post content, join discussion, or prove growth.

## Quality Checks

Before finalizing, verify:

- Exactly five news events are included.
- Exactly one news event is marked `全球形势`.
- Exactly four news events are marked `国内生活`, and each is close to ordinary users' daily concerns.
- Today's five news events do not repeat prior daily-report event subjects or core memory points.
- Each event has been checked against a real source link internally and has a recent date, or the insufficiency has been recorded internally and in the automation/Triage summary only.
- Each event includes `思考点`, `矛盾点`, `讨论点`, and all five analysis lenses: counterintuitive, economics, political science, history, and core memory point.
- The GitHub recommendation is a real repository, has not appeared in prior daily reports, and does not fabricate stars, license, maintainer, or update status.
- The philosophy section includes both a philosophy viewpoint and an economics idea, neither repeats the same prior pairing, then turns them into one life-like story.
- The speaking practice is around 300 Chinese characters, avoids long copyrighted excerpts, and does not reuse the same prior source theme.
- The daily deep philosophy reflection is based on a verifiable historical philosophical thought, does not repeat a prior deep-reflection theme, and includes a source, an explanation, and 1-2 active thinking questions.
- Every factual claim, source attribution, quote, and metadata item has been rechecked internally. Unverified limitations are not displayed in the report; they are recorded internally and in the automation/Triage summary only.
- Final Markdown and Word outputs do not display source webpage URLs, except the direct GitHub repository link.
- Final Markdown and Word outputs do not display verification labels, verification status, verification time, GitHub metadata verification summaries, or `待核验` notes unless explicitly requested.
- Final Markdown and Word outputs end with the exact attribution block: `大鱼-超级策划合伙人` and `联系微信：renzhiribao666`.
- No duplicate content remains across titles, examples, analysis angles, memory points, tool scenarios, speaking-practice text, and daily deep philosophy reflection.
- No duplicate content remains against prior daily reports; if new material is insufficient, do not repeat an old item or fabricate facts. Track the insufficiency internally and mention it only in the final automation/Triage summary, not as a standalone daily-report section.
- The final section invites reflection without forcing a conclusion or promising emotional relief.
