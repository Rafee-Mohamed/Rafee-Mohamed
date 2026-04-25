## Hi, I'm Mohamed Rafeek  
mohamedrafee2002@gmail.com | [Portfolio](https://rafeemohamed.com/) | [LinkedIn](https://www.linkedin.com/in/rafeemohamed)

I’m a software engineer focused on distributed systems, data systems and backend infrastructure.

I enjoy working on systems from first principles - understanding how they work at a fundamental level and building them with a focus on correctness, reliability and clear trade-offs. My work spans from low-level primitives like consensus and storage engines to higher-level distributed architectures.

I also write about system design and engineering, sharing lessons from building real-world systems.

---

### Technologies

I primarily work on systems and backend engineering:

* Languages: Java, TypeScript, Python, Rust - building backend services and system components  
* Systems engineering: Concurrency, Distributed systems and storage systems  
* System design: Microservices, event-driven architectures, coordination and consistency models 
* Data systems: PostgreSQL, Elasticsearch, ClickHouse, Redis etc.

---

### Building systems from First Principles

I’m interested in exploring foundational systems and infrastructure by building them end-to-end - implementing and understanding the underlying mechanisms from scratch to go beyond abstractions.

#### [Axis (WIP) - Distributed Key-Value Store](https://github.com/Rafee-Mohamed/axis)

I’m building this to understand how real distributed coordination systems work - combining consensus, storage, failure modes and system design.

Axis is a fault-tolerant, strongly consistent distributed key-value store designed for coordination, distributed locking and metadata management - inspired by [etcd-io/etcd](https://github.com/etcd-io/etcd).

* Raft-based replication for strong consistency  
* Multi-Versioned storage engine (MVCC) enabling non-blocking temporal queries  
* Linearizable reads  
* Leasing system with checkpointing  


#### [Jaft - Raft Consensus Protocol](https://github.com/Rafee-Mohamed/jaft)

I built this to deeply understand how consensus works in real systems - leader election, replication and maintaining consistency under failures - inspired by [etcd-io/raft](https://github.com/etcd-io/raft).

Jaft is an implementation of the Raft consensus protocol in Java, built as the consensus layer for Axis.

* Pure state machine design  
* Leader election, log replication and membership changes  
* Deterministic execution model  


#### [Versioned Index](https://github.com/Rafee-Mohamed/versioned-index)

Built as the indexing layer for Axis, this explores how atomicity and isolation can be achieved without locking in in-memory indexing under high concurrency.

It is a versioned, ordered key-value index designed for non-blocking single-writer, multi-reader systems.

* Persistent (copy-on-write) B+ tree implementation with structural sharing  
* Snapshot-isolated, lock-free reads  
* Atomic multi-operation transactions  

---
Thanks for reading - always up for a conversation about systems, trade-offs, and interesting engineering problems.
