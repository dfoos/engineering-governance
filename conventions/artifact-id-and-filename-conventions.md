# Artifact ID and Filename Conventions

This document defines the conventions for artifact IDs and filenames across ADRs, RFCs, and Standards. These conventions ensure consistency, discoverability, and traceability of governance artifacts.

---

## ADR Numbering Format

- **Format**: `adr-<number>-<short-title>.md`
- **Numbering**: Sequential, starting from `001`.
- **Short Title**: A concise, hyphenated summary of the ADR's purpose.
- **Example**: `adr-001-terraform-standardization.md`

### Rules:
1. Numbers are zero-padded to three digits (e.g., `001`, `002`).
2. Titles must be lowercase, hyphenated, and descriptive.
3. Avoid special characters or spaces in titles.

---

## RFC Numbering Format

- **Format**: `rfc-<number>-<short-title>.md`
- **Numbering**: Sequential, starting from `001`.
- **Short Title**: A concise, hyphenated summary of the RFC's purpose.
- **Example**: `rfc-001-cloud-governance.md`

### Rules:
1. Numbers are zero-padded to three digits (e.g., `001`, `002`).
2. Titles must be lowercase, hyphenated, and descriptive.
3. Avoid special characters or spaces in titles.

---

## Standard Naming/Versioning Format

- **Format**: `standard-<name>-v<version>.md`
- **Versioning**: Semantic versioning (`v1.0`, `v2.1`, etc.).
- **Name**: A concise, hyphenated summary of the standard's purpose.
- **Example**: `standard-security-baseline-v1.0md`

### Rules:
1. Use semantic versioning to indicate updates.
   - **Major Version**: Increment the major version (e.g., `v1.0` → `v2.0`) when introducing breaking changes that are not backward compatible.
     - **Example**: A security baseline standard removes support for a deprecated encryption algorithm, requiring teams to update their configurations.
   - **Minor Version**: Increment the minor version (e.g., `v1.0` → `v1.1`) when adding new features or making backward-compatible improvements.
     - **Example**: A security baseline standard adds a new optional control for logging enhancements.
2. Titles must be lowercase, hyphenated, and descriptive.
3. Avoid special characters or spaces in titles.

---

## General File Naming Convention

- **Format**: `<artifact-type>-<identifier>-<short-title>.md`
- **Artifact Types**: `adr`, `rfc`, `standard`.
- **Identifier**: A unique number or version.
- **Short Title**: A concise, hyphenated summary of the artifact's purpose.
- **Example**: `adr-001-terraform-standardization.md`

### Rules:
1. Use the appropriate artifact type prefix (`adr`, `rfc`, `standard`).
2. Ensure filenames are unique within their category.
3. Avoid special characters, spaces, or uppercase letters.

---

## Change Management

1. **New Artifacts**: Follow the numbering and naming conventions when creating new artifacts.
2. **Updates**: Increment the version for standards when making changes.
3. **Deprecation**: Mark deprecated artifacts with a `deprecated` tag in their metadata.

---

These conventions ensure clarity and consistency across all governance artifacts. Adherence to these rules is mandatory for all contributors.
