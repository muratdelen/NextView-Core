# NextView-Core

NextView-Core is the NextLife analytics, dashboard and data visualization
distribution.

It extends the official Apache Superset container image with the PostgreSQL
and Redis runtime drivers required by NextLife, then publishes it under the
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

The image keeps the standard Apache Superset runtime and adds
`psycopg2-binary` and `redis`. NextLife-Core provides the PostgreSQL, Redis,
initialization and persistent deployment settings.

## Image Publishing

GitHub Actions builds from the official upstream Superset image and publishes:

- `ghcr.io/muratdelen/nextview-core:latest`
- `ghcr.io/muratdelen/nextview-core:git-<commit>`

No upstream source files, licenses or notices are deleted or modified.
