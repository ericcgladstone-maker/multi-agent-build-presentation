# Building and validating a multi-agent research system with an AI agent

Eric Gladstone · research walkthrough · independent work · September 2026. The presentation's own header reads "Experimental rehearsal · Multi-agent system".

A real Claude Code session, presented as it was worked through. The Claude Code console is on the left and my commentary is on the right. Starting from a short research brief, the session builds the instrument for a computational experiment on information mutation: a system that sends the same source text through differently structured networks of stateless language-model agents and records how it changes at each step. It formalizes the phenomenon, represents the architectures as testable graphs, builds routing and provenance with deterministic checks, inserts the model behind a controlled interface, traces single runs node by node, builds and validates measures of information change, encodes the proposed study as an explicit matrix, and ends with a completed, verified build. The study itself is not run and no results are reported.

- **Live:** https://multiagentbuild.eric-c-gladstone.workers.dev
- **Also at:** https://graystoneindustries.co/talks/ (embedded)

## What is verbatim and what is editorial

The questions are mine. Claude's replies and tool output are verbatim, from one continuous session (Claude Code 2.1.283, Opus 5.5), recorded 28 September 2026. Turns 1–17 follow the planned sequence; turns 18–19 were adapted so the session stops before a study run; turn 20 was added after Claude asked whether to finish the one missing component. The experimental agents are Claude Haiku 4.5 and Sonnet 4.6 calls made through the `claude` command; the session found that this route adds hidden account context to each call and reports it as a failing check. Timing, grouping into parts, focus, and the commentary on the right are editorial.

The source texts are fictional, written for this demonstration. The session ran in an isolated directory; the account name and email are removed from the published data.

## Use

Open it and step with ← →. Use shift+← → to move between sections and space to play. A− / A+ (or the - and = keys) change the terminal text size. URL options: `?s=<screen>&b=<part>` opens at a given point, `?play=1` autoplays, `?t=<px>` sets the terminal size, and `?embed=1` fills its frame for embedding.

Run locally with any static server, for example `python3 -m http.server 4730 --directory public`.

## Files

`public/` is the whole site: `index.html`, `app.js`, `style.css`, `data/session.js` (the session, as the page plays it), `data/walkthrough.js` (the commentary), self-hosted Geist fonts, and `vendor/marked.umd.js` (MIT) for rendering Markdown. It makes no third-party requests.
