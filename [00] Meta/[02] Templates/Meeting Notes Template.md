<%*
const date = tp.date.now("YYYY-MM-DD");
const customTitle = await tp.system.prompt("Enter a title for the meeting") || "Untitled";
const fullTitle = `${date} - ${customTitle}`;
await tp.file.rename(fullTitle); // Rename the file with date and title
-%>
---
title: <% fullTitle %>
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
modified: <% tp.date.now("YYYY-MM-DD HH:mm") %>
tags:
  - 
  - meeting
aliases: []
url: ""
summary: ""
---

# <% fullTitle %>

**Attendees:**  
- 

## Agenda

## Notes

## Action Items
