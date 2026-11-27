---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?numbers(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:2|5|6|8)\b)'
weight: 1
---

The review cites numbers rule 2, 5, 6 or 8 (units, reference, digits, significance) by file and number.
