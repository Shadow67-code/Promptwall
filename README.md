# PROMPTWALL

**Firewalling the Conversation Between AI Agents.** PromptWall is a browser-only cybersecurity research and hackathon prototype. It demonstrates how an explainable security layer can inspect simulated messages before delivery between collaborating AI agents.

## Run

Open `index.html` in a modern browser. No Node.js, API keys, installation, network service, or backend is required. Open `tests.html` to run browser self-tests.

## Demo walkthrough

1. Click **Run Attack Simulation** on the dashboard.
2. Launch **Compromised Agent**.
3. Watch PromptWall intercept the fictional Research → Finance message.
4. Inspect transparent intent, policy, threat, risk, and decision evidence.
5. Visit Threat Center and Audit Logs, then use Security Playground to test another safe example.

## Detection methodology

The deterministic prototype combines message structure, contextual patterns, semantic intent categories, protected-resource indicators, role policy and behavioral-anomaly signals. Scores are capped at 100: 0–20 LOW/ALLOW, 21–50 MEDIUM/WARN, 51–75 HIGH/BLOCK, 76–100 CRITICAL/BLOCK. It includes a context exception so a security discussion about “prompt injection” is not automatically malicious.

## Architecture

Source Agent → Interceptor → Parser → Intent Engine → Policy Engine → Risk Engine → Decision → Audit Log / Destination. Six fictional agents have separate allowed and restricted capabilities. The audit log can export CSV locally.

## Deployment

Upload all files unchanged to GitHub Pages, Netlify, Vercel static hosting, Cloudflare Pages, or any static web host. There are no server-side assumptions.

## Limitations and ethics

This is a simulated, explainable cybersecurity research/demo prototype. It does not replace production security controls, does not guarantee detection accuracy, and performs no network scanning, credential collection, offensive action, or external system access. Production deployments need calibrated models, authentication, secure audit storage, privacy review and human oversight.

## Suggested five-minute presentation

Problem (45s): agent messages form a semantic attack surface.  Solution (45s): PromptWall is a policy-aware message boundary.  Demo (2m): launch Compromised Agent and show evidence.  Architecture (45s): explain the pipeline and deterministic risk.  Impact/limits (45s): visibility and enforcement, plus clear prototype boundaries.

## AI usage disclosure template

“This prototype used AI assistance for implementation and interface drafting. Detection rules, demo data, testing, and final review were validated by the project team. All security scenarios are fictional and simulated.”

## Features

Dashboard, deterministic live demo mode, agent network/trust model, eight safe simulations, explainable detector, policy engine, threat center, playground, filterable audit logs and CSV export, responsive keyboard-accessible navigation, architecture explanation, and browser self-tests.
