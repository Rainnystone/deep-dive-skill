# Deep Dive Skill for Claude Code

A research-grade search skill for Claude Code.

## Required MCP Servers

| MCP Server | Installation |
|------------|--------------|
| Exa Search | https://github.com/exa-labs/exa-mcp-server |
| Tavily Search | https://github.com/tavily-ai/tavily-mcp |
| DuckDuckGo | https://github.com/nickclyde/duckduckgo-mcp-server |
| Jina AI | https://github.com/jina-ai/MCP |
| Gemini CLI | https://github.com/jamubc/gemini-mcp-tool |

## Architecture

Phase 1: Broad Collection (Parallel)
- Exa -> Tavily -> DDG fallback
- Jina (Web/arXiv/Blog)
- Gemini Search
- Extended queries

Phase 2: Content Acquisition
- Full article reading via Jina AI

Phase 3: Deep Analysis
- Information Extraction
- Cross-Validation
- Contradiction Detection
- Logical Verification
- Source Tracing
- Causal Deep-Dive (4 levels)
- Credibility Scoring (0-100)

Phase 4: Structured Output
- Executive Summary
- Credibility Overview
- Cross-Validated Facts
- Contradictions Analysis
- Causal Inference
- Source Quality Assessment

## Usage

/deep-dive <query>
/dd <query>
/research <query>
