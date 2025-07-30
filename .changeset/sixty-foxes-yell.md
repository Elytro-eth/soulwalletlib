---
"@soulwallet/sdk": patch
---

Refactored getUserOpHash to compute the hash using an EIP-712 domain separator for improved standards compliance. Updated test values to match the new hashing logic and adjusted packUserOp encoding to include a type hash.
