# Daily Game News Reporting Guidelines

This document defines how the daily game news digest should be produced.

## Scope

Only include game-related news. Exclude general technology, politics, finance, entertainment, or social news unless the story has a direct and meaningful game-industry connection.

Covered areas:

- Console, PC, mobile, and indie games
- Game updates, releases, delays, reviews, demos, patches, DLC, and expansions
- Platform news from PlayStation, Xbox, Nintendo, Steam, Epic, Apple, Google, etc.
- Game studios, publishers, acquisitions, layoffs, earnings, regulation, and licensing
- China game approvals, publishing, operations, and local market changes
- Esports tournaments, clubs, rosters, and major competitive controversies
- Game-related adaptations, animation, film, music, merchandise, and events
- Player-community controversies or high-attention discussions

## Source Priority

Use sources in this order when possible:

1. Official announcements: studio/publisher/platform blogs, press releases, store pages, patch notes.
2. Reputable game and industry media: IGN, GameSpot, VGC, Eurogamer, GamesIndustry.biz, Gematsu, Famitsu, 4Gamer, Automaton, GameLook, Youxiputao, Gcores, etc.
3. Primary platform data: Steam pages/reviews, PlayStation Store, Nintendo, Xbox, Metacritic/OpenCritic, official esports pages.
4. Community sources: Reddit, ResetEra, X/Twitter, YouTube comments, Steam reviews, Bilibili, Weibo, Tieba, NGA, Zhihu.

When sources disagree, state the uncertainty instead of flattening it into a single claim.

## News Selection Criteria

Prioritize stories that meet at least one of these conditions:

- Affects many players directly, such as release dates, prices, subscriptions, platform rules, or major patches.
- Has clear industry impact, such as acquisitions, layoffs, regulation, financial results, or publishing policy changes.
- Involves high-profile games, studios, creators, franchises, or platforms.
- Has unusually strong community reaction or controversy.
- Adds meaningful context to games the user is likely to care about: cinematic story games, PlayStation first-party titles, major RPGs, open-world games, and visually polished releases.

Avoid filling the digest with minor trailer drops unless the game, studio, or community response is notable.

## Required Daily Structure

Use this Markdown structure:

```markdown
# YYYY-MM-DD 游戏新闻日报

## 今日最重要

### 1. 新闻标题

- 事件：一句话说明发生了什么。
- 重要性：为什么值得关注。
- 影响：对玩家、行业或平台可能产生什么影响。
- 国内态度：国内玩家/网友主要反应，需说明来源平台。
- 国外态度：国外玩家/网友主要反应，需说明来源平台。
- 来源：链接列表。

## 其他值得关注

### 2. 新闻标题
...

## 今日观察

用 2-4 句话总结当天游戏新闻的共同趋势。

## 来源索引

- Source name: URL
```

## Sentiment Rules

Do not invent sentiment. If there is no reliable community signal, write `暂未看到足够明确的玩家反馈`.

When summarizing sentiment:

- Separate domestic and overseas reactions.
- Distinguish consensus from controversy.
- Mention platform context, such as Weibo, Bilibili, NGA, Steam, Reddit, ResetEra, X/Twitter, YouTube.
- Avoid overclaiming from a single comment or small thread.
- Prefer phrasing like `较多讨论集中在...`, `争议点主要是...`, `海外玩家更关注...`.

## GitHub Update Rules

Each daily run should:

1. Create or update `news-YYYY-MM-DD.md`.
2. Update `README.md` so the latest report appears first under `Latest Reports`.
3. Preserve historical report links.
4. Use concise commit messages, for example:
   - `Add 2026-05-29 game news digest`
   - `Update README latest report link`

## Failure Handling

If search, source access, or GitHub write fails, the run should report:

- What failed.
- Which sources were checked.
- Whether the report was partially generated.
- Whether GitHub sync succeeded.
