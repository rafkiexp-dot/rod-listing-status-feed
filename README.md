# Encrypted listing-status feed

This repository is a machine-readable transport for encrypted availability
telemetry. `status.json` is encrypted with AES-256-GCM before publication.
It contains no readable listing IDs, URLs, titles, contacts, photos, or scores.

The repository does not use GitHub Actions. A local, scheduled monitor updates
the ciphertext through a repository-scoped deploy key.
