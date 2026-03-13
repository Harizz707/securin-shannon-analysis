# D1: Shannon Architecture & Agent Communication Analysis

## Shannon Overview
Shannon is an autonomous white-box AI pentester that performs 4-phase security analysis:

### Phase 1: Pre-Recon (Code Analysis)
- Analyzes source code structure
- Identifies endpoints, routes, functions
- Maps user input → data flow
- Finds potential attack surfaces

### Phase 2: Recon (Discovery)
- Discovers HTTP endpoints
- Tests authentication mechanisms
- Identifies API parameters
- Maps application structure

### Phase 3: Vulnerability Analysis (Parallel)
- **Injection Agent**: SQL, command injection
- **XSS Agent**: Stored/reflected XSS
- **SSRF Agent**: Server-side request forgery
- **Auth Agent**: Authentication bypass
- **Authz Agent**: Authorization bypass

### Phase 4: Exploitation & Reporting
- Generates proof-of-concept exploits
- Validates findings against live app
- Only reports vulnerabilities with working PoC

## Key Questions to Answer
1. How do agents communicate between phases?
2. How is context managed across LLM calls?
3. What prompts drive each agent?
4. How are findings compiled into reports?

---

## Agent Architecture Map
[Read /tmp/shannon/src/ and document the orchestration]

## Communication Flow Diagram
[How does pre-recon output feed into recon agents?]

## Context Management Strategy
[How does Shannon avoid LLM context overflow?]
