# Tri-Core LLM Engine (Factual + Functional + Explorative)

A modular cognitive engine where:
1) **Factual Core** stores verified knowledge (truth).
2) **Functional Core** stores deterministic procedures/tools.
3) **Explorative Core** uses a local LLM only for unknowns.

LLM is **not** the source of truth.
LLM is an **exploration/search component**.

## Why
Most AI apps today are wrappers around LLM APIs.
They mix facts, procedures, and guesses => hallucination + cost + fragility.

This project separates them:
- Facts are retrieved, not hallucinated.
- Functions are executed, not guessed.
- LLM explores unknowns, then gets validated.

## Status
Progress: **0%** (bootstrapping).

## Quickstart (dev)
```bash
go mod tidy
go run ./cmd/engine
