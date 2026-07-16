# Entity: Media Asset Reference

**Owner:** Profile, with storage delegated to an approved asset service. Records include owner aggregate, storage object reference, media type, classification, visibility, processing state, checksum, derivative references, and retention trigger.

Never store public URLs as authority. Access is evaluated through the owning domain, and storage references are not exposed to clients. Deletion removes derivatives and revokes delivery before object lifecycle expiry.
