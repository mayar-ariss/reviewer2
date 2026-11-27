---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?informativeness(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:3|7)\b)'
weight: 1
---

The review cites informativeness rule 3 (truism) or rule 7 (name the property meant) by file and number.
