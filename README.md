# NextView-Core

NextView-Core is the NextLife analytics, dashboard and data visualization
distribution.

It republishes the official Apache Superset container image under the
NextLife GHCR namespace:

```text
ghcr.io/muratdelen/nextview-core:latest
```

## Upstream

- Project: [Apache Superset](https://github.com/apache/superset)
- Official image: [apache/superset](https://hub.docker.com/r/apache/superset)
- License: Apache License 2.0

This repository does not replace or relicense Apache Superset. Upstream
copyright, license, attribution and NOTICE requirements continue to apply.
See [UPSTREAM.md](./UPSTREAM.md).

## NextLife Usage

NextView provides dashboards, charts and user-specific data views for
NextLife modules. Authentication and authorization integrations will be
coordinated through NextID and NextRole.

The image keeps the standard Apache Superset runtime. NextLife-Core provides
the PostgreSQL, Redis, initialization and persistent deployment settings.

## Image Publishing

GitHub Actions copies the configured official upstream Superset image to:

- `ghcr.io/muratdelen/nextview-core:latest`
- `ghcr.io/muratdelen/nextview-core:git-<commit>`

No upstream source files, licenses or notices are deleted or modified.
