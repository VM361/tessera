# Tessera

**AI agents now act without clicks. Most interfaces give people no consistent way to see what the agent did, approve it, or undo it.**

Tessera is a design system for products where AI agents take actions on a person's behalf. It defines tokens, components and rules for showing what an agent is doing, asking before it acts, and leaving a trail anyone can audit.

Live demo: _add your GitHub Pages link here_

## What the demo shows

1. **The problem.** The same task run twice: once with no visibility ("Done!"), once with Tessera (steps, checks, approval, undo, audit trail).
2. **Principles.** Agents propose, people decide. Show the work. Mark what the machine made. Autonomy is a setting, not a surprise.
3. **Foundations.** Color tokens with light and dark values, type scale, spacing, radius.
4. **Components.** Button, input, status pill, AI badge, AI-authored content.
5. **Agentic patterns.** Six agent states and a runnable token-audit agent with three autonomy levels: Suggest only, Ask first, Act then report.
6. **Action contract.** Every agent action declares intent, scope, reversibility, checks, sources and actor.

## Run it locally

No build step. Open `index.html` in a browser.

## Publish with GitHub Pages

```bash
git init
git add .
git commit -m "Add Tessera v0.1"
git branch -M main
git remote add origin https://github.com/<your-username>/tessera.git
git push -u origin main
```

Create the empty `tessera` repository on GitHub first. Then open the repository, go to **Settings > Pages**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, and save. The site appears at `https://<your-username>.github.io/tessera/` within a minute or two.

## Status and honesty note

- Version 0.1, a concept. It has not been validated with users yet.
- The agent demos run scripted logic in the browser. The contrast math is real. No AI model is called.
- Planned: usability test of the approval gate with five people, a real model behind the agent through a server function, a React component library with Storybook.

## Roadmap

- [ ] Tokens exported from Figma variables as `tokens.json`
- [ ] React components with tests for contrast and policy rules
- [ ] Policy engine: irreversible actions always need approval
- [ ] Storybook with a story per state
- [ ] Usability test report
