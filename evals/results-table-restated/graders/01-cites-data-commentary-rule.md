---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?data[- ]commentary(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:1|3|4)\b)'
weight: 1
---

The review cites data commentary rule 1, 3 or 4 (commentary not restatement, highlighting, results that do not fit) by file and number.
