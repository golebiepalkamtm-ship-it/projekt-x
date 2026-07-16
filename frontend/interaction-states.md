# Interaction States

Every asynchronous control has idle, pending, success, recoverable failure, and unavailable states. Buttons keep their accessible name while pending and prevent duplicate submission without trapping the user. Optimistic UI is permitted only with a reliable reversal path.

Empty states explain what happened, preserve user agency, and never suggest circumventing policy. Error states include a safe next action and correlation ID where support may need it.
