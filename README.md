![axiom-syslog-proxy: Syslog ingestion by proxy for Axiom](.github/images/banner-dark.svg#gh-dark-mode-only)
![axiom-syslog-proxy: Syslog ingestion by proxy for Axiom](.github/images/banner-light.svg#gh-light-mode-only)

<div align="center">

[![Documentation][docs_badge]][docs]
[![Go Workflow][workflow_badge]][workflow]
[![Latest Release][release_badge]][release]
[![License][license_badge]][license]

</div>

[Axiom](https://axiom.co) unlocks observability at any scale.

- **Ingest with ease, store without limits:** Axiom's next-generation datastore
  enables ingesting petabytes of data with ultimate efficiency. Ship logs from
  Kubernetes, AWS, Azure, Google Cloud, DigitalOcean, Nomad, and others.
- **Query everything, all the time:** Whether DevOps, SecOps, or EverythingOps,
  query all your data no matter its age. No provisioning, no moving data from
  cold/archive to "hot", and no worrying about slow queries. All your data, all.
  the. time.
- **Powerful dashboards, for continuous observability:** Build dashboards to
  collect related queries and present information that's quick and easy to
  digest for you and your team. Dashboards can be kept private or shared with
  others, and are the perfect way to bring together data from different sources.

For more information check out the
[official documentation](https://axiom.co/docs) and our
[community Discord](https://axiom.co/discord).

## Usage

There are multiple ways you can install the Axiom Syslog Proxy:

- With Homebrew: `brew install axiomhq/tap/axiom-syslog-proxy`
- Download the pre-built binary from the
  [GitHub Releases](https://github.com/axiomhq/axiom-syslog-proxy/releases/latest)
- Using Go: `go install github.com/axiomhq/axiom-syslog-proxy/cmd/axiom-syslog-prox@latest`
- Use the [Docker image](https://hub.docker.com/r/axiomhq/axiom-syslog-proxy): `docker run axiomhq/axiom-syslog-proxy`

### Configuration

If you use the [Axiom CLI](https://github.com/axiomhq/cli), run
`eval $(axiom config export -f)` to configure your environment variables.

Otherwise create a personal token in [the Axiom settings](https://app.axiom.co/profile)
and export it as `AXIOM_TOKEN`. Set `AXIOM_ORG_ID` to the organization ID from
the settings page of the organization you want to access.

Export the dataset name to ingest into as `AXIOM_DATASET`. The dataset must
exist prior to ingesting data into it.

## License

Distributed under the [MIT License](./LICENSE).

<!-- Badges -->

[docs]: https://docs.axiom.co
[docs_badge]: https://img.shields.io/badge/docs-reference-blue.svg
[workflow]: https://github.com/axiomhq/axiom-syslog-proxy/actions/workflows/push.yaml
[workflow_badge]: https://img.shields.io/github/actions/workflow/status/axiomhq/axiom-syslog-proxy/push.yaml?branch=main&ghcache=unused
[release]: https://github.com/axiomhq/axiom-syslog-proxy/releases/latest
[release_badge]: https://img.shields.io/github/release/axiomhq/axiom-syslog-proxy.svg
[license]: https://opensource.org/licenses/MIT
[license_badge]: https://img.shields.io/github/license/axiomhq/axiom-syslog-proxy.svg?color=blue
