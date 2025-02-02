# Journal AI

> An AI-powered journaling web app that uses LLMs to help you reflect, organize thoughts, and gain insights from your journal entries.

## Overview

Journal AI is a smart journaling platform built on top of [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui). It provides a conversational interface where you can write journal entries and have AI help you process your thoughts, identify patterns, and explore your emotions through natural dialogue.

### Features

- **Conversational journaling** — write entries through a chat-like interface
- **Multi-model support** — use OpenAI, Anthropic (Claude), Google (Gemini), Mistral, Perplexity, and more
- **Persistent storage** — entries stored in Supabase (PostgreSQL)
- **Prompt management** — save custom prompts for recurring reflection exercises
- **File & image support** — attach files and images to journal conversations
- **Workspaces** — organize journal entries into separate spaces
- **Responsive design** — works on desktop and mobile

## Tech Stack

- **Frontend**: Next.js, TypeScript, Tailwind CSS
- **Backend**: Supabase (Auth + PostgreSQL + Storage)
- **AI**: OpenAI, Anthropic, Google AI, Mistral, Perplexity APIs
- **Testing**: Jest

## Getting Started

### Prerequisites

- Node.js 18+
- Supabase CLI (`brew install supabase/tap/supabase`)

### Setup

```bash
git clone https://github.com/mMirmohammadi/journal-ai.git
cd journal-ai
npm install

# Start Supabase locally and generate types
supabase start
npm run db-types

# Start development server
npm run dev
```

Then visit `http://localhost:3000`.

### Environment Variables

Create a `.env.local` with your API keys:

```
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
OPENAI_API_KEY=...
ANTHROPIC_API_KEY=...
```

See the Supabase and provider documentation for full setup details.

## Acknowledgments

Built on [Chatbot UI](https://github.com/mckaywrigley/chatbot-ui) by Mckay Wrigley.
