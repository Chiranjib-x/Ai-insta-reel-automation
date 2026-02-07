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
**“Trending Topics in CSE & Technology”**

The system balances automation with quality using **two approval stages**.

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

