# Scraping And Data Extraction Resources

A curated index of tools, libraries, frameworks, and utilities for scraping web data — with a focus on packaging extracted data for consumption by AI agents (RAG pipelines, LLM context, agent tools).

**Snapshot:** 2026-04-29

> Each entry uses dynamic badges for ⭐ star count and last-updated date — the values refresh automatically when GitHub state changes.

---

## Scope

This index covers:

- **Scrapers & crawlers** — headless browser automation, HTTP scrapers, site mirrors
- **Extraction & parsing** — HTML → structured data, readability/article extractors, markdown converters
- **AI-ready packaging** — LLM-optimized scrapers and converters that output Markdown, JSON, or chunked text suitable for embeddings, RAG ingestion, or direct LLM context
- **Agent integrations** — MCP servers exposing scraping/extraction as tools to LLM agents
- **Anti-bot & rendering** — JS rendering, stealth/fingerprinting, proxy rotation utilities

For headless-browser automation aimed at agentic browsing (rather than data extraction), see the related index **[AI-Browser-Tools](https://github.com/danielrosehill/AI-Browser-Tools)**.

---

## Table of Contents

- [LLM-Optimized Scrapers](#llm-optimized-scrapers)
- [MCP Servers](#mcp-servers)
- [Frameworks / Tools](#frameworks--tools)
- [Extractors & Parsers](#extractors--parsers)
- [Markdown Conversion](#markdown-conversion)
- [Document & Component Extraction](#document--component-extraction)
- [Mobile](#mobile)
- [Use Cases & Recipes](#use-cases--recipes)
- [Israel-Specific](#israel-specific)
- [Awesome Lists](#awesome-lists)
- [Related Indexes](#related-indexes)

---

## LLM-Optimized Scrapers

Scrapers designed to feed LLMs directly — schema-driven extraction, structured output, AI-friendly formats.

### llm-scraper

Turn any webpage into structured data using LLMs (Node.js, schema-driven via Zod).

![Stars](https://img.shields.io/github/stars/mishushakov/llm-scraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/mishushakov/llm-scraper?style=flat)

[mishushakov/llm-scraper](https://github.com/mishushakov/llm-scraper)

### scrapeghost

Experimental Python library for scraping websites using OpenAI's GPT — pass a URL and a schema, get structured data.

![Stars](https://img.shields.io/github/stars/jamesturk/scrapeghost?style=flat) ![Last commit](https://img.shields.io/github/last-commit/jamesturk/scrapeghost?style=flat)

[jamesturk/scrapeghost](https://github.com/jamesturk/scrapeghost)

### scrapecraft

Visual builder for ScrapeGraphAI agentic scraping pipelines.

![Stars](https://img.shields.io/github/stars/ScrapeGraphAI/scrapecraft?style=flat) ![Last commit](https://img.shields.io/github/last-commit/ScrapeGraphAI/scrapecraft?style=flat)

[ScrapeGraphAI/scrapecraft](https://github.com/ScrapeGraphAI/scrapecraft)

### firecrawl

Production-grade web crawler that turns sites into LLM-ready Markdown / structured data — the engine behind the Firecrawl service.

![Stars](https://img.shields.io/github/stars/mendableai/firecrawl?style=flat) ![Last commit](https://img.shields.io/github/last-commit/mendableai/firecrawl?style=flat)

[mendableai/firecrawl](https://github.com/mendableai/firecrawl)

### Scrapegraph-ai

Python library for LLM-driven web scraping — describe what you want in natural language, get structured data.

![Stars](https://img.shields.io/github/stars/ScrapeGraphAI/Scrapegraph-ai?style=flat) ![Last commit](https://img.shields.io/github/last-commit/ScrapeGraphAI/Scrapegraph-ai?style=flat)

[ScrapeGraphAI/Scrapegraph-ai](https://github.com/ScrapeGraphAI/Scrapegraph-ai)

### crawl4ai

LLM-friendly web crawler with adaptive extraction, JS rendering, and Markdown output.

![Stars](https://img.shields.io/github/stars/unclecode/crawl4ai?style=flat) ![Last commit](https://img.shields.io/github/last-commit/unclecode/crawl4ai?style=flat)

[unclecode/crawl4ai](https://github.com/unclecode/crawl4ai)

### gpt-crawler

Crawl a site and produce a single knowledge file you can drop into a custom GPT or RAG pipeline.

![Stars](https://img.shields.io/github/stars/BuilderIO/gpt-crawler?style=flat) ![Last commit](https://img.shields.io/github/last-commit/BuilderIO/gpt-crawler?style=flat)

[BuilderIO/gpt-crawler](https://github.com/BuilderIO/gpt-crawler)

### llmsherpa

Layout-aware document extraction for LLMs — preserves sections, tables, and lists from PDFs/HTML.

![Stars](https://img.shields.io/github/stars/nlmatics/llmsherpa?style=flat) ![Last commit](https://img.shields.io/github/last-commit/nlmatics/llmsherpa?style=flat)

[nlmatics/llmsherpa](https://github.com/nlmatics/llmsherpa)

---

## MCP Servers

MCP servers that expose scraping, crawling, or markdown-conversion capabilities to AI agents.

### markdown-downloader

MCP server that downloads webpages and converts them to Markdown for agent consumption.

![Stars](https://img.shields.io/github/stars/dazeb/markdown-downloader?style=flat) ![Last commit](https://img.shields.io/github/last-commit/dazeb/markdown-downloader?style=flat)

[dazeb/markdown-downloader](https://github.com/dazeb/markdown-downloader)

### markdownify-mcp

MCP server for converting files and web content (PDFs, images, audio, YouTube, web pages) into Markdown.

![Stars](https://img.shields.io/github/stars/zcaceres/markdownify-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/zcaceres/markdownify-mcp?style=flat)

[zcaceres/markdownify-mcp](https://github.com/zcaceres/markdownify-mcp)

### firecrawl-mcp-server

Official MCP server for Firecrawl — web crawling, scraping, and structured extraction.

![Stars](https://img.shields.io/github/stars/firecrawl/firecrawl-mcp-server?style=flat) ![Last commit](https://img.shields.io/github/last-commit/firecrawl/firecrawl-mcp-server?style=flat)

[firecrawl/firecrawl-mcp-server](https://github.com/firecrawl/firecrawl-mcp-server)

### scrapegraph-mcp

Official MCP server for ScrapeGraphAI — agentic, schema-driven web scraping.

![Stars](https://img.shields.io/github/stars/ScrapeGraphAI/scrapegraph-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/ScrapeGraphAI/scrapegraph-mcp?style=flat)

[ScrapeGraphAI/scrapegraph-mcp](https://github.com/ScrapeGraphAI/scrapegraph-mcp)

### supadata mcp

MCP server for Supadata — structured data extraction from web, YouTube, and documents.

![Stars](https://img.shields.io/github/stars/supadata-ai/mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/supadata-ai/mcp?style=flat)

[supadata-ai/mcp](https://github.com/supadata-ai/mcp)

### mcp-read-website-fast

Fast, lightweight MCP server for reading webpages and returning clean Markdown.

![Stars](https://img.shields.io/github/stars/just-every/mcp-read-website-fast?style=flat) ![Last commit](https://img.shields.io/github/last-commit/just-every/mcp-read-website-fast?style=flat)

[just-every/mcp-read-website-fast](https://github.com/just-every/mcp-read-website-fast)

### webclaw

MCP server for web scraping and content extraction.

![Stars](https://img.shields.io/github/stars/0xMassi/webclaw?style=flat) ![Last commit](https://img.shields.io/github/last-commit/0xMassi/webclaw?style=flat)

[0xMassi/webclaw](https://github.com/0xMassi/webclaw)

### linkedin-mcp-server

MCP server for scraping LinkedIn profiles and data.

![Stars](https://img.shields.io/github/stars/eliasbiondo/linkedin-mcp-server?style=flat) ![Last commit](https://img.shields.io/github/last-commit/eliasbiondo/linkedin-mcp-server?style=flat)

[eliasbiondo/linkedin-mcp-server](https://github.com/eliasbiondo/linkedin-mcp-server)

### crawl4ai-mcp-server

MCP server wrapping Crawl4AI — LLM-friendly web crawler with adaptive extraction.

![Stars](https://img.shields.io/github/stars/sadiuysal/crawl4ai-mcp-server?style=flat) ![Last commit](https://img.shields.io/github/last-commit/sadiuysal/crawl4ai-mcp-server?style=flat)

[sadiuysal/crawl4ai-mcp-server](https://github.com/sadiuysal/crawl4ai-mcp-server)

### crawlbase-mcp

Official MCP server for the Crawlbase scraping API.

![Stars](https://img.shields.io/github/stars/crawlbase/crawlbase-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/crawlbase/crawlbase-mcp?style=flat)

[crawlbase/crawlbase-mcp](https://github.com/crawlbase/crawlbase-mcp)

### mcp-web-scrape

MCP server exposing web-scraping tools to LLM agents.

![Stars](https://img.shields.io/github/stars/mukul975/mcp-web-scrape?style=flat) ![Last commit](https://img.shields.io/github/last-commit/mukul975/mcp-web-scrape?style=flat)

[mukul975/mcp-web-scrape](https://github.com/mukul975/mcp-web-scrape)

### mcp-server-docy

MCP server for fetching and serving documentation pages to agents.

![Stars](https://img.shields.io/github/stars/oborchers/mcp-server-docy?style=flat) ![Last commit](https://img.shields.io/github/last-commit/oborchers/mcp-server-docy?style=flat)

[oborchers/mcp-server-docy](https://github.com/oborchers/mcp-server-docy)

### scraper-mcp

MCP server wrapping a general-purpose web scraper.

![Stars](https://img.shields.io/github/stars/cotdp/scraper-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/cotdp/scraper-mcp?style=flat)

[cotdp/scraper-mcp](https://github.com/cotdp/scraper-mcp)

### browsegenie

Browser-driven scraping MCP — agent-controlled page extraction.

![Stars](https://img.shields.io/github/stars/PushpenderIndia/browsegenie?style=flat) ![Last commit](https://img.shields.io/github/last-commit/PushpenderIndia/browsegenie?style=flat)

[PushpenderIndia/browsegenie](https://github.com/PushpenderIndia/browsegenie)

### opencode-browser

Browser tool integration for OpenCode — fetch and extract page content for agent context.

![Stars](https://img.shields.io/github/stars/michaljach/opencode-browser?style=flat) ![Last commit](https://img.shields.io/github/last-commit/michaljach/opencode-browser?style=flat)

[michaljach/opencode-browser](https://github.com/michaljach/opencode-browser)

### markitdown_mcp_server

MCP server wrapping Microsoft's `markitdown` — convert files and URLs to Markdown for LLM consumption.

![Stars](https://img.shields.io/github/stars/KorigamiK/markitdown_mcp_server?style=flat) ![Last commit](https://img.shields.io/github/last-commit/KorigamiK/markitdown_mcp_server?style=flat)

[KorigamiK/markitdown_mcp_server](https://github.com/KorigamiK/markitdown_mcp_server)

### scrapling-fetch-mcp

MCP server wrapping Scrapling — undetectable, adaptive page fetching exposed as an agent tool.

![Stars](https://img.shields.io/github/stars/cyberchitta/scrapling-fetch-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/cyberchitta/scrapling-fetch-mcp?style=flat)

[cyberchitta/scrapling-fetch-mcp](https://github.com/cyberchitta/scrapling-fetch-mcp)

### html-to-markdown-mcp

MCP server that converts arbitrary HTML to clean Markdown — ideal for piping scraped pages into LLM context.

![Stars](https://img.shields.io/github/stars/levz0r/html-to-markdown-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/levz0r/html-to-markdown-mcp?style=flat)

[levz0r/html-to-markdown-mcp](https://github.com/levz0r/html-to-markdown-mcp)

---

## Frameworks / Tools

General-purpose scraping frameworks and libraries across languages.

### scrapy

The canonical Python framework for large-scale web crawling and scraping.

![Stars](https://img.shields.io/github/stars/scrapy/scrapy?style=flat) ![Last commit](https://img.shields.io/github/last-commit/scrapy/scrapy?style=flat)

[scrapy/scrapy](https://github.com/scrapy/scrapy)

### ferret

Declarative, query-language-based web scraping (FQL — Ferret Query Language) in Go.

![Stars](https://img.shields.io/github/stars/MontFerret/ferret?style=flat) ![Last commit](https://img.shields.io/github/last-commit/MontFerret/ferret?style=flat)

[MontFerret/ferret](https://github.com/MontFerret/ferret)

### Scrapling

Undetectable, adaptive Python scraping library — auto-heals broken selectors when sites change.

![Stars](https://img.shields.io/github/stars/D4Vinci/Scrapling?style=flat) ![Last commit](https://img.shields.io/github/last-commit/D4Vinci/Scrapling?style=flat)

[D4Vinci/Scrapling](https://github.com/D4Vinci/Scrapling)

### rod

High-level Go wrapper around the Chrome DevTools Protocol — headless browser scraping.

![Stars](https://img.shields.io/github/stars/go-rod/rod?style=flat) ![Last commit](https://img.shields.io/github/last-commit/go-rod/rod?style=flat)

[go-rod/rod](https://github.com/go-rod/rod)

### jsoup

Java library for working with real-world HTML — parsing, manipulation, CSS-selector extraction.

![Stars](https://img.shields.io/github/stars/jhy/jsoup?style=flat) ![Last commit](https://img.shields.io/github/last-commit/jhy/jsoup?style=flat)

[jhy/jsoup](https://github.com/jhy/jsoup)

### scraper (Rust)

HTML parsing and querying with CSS selectors for Rust.

![Stars](https://img.shields.io/github/stars/rust-scraper/scraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/rust-scraper/scraper?style=flat)

[rust-scraper/scraper](https://github.com/rust-scraper/scraper)

### scala-scraper

Scala library for scraping content from HTML pages.

![Stars](https://img.shields.io/github/stars/ruippeixotog/scala-scraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/ruippeixotog/scala-scraper?style=flat)

[ruippeixotog/scala-scraper](https://github.com/ruippeixotog/scala-scraper)

### scrape

Simple, command-line web scraper for Go.

![Stars](https://img.shields.io/github/stars/lawzava/scrape?style=flat) ![Last commit](https://img.shields.io/github/last-commit/lawzava/scrape?style=flat)

[lawzava/scrape](https://github.com/lawzava/scrape)

### linkedin_scraper

Python scraper for LinkedIn profiles, companies, and jobs.

![Stars](https://img.shields.io/github/stars/joeyism/linkedin_scraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/joeyism/linkedin_scraper?style=flat)

[joeyism/linkedin_scraper](https://github.com/joeyism/linkedin_scraper)

### facebook-scraper

Python package for scraping public Facebook posts without API access.

![Stars](https://img.shields.io/github/stars/kevinzg/facebook-scraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/kevinzg/facebook-scraper?style=flat)

[kevinzg/facebook-scraper](https://github.com/kevinzg/facebook-scraper)

### obscura

Stealth scraping toolkit aimed at evading bot detection.

![Stars](https://img.shields.io/github/stars/h4ckf0r0day/obscura?style=flat) ![Last commit](https://img.shields.io/github/last-commit/h4ckf0r0day/obscura?style=flat)

[h4ckf0r0day/obscura](https://github.com/h4ckf0r0day/obscura)

### XActions

Scraper / automation toolkit for X (Twitter) — extract posts, threads, and profile data.

![Stars](https://img.shields.io/github/stars/nirholas/XActions?style=flat) ![Last commit](https://img.shields.io/github/last-commit/nirholas/XActions?style=flat)

[nirholas/XActions](https://github.com/nirholas/XActions)

### crawlee

Production-grade Node.js crawler framework — handles queueing, retries, proxies, and storage.

![Stars](https://img.shields.io/github/stars/apify/crawlee?style=flat) ![Last commit](https://img.shields.io/github/last-commit/apify/crawlee?style=flat)

[apify/crawlee](https://github.com/apify/crawlee)

### crawlee-python

Python port of Crawlee — full-featured crawler framework with HTTP and browser-based fetchers.

![Stars](https://img.shields.io/github/stars/apify/crawlee-python?style=flat) ![Last commit](https://img.shields.io/github/last-commit/apify/crawlee-python?style=flat)

[apify/crawlee-python](https://github.com/apify/crawlee-python)

### requests-html

Pythonic, high-level HTTP scraping library with built-in HTML parsing and JS rendering.

![Stars](https://img.shields.io/github/stars/psf/requests-html?style=flat) ![Last commit](https://img.shields.io/github/last-commit/psf/requests-html?style=flat)

[psf/requests-html](https://github.com/psf/requests-html)

### MechanicalSoup

Python library for automating interaction with websites — wraps Requests and BeautifulSoup.

![Stars](https://img.shields.io/github/stars/MechanicalSoup/MechanicalSoup?style=flat) ![Last commit](https://img.shields.io/github/last-commit/MechanicalSoup/MechanicalSoup?style=flat)

[MechanicalSoup/MechanicalSoup](https://github.com/MechanicalSoup/MechanicalSoup)

---

## Extractors & Parsers

Targeted extraction of metadata, articles, and structured fields.

### metascraper

Library for extracting structured metadata (title, author, image, publication date) from any URL — rule-based.

![Stars](https://img.shields.io/github/stars/microlinkhq/metascraper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/microlinkhq/metascraper?style=flat)

[microlinkhq/metascraper](https://github.com/microlinkhq/metascraper)

### trafilatura

Best-in-class Python library for web text and metadata extraction — article body, comments, publication date, language.

![Stars](https://img.shields.io/github/stars/adbar/trafilatura?style=flat) ![Last commit](https://img.shields.io/github/last-commit/adbar/trafilatura?style=flat)

[adbar/trafilatura](https://github.com/adbar/trafilatura)

### readability

Mozilla's standalone version of the Reader Mode library — turns cluttered pages into clean article text.

![Stars](https://img.shields.io/github/stars/mozilla/readability?style=flat) ![Last commit](https://img.shields.io/github/last-commit/mozilla/readability?style=flat)

[mozilla/readability](https://github.com/mozilla/readability)

### goose3

Article extractor for Python — pulls main text, top image, and metadata from news pages.

![Stars](https://img.shields.io/github/stars/goose3/goose3?style=flat) ![Last commit](https://img.shields.io/github/last-commit/goose3/goose3?style=flat)

[goose3/goose3](https://github.com/goose3/goose3)

### newspaper

Article scraping and curation for Python (newspaper3k) — author, publish date, top image, full text.

![Stars](https://img.shields.io/github/stars/codelucas/newspaper?style=flat) ![Last commit](https://img.shields.io/github/last-commit/codelucas/newspaper?style=flat)

[codelucas/newspaper](https://github.com/codelucas/newspaper)

### cheerio

jQuery-style server-side HTML parsing and manipulation for Node.js — fast and lean.

![Stars](https://img.shields.io/github/stars/cheeriojs/cheerio?style=flat) ![Last commit](https://img.shields.io/github/last-commit/cheeriojs/cheerio?style=flat)

[cheeriojs/cheerio](https://github.com/cheeriojs/cheerio)

### lxml

Fast, feature-rich Python library for processing XML and HTML — backbone of many scrapers.

![Stars](https://img.shields.io/github/stars/lxml/lxml?style=flat) ![Last commit](https://img.shields.io/github/last-commit/lxml/lxml?style=flat)

[lxml/lxml](https://github.com/lxml/lxml)

---

## Markdown Conversion

Markdown parsers and converters useful for normalizing scraped content into agent-friendly format.

### markdown-it

Pluggable, fast Markdown parser for Node.js — CommonMark-compliant.

![Stars](https://img.shields.io/github/stars/markdown-it/markdown-it?style=flat) ![Last commit](https://img.shields.io/github/last-commit/markdown-it/markdown-it?style=flat)

[markdown-it/markdown-it](https://github.com/markdown-it/markdown-it)

### gomarkdown

Markdown parser and renderer for Go.

![Stars](https://img.shields.io/github/stars/gomarkdown/markdown?style=flat) ![Last commit](https://img.shields.io/github/last-commit/gomarkdown/markdown?style=flat)

[gomarkdown/markdown](https://github.com/gomarkdown/markdown)

### markitdown

Microsoft's any-file-to-Markdown converter — handles PDFs, Office docs, images (OCR), audio (transcription), HTML, and more. Canonical input pre-processor for LLMs.

![Stars](https://img.shields.io/github/stars/microsoft/markitdown?style=flat) ![Last commit](https://img.shields.io/github/last-commit/microsoft/markitdown?style=flat)

[microsoft/markitdown](https://github.com/microsoft/markitdown)

---

## Document & Component Extraction

Extracting structured data from documents (PDFs, forms, invoices) — overlaps with web scraping when targets are document-heavy.

### sparrow

ML-driven data extraction from documents — invoices, receipts, forms — with LLM/VLM backends.

![Stars](https://img.shields.io/github/stars/katanaml/sparrow?style=flat) ![Last commit](https://img.shields.io/github/last-commit/katanaml/sparrow?style=flat)

[katanaml/sparrow](https://github.com/katanaml/sparrow)

### unstructured

Open-source library for partitioning, cleaning, and chunking unstructured documents (PDF, DOCX, HTML, images, email) for LLM ingestion.

![Stars](https://img.shields.io/github/stars/Unstructured-IO/unstructured?style=flat) ![Last commit](https://img.shields.io/github/last-commit/Unstructured-IO/unstructured?style=flat)

[Unstructured-IO/unstructured](https://github.com/Unstructured-IO/unstructured)

### docling

IBM's document conversion toolkit — PDF, DOCX, PPTX, images → structured Markdown/JSON with layout understanding.

![Stars](https://img.shields.io/github/stars/DS4SD/docling?style=flat) ![Last commit](https://img.shields.io/github/last-commit/DS4SD/docling?style=flat)

[DS4SD/docling](https://github.com/DS4SD/docling)

### pypdf

Pure-Python PDF library — read, split, merge, extract text and metadata.

![Stars](https://img.shields.io/github/stars/py-pdf/pypdf?style=flat) ![Last commit](https://img.shields.io/github/last-commit/py-pdf/pypdf?style=flat)

[py-pdf/pypdf](https://github.com/py-pdf/pypdf)

### PyMuPDF

High-performance PDF / e-book library (MuPDF bindings) — fast text and image extraction.

![Stars](https://img.shields.io/github/stars/pymupdf/PyMuPDF?style=flat) ![Last commit](https://img.shields.io/github/last-commit/pymupdf/PyMuPDF?style=flat)

[pymupdf/PyMuPDF](https://github.com/pymupdf/PyMuPDF)

---

## Mobile

Scraping and automation targeting mobile apps rather than the web.

### mobile-mcp

MCP server for automating mobile devices (iOS / Android) — scrape, interact, extract.

![Stars](https://img.shields.io/github/stars/mobile-next/mobile-mcp?style=flat) ![Last commit](https://img.shields.io/github/last-commit/mobile-next/mobile-mcp?style=flat)

[mobile-next/mobile-mcp](https://github.com/mobile-next/mobile-mcp)

---

## Use Cases & Recipes

Real-world scraper collections — useful as references and patterns to copy.

### city-scrapers

Civic-tech project scraping public meeting agendas and minutes from local government sites.

![Stars](https://img.shields.io/github/stars/City-Bureau/city-scrapers?style=flat) ![Last commit](https://img.shields.io/github/last-commit/City-Bureau/city-scrapers?style=flat)

[City-Bureau/city-scrapers](https://github.com/City-Bureau/city-scrapers)

### scrapfly-scrapers

Collection of production-grade scraping recipes from Scrapfly — covers many real-world targets (LinkedIn, Amazon, Zillow, etc.).

![Stars](https://img.shields.io/github/stars/scrapfly/scrapfly-scrapers?style=flat) ![Last commit](https://img.shields.io/github/last-commit/scrapfly/scrapfly-scrapers?style=flat)

[scrapfly/scrapfly-scrapers](https://github.com/scrapfly/scrapfly-scrapers)

---

## Israel-Specific

### israeli-bank-scrapers

Scrapers for major Israeli banks and credit-card companies — exports transactions in a normalized format.

![Stars](https://img.shields.io/github/stars/eshaham/israeli-bank-scrapers?style=flat) ![Last commit](https://img.shields.io/github/last-commit/eshaham/israeli-bank-scrapers?style=flat)

[eshaham/israeli-bank-scrapers](https://github.com/eshaham/israeli-bank-scrapers)

---

## Awesome Lists

Upstream curated lists worth referencing.

### awesome-web-scraping

Comprehensive awesome-list of web-scraping tools across languages.

![Stars](https://img.shields.io/github/stars/lorien/awesome-web-scraping?style=flat) ![Last commit](https://img.shields.io/github/last-commit/lorien/awesome-web-scraping?style=flat)

[lorien/awesome-web-scraping](https://github.com/lorien/awesome-web-scraping)

### awesome-mcp-api

Awesome-list of MCP servers exposing APIs and data sources to LLM agents — useful for finding scrape/fetch-style MCP tools.

![Stars](https://img.shields.io/github/stars/kawsarlog/awesome-mcp-api?style=flat) ![Last commit](https://img.shields.io/github/last-commit/kawsarlog/awesome-mcp-api?style=flat)

[kawsarlog/awesome-mcp-api](https://github.com/kawsarlog/awesome-mcp-api)

---

## Related Indexes

- **[AI-Browser-Tools](https://github.com/danielrosehill/AI-Browser-Tools)** — browser automation and browserless agentic browsing. See [SCOPE.md](./SCOPE.md) for disambiguation.

---

## License

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
