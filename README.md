# AI Instagram Reels Automation 

An end-to-end AI automation system that:
- Fetches trending Computer Science & Tech topics
- Generates viral 60-second Instagram Reel scripts using LLMs
- Uses human-in-the-loop approval
- (Upcoming) Generates AI avatar videos with cloned voice
- (Upcoming) Automatically posts to Instagram

Built using **n8n + Python + Open-Source AI tools**.

---

## Project Goal

To fully automate the creation and posting of Instagram Reels for the niche:
“Trending Topics in CSE & Technology”

The system balances automation with quality using two approval stages.

---

## System Architecture (High-Level)

Phase-based modular architecture:
1. Content Engine (Trending Topics + Script Generation) ✅
2. Clone Engine (Voice + Avatar) ⏳
3. Editing Engine (Captions, B-roll, Music) ⏳
4. Deployment Engine (Instagram Posting) ⏳

---

## Phase 1 – Content Engine (Completed)

### Features
- Fetches trending repositories from GitHub
- Converts trends into viral Instagram Reel scripts using LLMs
- Sends scripts to Telegram for approval
- Stores approved scripts for downstream processing

### Tech Used
- n8n (workflow orchestration)
- GitHub Search API
- LLM (Gemini / OpenAI – pluggable)
- Telegram Bot API
- Python (optional preprocessing)

---

## Repository Structure
workflows/ → n8n workflow exports
scripts/ → Python helper scripts
prompts/ → LLM prompt templates
data/ → Sample approved data (no secrets)
docs/ → Architecture & design notes

---

## Security & Cost
- No paid APIs required for Phase 1
- All API keys injected via environment variables
- Telegram-based human approval prevents bad content

---

## Roadmap
- [x] Phase 1: Content Engine
- [ ] Phase 2: AI Voice & Avatar Generation
- [ ] Phase 3: Video Editing Automation
- [ ] Phase 4: Instagram Auto-Posting

---

## Scripts

These scripts support the n8n workflows and handle logic that is
better suited for Python than no-code tools.

- topic_filter.py → ranks & cleans trending topics
- script_generator.py → generates reel scripts using LLMs

---

##  Author
**Chiranjib Dash**  
B.Tech CSE | Automation & AI Systems  


