## Summary and Insights:
https://github.com/Sasao4o/insight-archive


# Systems Projects

A collection of systems projects across distributed systems, databases, operating systems, blockchain, and open-source contributions.

---

## 🌐 Distributed Systems

### Distributed Log Service · C++
A replicated log service built on **Raft** for consensus and replication, **Serf** for cluster membership and node discovery, and **gRPC** for the client and server API.

### Primary/Backup Key-Value Store · Go
A monitor detects failed servers through heartbeats and promotes the backup. The primary forwards every write to the backup before replying, and request IDs ensure retries are applied only once.

### BitTorrent Client · Node.js
Built from scratch with no torrent libraries. It gets peers from a UDP tracker, runs the peer wire protocol over TCP, and downloads 16 KB blocks from many peers at once into the output file.

### MapReduce · Go
*(Princeton COS418 / MIT 6.824)*

### Chandy–Lamport Distributed Snapshots · Go
*(Princeton COS418)*
In a simulator of nodes passing tokens over FIFO links, nodes use markers to record their own state and in-transit messages. Multiple snapshots can run concurrently, and the total token count is preserved in every snapshot.

---

## 🗄️ Databases

### BusTub Educational Database · C++
*(CMU 15-445)*
Buffer pool manager with LRU-K replacement, B+ tree index, and query executors.
The demo shows SQL queries running through the engine and a page moving between disk and memory.

### pg_rusty_statement · Rust
A Postgres extension written in Rust. *Learning project, in progress.*

---

## ⚙️ OS & Low-Level

- **User-Level Threads** · *Stanford CS240, Lab 1*
- **Malloc Allocator** · *CS:APP*
- **Producer–Consumer** · System V shared memory + semaphores

---

## ⛓️ Blockchain

### Blockchain Ledger
Validates transactions (signatures, double spends, amounts) and builds blocks from a pool of pending transactions. Blocks are stored as a tree to handle forks, with the longest branch as the main chain and a UTXO pool per block.

### Auction Smart Contract · Solidity

---

## 🤝 Open Source — ClickHouse

| Contribution | Description |
|---|---|
| **Insert Streaming Graceful Shutdown** | |
| **Named Tuples Pretty Format** | |
| **Atomic `CREATE TABLE AS SELECT`** | Contributed to the PR: the table is not created if the `SELECT` fails. |
| **`optimize_row_order` Performance Investigation** | Benchmarked the setting on four variants of the `hits` dataset: inserts were 20–35% slower (up to 140% on wide tables) for only ~2% better compression. |


## 📚 Books I’ve Read

| Book / Paper | Chapters | Why I Read It |
|------|---------|---------------|
| Agile Principles, Patterns, and Practices in C# | Full Book | I read this to learn how to write **clean, maintainable, and well-structured code**. |
| Head First OOP | Full Book | I read this while studying **OOP** during my college days. |
| The Object-Oriented Thought Process | Full Book | I read this while studying **OOP** during my college days. |
| In Search of an Understandable Consensus Algorithm (Extended Version) | Full Paper | I read this while studying **distributed systems** in college to understand **Raft**. |
| Building Microservices – Designing Fine-Grained Systems | Chapters 2, 5, 10, 11 | I read this because I was curious about **microservice architecture**, as it’s a trendy approach for designing **highly scalable systems**. |
| REST API Design Rule Book | Full Book | I read this while designing **RESTful APIs** for a freelance project to follow **best practices and standards**. |
| Designing Data-Intensive Applications | Chapters 1 to 7 | I read this to get a **practical understanding of how large-scale data systems are designed and operate**. |
| The Design of a Practical System for Fault-Tolerant Virtual Machines | Full Paper | I read this in college while studying **distributed systems**, as we built a **demo project on fault-tolerant virtual machines**. |
| Computer Networking: A Top-Down Approach | Full Book | I read this in college while studying **computer networks**. |
| Distributed Services with Go: Your Guide to Reliable, Scalable, and Maintainable Systems | Full Book | I read this while working on my **graduation project**, which was a simple **distributed log service**. |
| Computer Systems: A Programmer’s Perspective | Chapters 5, 6, 7, 9, 10, 12 | I read this while studying **computer systems** to better understand **low-level concepts**. |
| Database Internals | Part 1 | I read this to deepen my understanding of **databases** |
| Architecture of a Database System – Joseph M. Hellerstein, Michael Stonebraker, James Hamilton | Full Paper | I read this while studying **15‑445** to get a **bird’s-eye view of how database components interact with each other**.|
| Lakehouse: A New Generation of Open Platforms .. | Full Paper | Interested in OLAP internals while following the CMU `15-721` Database course. |
| Python Concurrency with `asyncio` – Matthew Fowler | 1,2,3,4,7 | I'm writing a lot of Python at work lately. Coming from JavaScript, I wanted to understand how Python’s event loop and threading model work under the hood. |
| ClickHouse – Lightning Fast Analytics for Everyone | Full Paper | While contributing to **ClickHouse**, I read this to deepen my understanding of its architecture, as it was difficult to reverse engineer some of the complex parts from the source code. |
| An Empirical Evaluation of Columnar Storage Formats | Full Paper | Following the CMU `15-721` Database course|
| Spark: The Definitive Guide: Big Data Processing Made Simple | Part 1 , Chapter 12,20,21, and 23 | Reading Apache Spark to prep for upcoming projects at work |
| What Goes Around Comes Around... And Around... | Full Paper | What a great paper! |
| MonetDB/X100: Hyper-Pipelining Query Execution | Full Paper | Following the CMU `15-721` Database course |
| MCP Server Architecture Patterns for LLM-Integrated Applications | Full Paper | Working with bunch of mcps at work |
| The End of Software Engineering: How AI Agents Are Fundamentally Restructuring the Software Paradigm | Full Paper |  |
| Extending ResourceLink: Patterns for Large Dataset Processing in MCP Applications | Full Paper | Read MCP large dataset patterns while designing our AI-MCP agent architecture at work.  |
