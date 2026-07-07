# RecordWeb Protocol (RWP)

**Status:** CG Input - Editor's Draft  
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

## Repository Structure
index.bs ← Bikeshed source (edit this)
index.html ← Auto-generated (do not edit)
CHANGELOG.md ← Version history
.github/
workflows/
build.yml ← Auto-build on push

## License

Current draft: published under [W3C Software and Document License] for discussion. Future CG specification: will follow W3C Community Group report licensing and CLA requirements.

## Related

- [RecordWeb Concept (RWC)](https://recordweb.github.io/rwc/) — Conceptual foundation
- [RecordWeb Community Group](https://www.w3.org/community/recordweb/) — W3C CG
