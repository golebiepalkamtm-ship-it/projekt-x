# Commerce Data Model

Commerce owns `PaymentIntent`, `ProviderTransaction`, `Order`, `Refund`, `LedgerAccount`, and `LedgerPosting`. Provider identifiers are unique in their provider scope and webhook processing is idempotent.

A posting has debit, credit, currency, amount, transaction reference, effective time, and reason. A transaction is balanced per currency. No other domain writes ledger data directly.
