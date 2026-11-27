---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?informativeness(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:2|3)\b)|(?:\b(?:rules/)?vagueness(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:2|3|4)\b)|(?:\b(?:rules/)?unpacking(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:3|4)\b)'
weight: 1
---

The review cites, by file and number, informativeness rule 2 or 3, vagueness rule 2, 3 or 4, or unpacking rule 3 or 4.
