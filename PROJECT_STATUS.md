# Project status

This is the standalone RelayGuard LLM gateway prototype. DecisionGraph integrates a copy of this code in its `relayguard/` directory at https://github.com/jainsujal720-jpg/decisiongraph-rag . The two copies must be synchronized when either changes.

The default mock provider demonstrates routing, fallback, budgets, rate limiting and audit behavior without generating a document-grounded answer. Configure `RELAYGUARD_PROVIDER_MODE=openai` and a server-side key for live OpenAI completions. Jev is optional and disabled in the integrated DecisionGraph configuration because provider access is pending.

This is a portfolio prototype; the local demo API keys in `.env.example` must be changed for shared use. Keep live keys in environment variables or a secrets manager and never commit `.env`. API model availability and cost depend on the provider account; cost estimates do not replace invoices.
