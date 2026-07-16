# Entity: Ledger Posting

**Owner:** Commerce. A posting is immutable accounting evidence: transaction ID, debit account, credit account, amount, currency, effective time, source event, reason, and reversal reference.

The transaction balance must equal zero in each currency. Postings are indexed by account, transaction, source event, and effective time. Corrections are new balanced postings; destructive edits are prohibited.
