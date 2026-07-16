# Search and Recommendation Architecture

Search supports keyword, faceted, geo, autocomplete, saved-query, and—when approved—semantic retrieval. The index is a minimised projection rebuilt from durable events; it is never the authority for access or policy state.

Recommendation supports content-based, collaborative, trending, nearby, history, popularity, similarity, and cold-start strategies. Eligibility and safety filtering precede ranking. Explanations, reset controls, evaluation, and rollback are mandatory.
