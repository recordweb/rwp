# Changelog — RecordWeb Protocol (RWP)

All notable changes to this specification are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
Versioning follows [Semantic Versioning](https://semver.org/).

---

## [0.0.3] – 2026-08-06

Editorial: required standards and references

This version refines the way RWP lists and references external standards, in order to distinguish clearly between technical dependencies and conceptual/contextual frameworks:

- Narrowed Section 2.3 (“Required standards”) to include only those standards that are technically required for RWP conformance (e.g. DID Core, JSON Canonicalization Scheme, Ed25519, JSON Schema). Conceptual and contextual standards such as ISO 15489, ISO 14721 (OAIS), and national frameworks (e.g. eCH-0164) are no longer listed as “required”.
- Cleaned up the RWP bibliography.

These changes simplify the dependency landscape for implementers: RWP now lists only its true technical requirements, while keeping conceptual relationships to archival and records management standards in the descriptive sections and in RWC.

## [0.0.2] – 2026-08-04

Editorial alignment between RWC and RWP:

- RWC §11.3: aligned metadata field names to camelCase (`accessPolicy`, `deletionRegime`)
- RWP §9.5: corrected pseudocode return types and restored missing bracket
- RWP §14.1: removed duplicate chapter reference in Level 2 conformance list
- Both documents: added explicit `Version: 0.0.2` in Bikeshed metadata

## [0.0.1] — 2026-06-26

### Added
- Initial draft version: all 14 chapters and Annexes A–C
- Chapter 2: Record Identity (DID), `did:rwp` method specification
- Chapter 3: Record Structure, snapshot definition, minimum metadata set
- Chapter 4: Payload and Formats, multi-representation, archival-grade formats
- Chapter 5: Record Types and Schemas, SchemaRecord, core Record types
- Chapter 6: States and Transitions, finalisation requirements
- Chapter 7: Version Graph (DAG), branches, merges, cross-Record merges
- Chapter 8: Case Specification, hard/soft links, Merkle root calculation
- Chapter 9: Integrity and Hashing Procedures, SHA-256, RFC 8785, Ed25519
- Chapter 10: Optional Ledger Anchoring (Hyperledger Fabric)
- Chapter 11: Access Control Delegation Framework
- Chapter 12: Federation, DNS-analogous namespace model
- Chapter 13: Payload Deletion, DeletionRecord protocol
- Chapter 14: Conformance Requirements (Level 1 and Level 2)
- Annex A: Normative JSON Schemas (Snapshot, CaseRecord, DeletionRecord)
- Annex B: Reference Implementation Notes (non-normative)
- Annex C: Change Log

### Notes
- Published baseline: https://doi.org/10.5281/zenodo.20475345
- Not yet approved for production implementations
