# Identity Data Model

Identity owns `Account`, `Credential`, `Session`, `VerificationRequest`, and `VerificationAssertion`. Profile references an account by opaque ID but does not copy credentials or raw identity evidence.

Verification evidence is separated from ordinary account records, encrypted, access-controlled, and retained according to the verification purpose. Assertions expose only the minimum claim needed by a consuming domain, such as an approved eligibility state and expiry.
