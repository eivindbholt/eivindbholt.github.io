---
title: "{{ replace .File.ContentBaseName "-" " " | title }}"
date: {{ .Date }}
draft: true
summary: "One or two sentences: what the challenge was and the key technique."
# Platform / event, e.g. HackTheBox, TryHackMe, picoCTF
categories: ["HackTheBox"]
# Techniques and tools, e.g. web, sqli, privesc, reversing, ghidra
tags: []
---

## Overview

- **Platform:**
- **Category:**
- **Difficulty:**

Short summary of the challenge and the path to the solution.

## Recon

What you looked at first and what you found.

```bash
nmap -sC -sV -oN nmap.txt 10.10.10.10
```

<!-- Images: put them in this same folder and write ![description](filename.png) -->

## Exploitation / Analysis

The main steps, with commands and screenshots. Explain *why* each step works,
not only what you typed.

## Privilege escalation / Getting the flag

## Lessons learned

- What was new to you
- What you would do differently
- How this maps to real-world defence (detection, mitigation)

<!--
Before publishing (draft: false):
- Remove real flags if the platform's rules require it
- Only publish write-ups for retired machines / finished events
- No credentials, tokens or data from real engagements
-->
