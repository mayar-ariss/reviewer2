---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?spin(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:1|2|3|4|5|6|7)\b)'
match: not_contains
weight: 1
---

The review does not cite a spin rule by file and number (it may say the spin checks were not run).
