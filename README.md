# SLAB-Hackathon-Webcmd-browser-
SLAB Hackathon project: A self-learning webcmd browser agent that automates live job extraction from Figma Careers and compiles exploratory workflows into zero-token CLI commands.
# 🚀 Figma Careers — SLAB Browser Agent (`webcmd`)

Built for the **SLAB (Self-Learning Agent Browser) Hackathon @ GCELT**.

This project implements an automated **Browser Agent** powered by [`webcmd`](https://github.com/agentrhq/webcmd) and the **CloakBrowser** stealth runtime. It transitions complex, interactive browser navigation into deterministic, sub-second CLI commands—reducing LLM token consumption by up to 90%.

---

## 🌟 Key Features

* **Layer 0 Exploration:** Live DOM inspection, session initialization, and Playwright-style script execution (`temp.js`).
* **Adapter Compilation:** Converts exploratory web interactions into a cached, reusable local adapter (`figma/careers.js`).
* **Zero-Token Deterministic Runs:** Returns structured JSON output instantly without re-invoking LLM browser reasoning.
* **Resilient Architecture:** Handles dynamic DOM changes through accessibility tree snapshots and execution contracts.

---

## 🛠️ Prerequisites & Setup

Ensure `webcmd` and global dependencies are installed:

```powershell
# Install esbuild globally for TypeScript adapter compilation
npm install -g esbuild

# Verify environment setup
webcmd doctor
