# J-007: Initiate a Permitted Transaction

This journey remains blocked until RFC-0001 approves the commercial and legal model. When enabled, it will show price, currency, fees, taxes where applicable, fulfilment terms, cancellation/refund rules, provider role, and receipt before authorisation.

Payment initiation is idempotent. A client never determines a final payment state; the Commerce domain reconciles provider webhooks to immutable ledger postings. Failed or pending states give clear next steps without duplicate charges.
