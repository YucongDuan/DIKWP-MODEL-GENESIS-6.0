# DIKWP MODEL GENESIS 6.0

A runnable, evidence-bounded observatory for GPT-5.6 and other mainstream AI models.

## What it does

- Stores official vendor specifications as **D**, never as proof of cognition or universal performance.
- Generates **I** only from controlled comparisons of observed records.
- Forms local **K** only after repetition and held-out evidence.
- Produces **W** only for an explicit purpose and at least two empirically supported options.
- Issues a limited **P** with target, success criteria, stop conditions and scope.
- Keeps product tools, routing, prices, timestamps and URLs as engineering metadata rather than new semantic primitives.

## What it does not do

It does not infer hidden chain of thought, consciousness, values or intentions from model marketing. It does not publish a global best-model leaderboard. The bundled offline fixtures validate the software pipeline only; they do not simulate any vendor model.

## Quick start

```bash
python -m pip install -e .
model-genesis demo --out outputs/reference
model-genesis verify outputs/reference/model_genesis.sqlite
model-genesis serve --dir outputs/reference --port 8780
```

Open `http://127.0.0.1:8780/dashboard.html`.

## Run a real model

```bash
export OPENAI_API_KEY=...
model-genesis run \
  --db outputs/openai.sqlite \
  --model gpt-5.6-sol \
  --provider OpenAI \
  --api-style openai_responses \
  --api-key-env OPENAI_API_KEY \
  --repetitions 2
```

Equivalent adapters are included for Anthropic Messages, Gemini generateContent, and OpenAI-compatible chat APIs. API keys are read only from environment variables.

## Core files

- `configs/models_official_2026-07-28.json`: official model snapshot.
- `suites/mesh60_core_v1.json`: ten disclosed D/I/K/W/P probes.
- `purposes/*.json`: purpose-relative selection contracts.
- `outputs/reference/dashboard.html`: single-file offline observatory.

## Evidence boundary

A million-token context window is D about capacity; it is not K about stable long-context use. A tool list is D about the product surface; it is not proof that the base model independently possesses those capabilities. A vendor benchmark is D about a vendor-reported experiment; target-deployment K requires reruns in the target harness.
