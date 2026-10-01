# llm-lab#

## Purpose
Your LLM engineering lab. You build a RAG system and an agent system here and prove they work with evals. Evals are the point.

## Tracker tasks
Prompting and tool calling, embeddings, RAG, agent, eval harness, FastAPI, Docker and CI, deployment, README and write-up.

## Folder structure
```
llm-lab/
  notes/          lessons learned and design decisions
  01_prompting/   structured output and tool calling
  02_embeddings/
  rag/            RAG system
  agent/          agent system
  evals/          test sets and scoring scripts
  api/            FastAPI wrapper
  Dockerfile
  README.md       final project README
```

## Daily input
- 1 working piece of code (a prompt pattern, a retriever, a tool, an eval case)
- 5 new eval cases added to `evals/` (question, expected result, scoring rule)
- 1 note in `notes/`: what failed and why
- Commit message format: `component: what changed and effect on eval score`

Minimum on a bad day: add 3 eval cases and one note.

## Order
1. Prompting, structured output, tool calling
2. Embeddings and vector search
3. RAG with chunking and reranking
4. Agent with tools and memory
5. Eval harness covering both
6. FastAPI, Docker, CI, public deploy
7. Cost and latency notes, final write-up

## Done when
- RAG and agent each have measured eval results
- One system is deployed with README, evals and a design write-up

## Rules
- No change without an eval run before and after
- Log cost and latency from day one
- Keep every prompt in version control
