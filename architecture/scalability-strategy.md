# Scalability Strategy

Scale independently by workload: edge/CDN for public media, cache for read projections, queues/workers for asynchronous processing, partitioned data for high-volume domains, and dedicated realtime/media capacity. State-changing paths remain correct under retries and partial outages.

Capacity planning defines peak concurrency, stream fan-out, message throughput, index lag, media processing backlog, and financial reconciliation windows. Horizontal scaling is proven through load tests and failure exercises before launch.
