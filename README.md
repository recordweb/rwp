# RecordWeb Protocol (RWP)

**Status:** CG Draft — Editor's Draft  
**Version:** 0.0.1  
**Published baseline:** [DOI 10.5281/zenodo.20475345](https://doi.org/10.5281/zenodo.20475345)  
**Editor's Draft:** https://recordweb.github.io/rwp/  
**Editor:** Nik Jenzer, nik@triebwerkstatt.ch 

---

## What is RWP?

The RecordWeb Protocol (RWP) is the normative technical specification for the creation, versioning, linking, and cryptographic proof of Records in RWP-compliant systems.

RWP is the normative counterpart to the [RecordWeb Concept (RWC)](https://recordweb.github.io/rwc/). The RWC describes the conceptual foundations; RWP translates these into binding technical requirements using RFC 2119 compliance terminology.

## Core Ideas

1. Every Record is globally identifiable via a **Decentralized Identifier (DID)**, independent of storage location.
2. Every finalised version is a **cryptographically secured, immutable snapshot** identified by its content hash.
3. All versions form a **Directed Acyclic Graph (DAG)** that structurally anchors the complete history.
4. The **Case Merkle root** aggregates all linked Records into a single, provable fingerprint.

## Conformance Levels

| Level | Chapters | Description |
|---|---|---|
| **Level 1** — Basic | 2, 3, 4, 5, 6, 7, 9 | Record identity, snapshots, payload, hashing, version graph |
| **Level 2** — Full | + 8, 12, 13 | Cases, federation, payload deletion |

## Repository Structure
index.bs ← Bikeshed source (edit this)
index.html ← Auto-generated (do not edit)
CHANGELOG.md ← Version history
.github/
workflows/
build.yml ← Auto-build on push

## License

© 2026 Nik Jenzer

Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
You are free to share and adapt this material with attribution.

This specification serves as **prior art**, preventing third parties from patenting RWP's core technical concepts without acknowledgment.

## Related

- [RecordWeb Concept (RWC)](https://recordweb.github.io/rwc/) — Conceptual foundation
- [RecordWeb Community Group](https://www.w3.org/community/recordweb/) — W3C CG
