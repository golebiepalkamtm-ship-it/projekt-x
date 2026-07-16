# Transactional Outbox

The producing domain writes a business change and an outbox record in one transaction. A relay publishes the outbox record with stable event ID, retries safely, and marks delivery separately. Consumers deduplicate independently.

Outbox retention supports replay and incident investigation. Payloads obey event data minimisation, and poison events enter a monitored quarantine rather than blocking unrelated delivery.
