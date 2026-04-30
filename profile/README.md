# oxide-sloc

**IEEE 1045-1992 compliant source line counter — CLI, web UI, HTML/PDF reports, and CI/CD integration. Built in Rust.**

[![CI](https://github.com/oxide-sloc/oxide-sloc/actions/workflows/ci.yml/badge.svg)](https://github.com/oxide-sloc/oxide-sloc/actions/workflows/ci.yml)
[![Latest Release](https://img.shields.io/github/v/release/oxide-sloc/oxide-sloc?label=release)](https://github.com/oxide-sloc/oxide-sloc/releases/latest)
[![License: AGPL-3.0-or-later](https://img.shields.io/badge/license-AGPL--3.0--or--later-blue.svg)](https://github.com/oxide-sloc/oxide-sloc/blob/main/LICENSE)

---

## What is oxide-sloc?

oxide-sloc counts what matters. It goes beyond simple line counting to implement the [IEEE 1045-1992](https://standards.ieee.org/ieee/1045/788/) standard for physical SLOC measurement — giving you counts you can actually cite in reports, proposals, and compliance documentation.

Most SLOC tools count total lines or blank-stripped lines. oxide-sloc lets you choose: count continuation lines as physical lines or collapse them to logical lines, decide how blanks inside block comments are treated, and track compiler directives separately — all per the standard.

| Capability | Details |
|---|---|
| **Languages** | 41 supported — Rust, C/C++, Python, Go, TypeScript, Java, and more |
| **Interfaces** | CLI / localhost web UI / embeddable summary widget |
| **Output formats** | Plain text / JSON / HTML / PDF / CSV / XLSX |
| **IEEE compliance** | Continuation-line policy / blank-in-block-comment policy / compiler-directive tracking |
| **CI/CD** | GitHub Actions / GitLab CI / Jenkins / Docker / Bitbucket Pipelines |
| **Platforms** | Windows / Linux / macOS |

---

## Why oxide-sloc?

- **Standard-backed counts.** Results are reproducible and citable — not "lines minus blanks."
- **No runtime dependency.** Single static binary. No Python, no Node, no JVM.
- **Web UI included.** Point it at a directory, get an interactive HTML report in the browser.
- **PDF export built in.** Requires a locally installed Chromium-based browser; no cloud calls.
- **CI-native.** Structured JSON output, exit codes, and Docker image for easy pipeline integration.
- **AGPL-licensed.** Free to use, study, and modify.

---

## Quick start

**Download a release binary (Windows x64):**

→ [Latest release](https://github.com/oxide-sloc/oxide-sloc/releases/latest) — grab `oxidesloc-windows-x64.zip` or `oxidesloc-windows-x64.7z`

**Build from source (requires Rust):**

```bash
git clone https://github.com/oxide-sloc/oxide-sloc.git
cd oxide-sloc
bash run.sh          # starts the web UI at http://127.0.0.1:4317
```

**CLI one-liners:**

```bash
oxide-sloc analyze ./my-repo --plain
oxide-sloc analyze ./my-repo --html-out report.html --pdf-out report.pdf
oxide-sloc analyze ./my-repo --json-out result.json
```

---

## Repositories

| Repo | Description |
|---|---|
| [oxide-sloc/oxide-sloc](https://github.com/oxide-sloc/oxide-sloc) | Main source — 6-crate Rust workspace |

---

## Links

- [Releases](https://github.com/oxide-sloc/oxide-sloc/releases)
- [Changelog](https://github.com/oxide-sloc/oxide-sloc/blob/main/CHANGELOG.md)
- [README / Documentation](https://github.com/oxide-sloc/oxide-sloc#readme)
- [Contributing guide](https://github.com/oxide-sloc/oxide-sloc/blob/main/CONTRIBUTING.md)
- [Security policy](https://github.com/oxide-sloc/oxide-sloc/security)
- [License: AGPL-3.0-or-later](https://github.com/oxide-sloc/oxide-sloc/blob/main/LICENSE)
