# Observability Standard

Every request receives a correlation ID that propagates to commands, events, provider calls, logs, traces, and operator actions. Logs are structured and classified; they exclude secrets and redact personal data by default.

Service dashboards answer: is the service available, is it correct, is it timely, is it safe, and who owns the next action? Alerts use user impact and error budgets, not raw infrastructure noise. Operators can reconstruct a sensitive decision without inspecting unrestricted raw data.
