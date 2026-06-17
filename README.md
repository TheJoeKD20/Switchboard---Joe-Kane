<p align="center">
  <img src="https://nexus.joekane.org/assets/switchboard-logo.png" alt="Switchboard" width="96" />
</p>

<h1 align="center">Switchboard</h1>

<p align="center"><b>Every ticket to the right engineer — automatically.</b></p>

<p align="center">A private auto-routing add-on for <a href="https://nexus.joekane.org">Nexus</a> — specialism, availability and load, with a trace behind every call.</p>

<p align="center">
  <a href="https://nexus.joekane.org/switchboard">Overview</a> ·
  <a href="https://nexus.joekane.org/docs#switchboard">Docs</a> ·
  <a href="mailto:joe@joekane.org?subject=Switchboard%20beta%20access">Request beta access</a>
</p>

<p align="center">
  <img alt="Closed beta" src="https://img.shields.io/badge/status-closed%20beta-D6A42A" />
  <img alt="Private add-on" src="https://img.shields.io/badge/private-add--on-24C9A6" />
  <img alt="Part of Nexus" src="https://img.shields.io/badge/part%20of-Nexus-3A9BF0" />
</p>

<p align="center">
  <img src="https://nexus.joekane.org/assets/shots/switchboard-trace.png" alt="The Switchboard console — engineers with their specialisms and load bars beside the unassigned queue, each ticket routed to a named engineer with the reason shown." width="820" />
</p>

---

## What is Switchboard?

Switchboard reads your **unassigned queue** and gets each ticket to the right person — matched by **specialism**, **who's actually free** (from your help desk's live agent presence) and **current load**. It recommends, or — when you're ready — assigns automatically, writing the result straight back to your help desk.

It runs on the help desk Nexus is already connected to — Zendesk, Freshdesk, Freshservice, Jira Service Management or HaloPSA — so there's nothing new to plug in. And it's **deterministic and explainable**: every decision comes with a plain-English trace of why this engineer, this time.

- 🎯 **Right person, not nearest person** — specialism first, then live availability, then load.
- 🔍 **Explainable by default** — a plain-English trace behind every routing decision.
- 🛡️ **Safe to switch on** — manual by default, with a dry run and rails before anything writes back.

> **Closed beta · private add-on.** Switchboard stays hidden in Nexus unless your licence key carries the entitlement — there's no upsell, just nothing, until you're in the beta. And even then it's **manual by default** and honest about being early: turn on automatic only once you've watched it get the calls right.

## How it decides

| | |
|---|---|
| **1 · Classify** | Read the ticket — subject *and* body, with quoted history and signatures stripped — and tag its area (POS, M365, network, access, on-site…) plus a P1/P2/P3 priority. |
| **2 · Match specialism** | Find the engineers whose primary skill is that area, then their secondary specialists — the right person before the nearest person. |
| **3 · Check availability** | Cross-reference live agent presence: online beats away; on-site and at-capacity engineers sit out. |
| **4 · Balance the load** | Among equally-good options the least-loaded wins, with a fairness rotation — or it **holds** for the team when nobody's free. |

## Recommend, or just do it

Three modes — **off**, **manual** (it recommends, you click Assign) and **automatic** (it writes the assignment straight back to your help desk). Start with a **dry run** that records exactly what it *would* have done — no writes — so you can trust it before you let it loose.

<p align="center">
  <img src="https://nexus.joekane.org/assets/shots/switchboard-routing.png" alt="The Routing tab — an Off / Manual / Automatic control with the safety rails: dry run, business-hours only, online-only, a per-minute cap and area exclusions." width="760" />
</p>

- **Real-load capacity** — caps each engineer by their actual open tickets, not a guess.
- **Your rails** — business-hours only, online-only, a per-minute cap, hold your P1s, exclude whole areas.
- **A full audit trail** — every automatic assignment (and every dry-run preview) logged with its reason.
- **Optional AI** for the tickets keywords can't call — your provider, your key, with the built-in engine always as the fallback.

## Learns your team

Not sure who's best at what? Switchboard reads each engineer's recently-**solved** tickets and proposes their specialisms — with the evidence in plain English. You review and apply; it never overwrites what you've set by hand.

<p align="center">
  <img src="https://nexus.joekane.org/assets/shots/switchboard-learn.png" alt="The specialism-learning review — each engineer with the specialisms inferred from their solved history and a one-line rationale to accept or edit." width="760" />
</p>

## AI for the hard ones

When the keyword classifier is **unsure**, Switchboard can ask the AI provider *you* configure (Anthropic or OpenAI, your own key) to pick the engineer — only for those uncertain tickets, and only from the eligible team. The deterministic engine is always the fallback, so AI never blocks a routing.

## On the wall, live

Switchboard isn't just a console — it's a **board panel**, too. A live feed streams every incoming ticket and the engineer it's headed to, with engineer load bars, tap-a-row for the trace, one-tap assign, and a little celebration when the queue hits zero.

<p align="center">
  <img src="https://nexus.joekane.org/assets/shots/switchboard-panel.webp" alt="The Switchboard live-feed panel on the wallboard." width="760" />
</p>

## Write-back support by help desk

Routing works on **every** help desk Nexus connects to (it only needs live presence + the unassigned queue). Applying an assignment — the write-back — depends on the provider:

| Help desk | Recommend | Assign (write-back) |
|---|:---:|:---:|
| Zendesk | ✅ | ✅ |
| Freshdesk | ✅ | ✅ |
| Freshservice | ✅ | ✅ |
| HaloPSA | ✅ | ✅ |
| Jira Service Management | ✅ | — *(advisory-only in this beta)* |

## Get in

Switchboard is part of **[Nexus](https://nexus.joekane.org)** — a private add-on unlocked per-licence, in closed beta while we tune it against real teams. Want a look? Tell us about your team:

→ **[Request beta access](mailto:joe@joekane.org?subject=Switchboard%20beta%20access)** · or read the [overview](https://nexus.joekane.org/switchboard).

---

<p align="center">
  <a href="https://nexus.joekane.org/switchboard">nexus.joekane.org/switchboard</a> · Built by <a href="https://joekane.org">Joe Kane</a><br/>
  <sub>© 2026 Joe Kane. A private add-on for Nexus, a proprietary product.</sub>
</p>
