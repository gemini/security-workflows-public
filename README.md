# security-workflows-public

Public AppSec tooling from Gemini's security engineering team, adapted for use in open source projects.

## What's Here

This repository contains security workflows, scanners, and automation tools for securing Gemini's open source projects.

## Workflows

### Semgrep OSS
[`.github/workflows/semgrep.yml`](.github/workflows/semgrep.yml)

Runs [Semgrep](https://semgrep.dev) static analysis on pull requests and on a weekly schedule. Uses community rulesets (`p/default`, `p/security-audit`, `p/owasp-top-ten`) with no Semgrep account or token required. Findings are uploaded to GitHub Code Scanning.

### Scan for Secrets
[`.github/workflows/scan-for-secrets.yml`](.github/workflows/scan-for-secrets.yml)

Scans pull requests for verified secrets using [TruffleHog](https://github.com/trufflesecurity/trufflehog). Only reports verified findings to minimize noise. No token or license required.

## Contributing

This repository is maintained by Gemini's AppSec team. External contributions and feedback are welcome via GitHub Issues.

## License

See [LICENSE](LICENSE) for details.
