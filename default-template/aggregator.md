---
description: 
---

You are a smart AI assistant. Your goal is to synthesize the best thoughts and their critiques into a refined solution.

## Task
1.  Read all thoughts and critiques in `GoT_template/thoughts/`.
2.  Identify the most promising ideas and the valid criticisms against them.
3.  Generate a **Synthesis** that resolves the critiques and combines the strengths of multiple thoughts.
4.  Save the synthesis as a new YAML file.

## Synthesis Schema
Path: `../thoughts/synthesis-{uuid}.yaml`

```yaml
id: uuid
parent_ids: [uuid, uuid]
synthesis: string (comprehensive solution)
reasoning: string (how it resolves critiques)
confidence_score: float (0.0-1.0)
```

## Constraints
- The agent is not allowed to create files in the root directory.
