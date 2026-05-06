## Hi, I'm Mohamed Rafeek  
mohamedrafee2002@gmail.com | [Portfolio](https://rafeemohamed.com/) | [LinkedIn](https://www.linkedin.com/in/rafeemohamed)

I’m a software engineer focused on distributed systems, data systems and backend infrastructure.

I enjoy working on systems from first principles - understanding how they work at a fundamental level and building them with a focus on correctness, reliability and clear trade-offs. My work spans from low-level primitives like consensus and storage engines to higher-level distributed architectures.

I also write about system design and engineering, sharing lessons from building real-world systems.

---

### Skills and Technologies

I primarily work on systems and backend engineering:

* Languages: Java, TypeScript, Python, Rust - building backend services and system components  
* Systems engineering: Concurrency, Distributed systems and storage systems  
* System design: Microservices, event-driven architectures, coordination and consistency models 
* Technologies : PostgreSQL, Elasticsearch, ClickHouse, Redis, Kubernetes, Prometheus, Grafana, AWS - Lamda, S3, DynamoDB, SQS etc.

---

### Building systems from First Principles

I’m interested in exploring foundational systems and infrastructure by building them end-to-end - implementing and understanding the underlying mechanisms from scratch to go beyond abstractions.

#### [Axis - Distributed Key-Value Store](https://github.com/Rafee-Mohamed/axis)

I’m building this to understand how real distributed systems and coordination work - combining consensus, storage, failure modes and system design.

Axis is a fault-tolerant, strongly consistent distributed key-value store designed for coordination, distributed locking and metadata management - inspired by [etcd-io/etcd](https://github.com/etcd-io/etcd).

* Raft-based replication with leader election, failover and crash-safe recovery
* Multi-Versioned storage engine (MVCC) with ACID semantics enabling non-blocking temporal queries
* Linearizable reads
* Leasing system with checkpointing


#### [Jaft - Raft Consensus Protocol](https://github.com/Rafee-Mohamed/jaft)

I built this to deeply understand how consensus works in real systems - leader election, replication and maintaining consistency under failures - inspired by [etcd-io/raft](https://github.com/etcd-io/raft).

Jaft is an implementation of the Raft consensus protocol in Java, built as the consensus layer for Axis.

* Pure state machine design with determisitic execution model 
* Leader election, log replication and joint consensus for dynamic cluster membership  
* Snapshot via log compaction, Quorum confirmed and lease based linearizable reads, Leadership transfer


#### [TimelineDB - MVCC Storage engine](https://github.com/Rafee-Mohamed/timeline-db)

I built this to understand and learn storage engines and MVCC works

An embeddable multi-versioned storage engine enabling time-travel queries built on LMDB.

* Implements a non-blocking single-writer, multi-reader concurrency model and timeline of historical states 
* Uses [versioned-index](https://github.com/Rafee-Mohamed/versioned-index), an ordered key-value index based on Persistent (copy-on-write) B+tree for key timline indexing enabling efficient lock-free reads and atomic writes
* Supports snapshot isolated point and range reads, batched writes and incremental background compaction

---
Thanks for reading - always up for a conversation about systems, trade-offs, and interesting engineering problems.
