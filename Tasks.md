---
title: Tasks
created: 2024-08-21 12:43
modified: 2025-09-03 23:55
tags:
  - tasks
  - aggregator
aliases: []
url: 
summary: 
cssclasses:
  - smaller-note
---

# Global Tasks

```dataview
TASK
WHERE !completed
AND text != ""
SORT date(created, "yyyy-MM-dd HH:mm") DESC
LIMIT 30
```
