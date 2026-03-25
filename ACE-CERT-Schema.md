# ACE‑CERT Schema  
**ACE Protocol – Constitutional Data Specification**

ACE‑CERT is the canonical, implementation‑neutral data structure for verifiable certificates within the Adaptive Carbon Engine ecosystem.  
This schema defines the mandatory fields, SI units, and structural requirements that all ACE‑compatible systems must follow.

The schema is:

- public  
- deterministic  
- implementation‑agnostic  
- value‑free  
- stable and versioned  

It contains no code, algorithms or engine logic.

---

## Structure Overview

The ACE‑CERT schema consists of the following sections:

- **certificate_id** – unique identifier  
- **timestamp** – ISO 8601 timestamp  
- **soil_params** – physical soil parameters  
- **domain_profile** – categorical domain descriptors  
- **metrics** – aggregated performance indicators  
- **co2e_data** – detailed greenhouse gas accounting  
- **metadata** – contextual information  
- **input** – raw input data used for calculation  
- **hashes** – deterministic integrity anchors  
- **IS** – nitrogen balance components  
- **pools** – opening nitrogen pools  
- **closing** – closing nitrogen pools  
- **mineralisering** – mineralisation estimate  

All fields are required unless explicitly stated otherwise.

---

## Integrity Requirements

Each ACE‑CERT must include a deterministic hash chain:

- **input hash**  
- **scenario hash**  
- **method hash**  
- **calculation hash**

These hashes bind the certificate to its originating data and method.  
A certificate is only valid when its hash chain is anchored in the ACE Ledger.

---

## Units

All physical quantities must use SI units or accepted derivatives:

- mass → kg  
- nitrogen → kg N  
- carbon dioxide equivalents → kg CO₂e  
- area → ha  
- density → g/cm³  
- depth → m  
- volume → m³sk  

---

## Versioning

The schema follows semantic versioning.  
Breaking changes increment the major version.

---

This document defines the normative structure of ACE‑CERT.  
All implementations must follow this specification exactly.
