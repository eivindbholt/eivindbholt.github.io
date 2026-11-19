---
title: "HTB Doubletake"
date: 2026-11-19T20:56:24+01:00
draft: true
summary: "One or two sentences: what the challenge was and the key technique."
# Platform / event, e.g. HackTheBox, TryHackMe, picoCTF
categories: ["HackTheBox"]
# Techniques and tools, e.g. web, sqli, privesc, reversing, ghidra
tags: ["SSH", "nmap", "Alpine", "Linux"]
---

## Overview

- **Platform:** HackTheBox
- **Difficulty:** Easy

IP address: 10.129.102.236

## Recon

I started with a nmap scan to identify open ports, the services running behind them, and the operating system.

```bash
sudo nmap -T4 -sV -sC -p- -A 10.129.102.236
```

This revealed two open ports, and identified the operating system:
- **22**: OpenSSH 10.6 (protocol 2.0)
- **80**: nginx 1.24.0 
- **OS**: MikroTik RouterOS

<!-- Images: put them in this same folder and write ![description](filename.png) -->

## Exploitation / Analysis

According to the provided description, port 22 serves SSH from an Alpine container with OpenSSH 10.6p1 compiled against musl. 


musl is a C standard library intended for operating systems based on the Linux kernel. - [Wikipedia](https://en.wikipedia.org/wiki/Musl)



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
