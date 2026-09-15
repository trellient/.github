# Trellient

**AI agents that do the work, on WhatsApp.**

Most businesses in India already talk to their customers on WhatsApp. They answer the same questions every
day, miss messages after closing time, and lose orders to a reply that came an hour too late.

Trellient puts an AI agent on that number. It answers from the business's own documents, in the customer's
language. It checks orders, stock and appointments in the systems the business already uses. And when it needs
to do something that matters — a refund, an exchange, a booking — it asks the owner first, on WhatsApp.

---

## What makes it different

Answering questions is not the hard part, and it is not where the value is. Meta's own free Business AI covers
FAQ bots. The three things that are genuinely hard:

**It takes actions, not just messages.** Through the business's own systems, the agent looks things up and
changes them — order status, stock, slots, returns. Not a decision tree with a chat skin.

**The owner stays in control.** Every action has a setting: run it, ask me first, or never. Anything that
changes data or moves money waits for an Approve or Reject on the owner's phone, with a plain-English summary
of what is about to happen. Every change is logged with who made it.

**It knows what WhatsApp actually allows.** WhatsApp only lets a business send a normal message within 24
hours of the customer's last one. Trellient's agents know this: they will not promise an update they cannot
deliver, and a follow-up that falls outside the window is handed to a person instead of quietly dropped.

---

## How it is built

Agents are **configuration, not code**. Each one starts from a reviewed template — its instructions, its
tools, and a setup form — and is filled in per business. A new client is set up in the admin panel, not in a
new codebase. New capabilities are written once and every client gets them.

| | |
|---|---|
| **Channel** | WhatsApp Cloud API, with one-click connection and coexistence with the WhatsApp Business app |
| **Agents** | Versioned YAML templates; business verbs bound per client to their own systems |
| **AI** | Bring your own key — Anthropic, OpenAI, Google, Groq, Mistral and others, or Trellient's |
| **Integrations** | MCP servers and HTTP endpoints, with per-tool approval policies |
| **Knowledge** | Hybrid retrieval over the business's own documents, built for Hinglish and short queries |
| **Stack** | Java 21 · Spring Boot · PostgreSQL · Next.js · TypeScript |

---

## Status

In pilot. The platform is built and tested; we are working with our first businesses now.

If you run an SMB that lives on WhatsApp and this sounds like your problem, we would like to hear from you.

**[trellient.tech](https://trellient.tech)** · [hello@trellient.tech](mailto:hello@trellient.tech)
