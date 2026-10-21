# PackDB OSS

Open-source Rust clients and query-language parsers from
[PackDB](https://packdb.io).

PackDB is building observability infrastructure around OpenTelemetry. These
repositories contain supporting components, not the full PackDB platform.

## Projects

| Project | Use it for | Start here |
| --- | --- | --- |
| [PackDB SDK](https://github.com/packdb-oss/packdb-sdk) | SQL client integration over HTTP or Arrow Flight SQL, and W3C trace-context propagation | [README](https://github.com/packdb-oss/packdb-sdk#readme) |
| [PackDB query CLI](https://github.com/packdb-oss/packdb-cli) | Running a SQL query against an existing PackDB endpoint | [README](https://github.com/packdb-oss/packdb-cli#readme) |
| [LogQL parser](https://github.com/packdb-oss/logql-parser) | Parsing LogQL into a typed syntax tree with structured errors | [Supported syntax](https://github.com/packdb-oss/logql-parser#readme) |
| [TraceQL parser](https://github.com/packdb-oss/traceql-parser) | Parsing a supported TraceQL subset into a typed syntax tree | [Supported syntax and limitations](https://github.com/packdb-oss/traceql-parser#readme) |

The parsers do not execute queries. The SDK and CLI require an existing PackDB
endpoint and any credentials required by its operator; they do not provision a
service or issue credentials. `packdb-otel` provides context propagation, not an
OpenTelemetry exporter.

## Releases and Contributions

Start with each project's README for installation, supported versions, platforms,
and compatibility limits. Source releases, and CLI binary archives, are available
through the repositories' GitHub Releases. These packages are not currently
published to crates.io.

The four projects are licensed under Apache-2.0; see each repository's license
and notices. Contributions and questions are welcome through the project's
contribution and support guidelines. Community support is best effort, not a
commercial service-level agreement.

For security reports, follow the affected repository's `SECURITY.md` instead of
opening a public issue. Never include credentials or customer telemetry in public
reports.

[Website](https://packdb.io) |
[LinkedIn](https://www.linkedin.com/company/packdb-io/) |
[X](https://x.com/packdbio) |
[Bluesky](https://bsky.app/profile/packdb.io)
