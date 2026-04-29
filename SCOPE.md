# Scope

This index sits next to [AI-Browser-Tools](https://github.com/danielrosehill/AI-Browser-Tools). The two cover adjacent territory and the boundary matters when deciding which one a tool belongs in.

## This index — Scraping-And-Data-Extraction-Resources

**Direct scraping utilities.** Tools whose job is to fetch a URL (or a set of URLs) and return data — HTML, structured fields, Markdown, JSON.

In scope:
- HTTP scrapers and crawlers (scrapy, ferret, Scrapling, jsoup, etc.)
- HTML / metadata parsers (metascraper, markdown-it, scraper)
- LLM-driven extraction (llm-scraper, scrapeghost, ScrapeGraphAI)
- MCP servers that wrap scrape/crawl/markdown-convert as agent tools
- Document extraction (sparrow) when the target is structured data
- Stealth / anti-bot libraries used in service of extraction

Mental model: **input = URL, output = data.** The "browser" (if any) is an implementation detail; the user never sees a page.

## Sibling index — AI-Browser-Tools

**Browser automation and browserless agentic browsing.** Tools where an agent (or human) drives a browser to complete a task — clicking, filling forms, navigating multi-step flows, reading rendered pages.

In scope there:
- Headless / headful browser frameworks pitched at agents (browser-use, Stagehand, Playwright wrappers for LLMs)
- Browserless / cloud-browser services
- Computer-use and screen-driving agents that operate a browser
- Browser extensions that expose the page to an LLM

Mental model: **input = task, output = action.** The browser session is the product.

## Edge cases

- **Headless-browser scraping libraries** (go-rod, puppeteer-style tools) — listed here when they're used as scraping primitives, in AI-Browser-Tools when they're framed as agent infrastructure.
- **Firecrawl, ScrapeGraphAI, Crawl4AI** — listed here. They take a URL and return data, even though they use a browser internally.
- **browser-use, Stagehand, Skyvern** — belong in AI-Browser-Tools. The agent drives the browser; extraction is incidental.
- **MCP servers** — listed here when the tool surface is `scrape(url) → markdown/json`; in AI-Browser-Tools when it's `navigate / click / fill`.

When a tool genuinely spans both, it can be cross-listed with a note pointing to the other index.
