---
type: regex
target: last_message
flags: i
pattern: '(?:\b(?:rules/)?argument(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:2|4)\b)|(?:\b(?:rules/)?claims(?:\.md)?`?,?\s+rules?\s+(?:\d+\s*(?:[–-]|,|and|&)\s*)*(?:4)\b)'
weight: 1
---

The review cites argument rule 2 or 4 (warrant, strength) or claims rule 4 (certainty the evidence supports) by file and number.
