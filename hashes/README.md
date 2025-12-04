# PortusSophia™ Artifact Hashes

## Overview

This directory maintains cryptographic hashes of all sealed canonical artifacts for integrity verification.

## Hash Format

Each hash entry must include:

1. Artifact identifier
2. Hash algorithm (SHA-256 minimum)
3. Hash value
4. Seal date
5. Artifact type

## Verification

To verify artifact integrity:

```bash
sha256sum <artifact-file>
```

Compare output against recorded hash. Any mismatch indicates artifact modification and canon violation.

## Hash Records

Hash records are themselves canonical and immutable. New hash records are added for new canonical artifacts only.
