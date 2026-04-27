# ThreatForge
LLM-powered pipeline that takes a CVE URL and generates a Splunk detection rule using Claude and LangFlow.

## How it works
1. Paste a CVE URL as input
2. LangFlow fetches and extracts the page content
3. Claude generates a targeted Splunk detection rule
4. Output is saved as a text file — one rule per CVE

## Example
**Input:** `https://cvedb.shodan.io/cve/CVE-2026-2370`
**Output:** see [splunk_cve_rules.txt](splunk_cve_rules.txt)

## Setup
- Install [LangFlow](https://langflow.org)
- Add your Anthropic API key to the Claude component
- Import `threatforge_pipeline.json` into LangFlow
- Paste a CVE URL and run

## Stack
`LangFlow` `Claude (Anthropic)` `Splunk`

## Legal Notice
For defensive security use only. Validate all generated rules before deploying to production.

## License
MIT © [Abhi Jayaswal](https://github.com/abhij2503)
