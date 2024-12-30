---
layout: post
title: A project on the GFS
date: 2024-12-29 20:56:00
description: Adding exactly-once record append semantics to the Google File System
tags: IIIT systems
categories: software
---

Essentially, I, along with a collaborator, did the following -

1. **Localized Implementation:** Implemented pretty much everything that's offered by the GFS inclusing
    1. Write 
    2. Read
    3. Replication
    4. Record Append
    5. Re-Replication
    6. Stale Replica Handling
    7. Garbage Collection
    8. Operation Log
    9. Data Integrity

using a codebase of 7200 LOC in Go. Evidently, we missed out on snapshoting and directory management and have left them as to-dos.

2. **Enhanced Consistency:** Rather than the at-least once record append operations offered by the GFS, we implemented it to be exactly once. This was done using a modified version of the 2PC protocol and handling idempotency (do see our report!).

3. **Comprehensive System Analysis:** Validated system performance through extensive benchmarking, demonstrating near-linear scaling in throughput for reads, writes, and appends, while maintaining consistency and reliability.

The implementation could be found [here](https://github.com/reimagining-gfs/main-repo) and thr report [here](https://github.com/reimagining-gfs/main-repo/blob/main/report.pdf).
