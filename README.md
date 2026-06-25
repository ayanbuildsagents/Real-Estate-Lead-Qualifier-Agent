# 🏠 Real Estate Lead Qualifier Agent

> AI-powered WhatsApp agent that qualifies inbound real estate leads through natural conversation — filters time-wasters, books site visits, and alerts broker instantly.

## 🔥 What It Does

Lead messages on WhatsApp → Bilal (AI agent) qualifies through 4 questions → HOT lead detected → broker gets instant WhatsApp alert + Google Calendar site visit created. WARM lead → nurture message sent. Zero human effort.

## 🧠 How It Works

| Step | What Happens |
|------|-------------|
| 1 | Lead sends WhatsApp message from ad |
| 2 | Bilal AI collects: budget → area → timeline → purpose |
| 3 | HOT lead (budget confirmed + timeline 1-3 months) detected |
| 4 | Clean response sent to lead — status tags stripped |
| 5 | Broker gets instant WhatsApp alert with lead number |
| 6 | Google Calendar site visit appointment auto-created |
| 7 | WARM lead → nurture message sent, conversation closed softly |

## 🛠️ Built With

- **n8n** — workflow automation
- **OpenAI GPT-4o-mini** — AI conversation engine
- **WhatsApp API (Whapi.cloud)** — messaging
- **Google Calendar API** — site visit booking
- **Window Buffer Memory** — per-user conversation history

## 📋 Setup

1. Import `Real_Estate_Agent.json` into your n8n instance
2. Add credentials: OpenAI API, Whapi.cloud token, Google Calendar OAuth
3. Update webhook URL in your WhatsApp provider
4. Update broker WhatsApp number in the `Broker Alert` node
5. Activate workflow

## 💡 Key Features

- Speaks Roman Urdu, English, or Urdu script — mirrors user automatically
- Never reveals it's an AI
- Collects all 4 qualifiers before classifying lead
- HOT lead = instant broker alert + calendar event
- WARM lead = soft nurture message
- Legal queries flagged separately with `[LEGAL_QUERY_FLAGGED]`

## 📁 Files

| File | Description |
|------|-------------|
| `Real_Estate_Agent.json` | Complete n8n workflow — ready to import |
