---
layout: post
title: Threat Hunting Checklist
categories: blue-team
tags:
    - threat-hunting
    - checklist
date: 2025-12-19
---

This is a resource for threat hunting in the cyber domain


### Threat Hunting Checklist
#### Endpoint Events
- [ ] Process Start and Stop Events
- [ ] Command-line arguments supplied to process
- [ ] Process hierarchy (parent process of each process)
- [ ] Details of modules (DLLs) loaded by process
- [ ] File hashes (including import hashes) of every executable program run and every module loaded
- [ ] Digitial signatures (or lack therof) and version metadata for each and every program
- [ ] Files written by process
- [ ] Selected registry keys and values created and written by processes
- [ ] DNS lookup and network communication by processes
- [ ] Security events including logon, logoff and indentification of remote hosts
- [ ] Web browser history

#### Network Events
- [ ] Netflow data (metadata about all network connections, not the content)
- [ ] Identification of network protocols detected
- [ ] Extraction of executable files sent across the network

#### Server Log Events
- [ ] DNS log of queries and responses (all types, including TXT records)
- [ ] HTTP proxy records of requests and metadata about responses
- [ ] Firewall logs (allowed and blocked connections)
- [ ] DHCP logs (allowes and blocked connections)
- [ ] Domain Controller authentication logs
- [ ] Email server logs, including metadata for email messages sent/recieved





### Acknowledgements
This checklist is taken heavily from Binary Defense Threat Hunters Checklist
- https://binarydefense.nyc3.digitaloceanspaces.com/docs/ThreatHuntersCheckList_BinaryDefense.pdf



[back](../index.md)