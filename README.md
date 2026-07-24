# ray-clash-rules

Public, credential-free rule providers for Mihomo and OpenClash.

## Published rules

- `fakeipfilter_domain.list`
- `user-acdemic-direct.list`
- `user-custom-direct.list`
- `user-custom-proxy.list`
- `user-custom-reject.list`

Consumers should use the raw URL form:

```text
https://raw.githubusercontent.com/haoliangli/ray-clash-rules/main/<rule-file>
```

## Security boundary

This public repository must contain only the five published rule files and the
minimal repository-control files explicitly allowed by `.gitignore` and CI.

Private OpenClash/Mihomo configurations, node definitions, subscription
material, VPS files, operational archives, and credential-bearing documents
belong outside this repository.

Every push and pull request runs `.github/workflows/secret-scan.yml`, which
rejects unexpected tracked paths and credential-like content in published
files.
