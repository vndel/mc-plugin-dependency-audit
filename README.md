# Minecraft Plugin Dependency Audit

Release review worksheet for the libraries and build tooling shipped with a Minecraft plugin. A clean dependency report is a point-in-time observation, not a guarantee that an artifact is safe.

## Review checklist
1. Generate a resolved dependency tree for the exact release commit.
2. Identify direct and transitive libraries, licenses, versions, and whether they are shaded or provided by the server.
3. Check for known vulnerabilities and supported upstream releases using approved scanners and advisories.
4. Verify shaded packages are relocated where namespace conflicts are possible.
5. Record exceptions, owners, and remediation dates; rerun the review before publishing.
6. Keep build provenance and artifact checksums with the release.

Do not upload proprietary source or credentials to public scanning services without authorization.

## Files
- `dependency-inventory.csv`: release inventory worksheet.
- `release-review.md`: sign-off record template.