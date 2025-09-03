<%*

let fullTitle = tp.file.title;

if (fullTitle.startsWith("Untitled")) {
  const customTitle = await tp.system.prompt("Enter a title for the note") || "Untitled";
  fullTitle = customTitle;
  await tp.file.rename(fullTitle);
}

-%>
---
title: <% fullTitle %>
created: <% tp.date.now("YYYY-MM-DD HH:mm") %>
modified: <% tp.date.now("YYYY-MM-DD HH:mm") %>
tags:
  - 
  - aliases: []
url: ""
summary: ""
---

# <% fullTitle %>
