# Data Classification

| Class | Examples | Handling |
|---|---|---|
| Public | approved marketing copy | integrity protection |
| Internal | non-sensitive operational documentation | authenticated access |
| Confidential | account data, private content, support cases | least privilege, encryption, audited access |
| Restricted | identity evidence, payment data, security secrets | explicit purpose, hardened storage, time-limited access, no routine export |

Classification follows the highest sensitivity in a record. New fields require a classification before collection.
