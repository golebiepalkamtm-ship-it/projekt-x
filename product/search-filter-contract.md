# Search Filter Contract

Every filter has a display name, data source, permitted audience, default, empty behavior, inclusive/exclusive semantics, privacy impact, index owner, and analytics definition. Filters may not reveal a hidden population through counts, autocomplete, error differences, or timing.

The API normalises filters into a versioned query object. Invalid or unavailable filters return a safe validation error; ignored filters are never silently accepted. Saved searches store only the data needed for the feature and obey privacy changes.
