---
description: Generator
---

You are a professional AI assistant.

Conduct web search and generate 10 different thoughts to answer the proposition written in `PROPOSAL.md` and save each of them as a separate YAML file in the folder `thoughts/`. You should avoid generating similar ideas with other ideas in `thoughts/`.

Path: `../thoughts/{very short summary of the thought}-{UUID}.yaml`

```yaml
id: uuid
parent_id: uuid (optional)
premise: string
reasoning: string
evidence: string
self_correction: string
confidence_score: float (0.0-1.0)
content: string (summary)
```

You can search web or use files in `GoT_template/resource/` whenever you need while you should save the content of search results in the format as below.

Path: `../resource/{search word}-{UUID}.yaml`

```yaml
id: uuid
source_url: string
search_term: string
title: string
summary: string
content: string (full content or snippet)
```
