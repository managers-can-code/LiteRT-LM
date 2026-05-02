# LiteRT-LM

LiteRT-LM is Google's production-ready, high-performance, open-source inference
framework for deploying Large Language Models on edge devices.

🔗 [Product Website](https://ai.google.dev/edge/litert-lm)

## 🔥 What's New: Gemma 4 support with LiteRT-LM

Deploy [Gemma 4](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/)
across a broad range of hardware with stellar performance
([blog](https://developers.googleblog.com/bring-state-of-the-art-agentic-skills-to-the-edge-with-gemma-4/)).

👉 Try on Linux, macOS, Windows (WSL) or Raspberry Pi with the
[LiteRT-LM CLI](https://ai.google.dev/edge/litert-lm/cli):

```bash
litert-lm run  \
   --from-huggingface-repo=litert-community/gemma-4-E2B-it-litert-lm \
   gemma-4-E2B-it.litertlm \
   --prompt="What is the capital of France?"
```

## 🌟 Key Features

-   📱 **Cross-Platform Support**: Android, iOS, Web, Desktop, and IoT (e.g.
Raspberry Pi).
-   🚀 **Hardware Acceleration**: Peak performance via GPU and NPU accelerators.
-   👁️ **Multi-Modality**: Support for vision and audio inputs.
-   🔧 **Tool Use**: Function calling support for agentic workflows.
-   📚 **Broad Model Support**: Gemma, Llama, Phi-4, Qwen, and more.

![](./docs/api/kotlin/demo.gif)

---

## 🚀 Production-Ready for Google's Products

LiteRT-LM powers on-device GenAI experiences in **Chrome**, **Chromebook Plus**,
**Pixel Watch**, and more.

You can also try the
[Google AI Edge Gallery](https://github.com/google-ai-edge/gallery) app to run
models immediately on your device.

| **Install the app today from Google Play** | **Install the app today from App Store** |
| :---: | :---: |
| <a href='https://play.google.com/store/apps/details?id=com.google.ai.edge.gallery'><img alt='Get it on Google Play' height="120" src='https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png'/></a> | <a href="https://apps.apple.com/us/app/google-ai-edge-gallery/id6749645337?itscg=30200&itsct=apps_box_badge&mttnsubad=6749645337" style="display: inline-block;"> <img src="https://toolbox.marketingtools.apple.com/api/v2/badges/download-on-the-app-store/black/en-us?releaseDate=1771977600" alt="Download on the App Store" style="width: 246px; height: 90px; vertical-align: middle; object-fit: contain;" /></a> |

### 📰 Blogs & Announcements

| Link | Description |
| :--- | :--- |
| [Bring state-of-the-art agentic skills to the edge with Gemma 4](https://developers.googleblog.com/bring-state-of-the-art-agentic-skills-to-the-edge-with-gemma-4/) | Deploy Gemma 4 in-app and across a broader range of devices with stellar performance and broad reach using LiteRT-LM. |
| [On-device GenAI in Chrome, Chromebook Plus and Pixel Watch](https://developers.googleblog.com/on-device-genai-in-chrome-chromebook-plus-and-pixel-watch-with-litert-lm/) | Deploy language models on wearables and browser-based platforms using LiteRT-LM at scale. |
| [On-device Function Calling in Google AI Edge Gallery](https://developers.googleblog.com/on-device-function-calling-in-google-ai-edge-gallery/) | Explore how to fine-tune FunctionGemma and enable function calling capabilities powered by LiteRT-LM Tool Use APIs. |
| [Google AI Edge small language models, multimodality, and function calling](https://developers.googleblog.com/google-ai-edge-small-language-models-multimodality-rag-function-calling/) | Latest insights on RAG, multimodality, and function calling for edge language models. |

---

## 🏃 Quick Start

### 🔗 Key Links

-   👉 [Technical Overview](https://ai.google.dev/edge/litert-lm/overview) including performance benchmarks, model support, and more.
-   👉 [LiteRT-LM CLI Guide](https://ai.google.dev/edge/litert-lm/cli) including installation, getting started, and advanced usage.

### ⚡ Quick Try (No Code)

Try LiteRT-LM immediately from your terminal without writing a single line of code using [`uv`](https://docs.astral.sh/uv/getting-started/installation/):

```bash
uv tool install litert-lm

litert-lm run \
  --from-huggingface-repo=google/gemma-3n-E2B-it-litert-lm \
  gemma-3n-E2B-it-int4 \
  --prompt="What is the capital of France?"
```


---

### 📚 Supported Language APIs
Ready to get started? Explore our language-specific guides and setup instructions.

| Language | Status | Best For... | Documentation |
| :--- | :--- | :--- | :--- |
| **Kotlin** | ✅ Stable | Android apps & JVM | [Android (Kotlin) Guide](https://ai.google.dev/edge/litert-lm/android) |
| **Python** | ✅ Stable | Prototyping & Scripting | [Python Guide](https://ai.google.dev/edge/litert-lm/python) |
| **C++** | ✅ Stable | High-performance native | [C++ Guide](https://ai.google.dev/edge/litert-lm/cpp) |
| **Swift** | 🚀 In Dev | Native iOS & macOS | (Coming Soon) |

#### 🏗️ Build From Source

This [guide](./docs/getting-started/build-and-run.md) shows how you can
compile LiteRT-LM from source. If you want to build the program from source,
you should checkout the stable [![Latest
Release](https://img.shields.io/github/v/release/google-ai-edge/LiteRT-LM)](https://github.com/google-ai-edge/LiteRT-LM/releases/latest) tag.

---

## 📦 Releases

-   **v0.10.1**: Deploy [Gemma 4](https://blog.google/innovation-and-ai/technology/developers-tools/gemma-4/) with stellar performance ([blog](https://developers.googleblog.com/bring-state-of-the-art-agentic-skills-to-the-edge-with-gemma-4/)) and introduce [LiteRT-LM CLI](https://ai.google.dev/edge/litert-lm/cli).
-   **v0.9.0**: Improvements to function calling capabilities, better app performance stability.
-   **v0.8.0**: Desktop GPU support and Multi-Modality.
-   **v0.7.0**: NPU acceleration for Gemma models.

For a full list of releases, see [GitHub Releases](https://github.com/google-ai-edge/LiteRT-LM/releases).

---

<!-- BEGIN claude-code-integration -->
<!--
This file is the proposed addition to the LiteRT-LM repo's top-level README.md.
It is intended to be inserted under the existing "Tools" / "CLI" section, or
wherever the maintainers determine fits the narrative best. Agent C verifies
fit before the PR opens.
-->

## Use with Claude Code

LiteRT-LM's `serve` subcommand can expose an Anthropic Messages API surface, letting [Claude Code](https://docs.claude.com/en/docs/claude-code) talk to a locally-running model. There are two ways to wire them together — same server, different interaction patterns:

1. **Server proxy** (this README's quick start): `ANTHROPIC_BASE_URL=http://localhost:9379`. ALL Claude Code traffic goes to local model. Best for offline / privacy-required / max cost savings.
2. **Subagent delegation** (via the companion plugin): Cloud Claude stays primary and delegates routine tasks (doc strings, simple refactors, summaries) to a `litert-lm-local` subagent that runs on the user's machine. Best for keeping cloud-Claude quality on hard work while offloading routine work locally. Modeled on the [codex-plugin-cc](https://github.com/openai/codex-plugin-cc) pattern.

> **Companion docs, plugin, and reproduction kit.** Plain-English overview, design doc, risks-and-limitations, an optional Claude Code plugin that ships **both modes** (slash commands `/litert-lm-start`, the `litert-lm-local` inference subagent, the `litert-lm-debug` subagent, MCP server with `litert_lm_generate` tool), reproducible Tier 3 verification runner, validation reports, and a side-by-side **TESTING.md** for both modes — all live in the companion repo at [`managers-can-code/litert-lm-claude-code`](https://github.com/managers-can-code/litert-lm-claude-code). This `README.md` covers the minimal "server proxy" path; the companion repo covers everything else.

### Requirements

- LiteRT-LM ≥ `<release-with-this-PR>`
- A LiteRT-LM-compatible model (e.g., a `.litertlm` file from the [Models page](https://ai.google.dev/edge/litert-lm))
- [Claude Code CLI](https://docs.claude.com/en/docs/claude-code/install) ≥ 2.1.123
- Linux or macOS (Windows planned for v1.5)

### Quick start

Start the LiteRT-LM server in Anthropic-compatible mode:

```bash
litert-lm serve --api anthropic --model /path/to/your/model.litertlm
```

The server binds `localhost:9379` by default. In a separate shell, point Claude Code at it:

```bash
export ANTHROPIC_BASE_URL=http://localhost:9379
export ANTHROPIC_AUTH_TOKEN=any-value-server-ignores-it
claude --model your-model-id
```

That's it. `claude` now routes every request through your local LiteRT-LM model.

### What's supported

- `POST /v1/messages` — non-streaming and streaming (SSE) responses
- `POST /v1/messages/count_tokens` — coarse estimate (avoids the 404-cascade degradation pattern when clients pre-flight)
- `GET /v1/models` — currently loaded model list
- Anthropic `tool_use` / `tool_result` content blocks for tool-capable models
- Incremental tool-call argument streaming (avoids the 255-second Claude Code timeout that buffered tool-call arguments would otherwise trigger)
- Periodic `ping` events during long generations

### Server flags

| Flag | Default | Purpose |
|---|---|---|
| `--api` | `gemini` | Set to `anthropic` for Claude Code |
| `--model` | required | Path to a `.litertlm` model file |
| `--host` | `localhost` | Bind address. Use `0.0.0.0` only behind a reverse proxy |
| `--port` | `9379` | Bind port |
| `--max-request-bytes` | `4194304` (4 MiB) | Reject request bodies larger than this |
| `--request-timeout-secs` | `300` | Per-request wall-time cap |
| `--max-concurrent` | `4` | Maximum concurrent inferences (over-cap returns `overloaded_error`) |
| `--bearer-token` | unset | If set, require `Authorization: Bearer <this>` on every request |
| `--accept-any-model` | unset | Route any incoming model name to the loaded model (default: 404 unknown names) |
| `--verbose` | unset | Log request bodies + responses (use sparingly — never enable on a public host) |

### Recommended Claude Code flags

For one-shot scripted use:

```bash
claude -p "your task" --bare --output-format json --allowedTools "Read,Edit,Bash"
```

`--bare` skips local hooks/skills/plugins/MCP — it's the right setting for CI/CD.

### Performance notes

LiteRT-LM is built for on-device inference; expect first-token latency under 1.5 s on a typical Apple-silicon laptop with a small Gemma 3n variant. Long-context (>20 k tokens in) and long-output (>4 k tokens out) workloads are functional but not the optimization target — Claude on the cloud is much faster for those.

### Security

The default bind is `127.0.0.1` and there is no authentication. **Do not expose this server to a network without a reverse proxy that terminates TLS and enforces auth.** Use `--bearer-token` for a basic shared-secret check on a trusted LAN; production deployments should sit behind an authenticating reverse proxy.

### Known limitations (v1)

- Linux + macOS only. Windows in v1.5.
- Tool use requires the underlying model to natively support tool calling. Models without it will return `invalid_request_error` when given a non-empty `tools` array. Grammar-constrained tool emulation is planned for v1.5.
- Image content blocks are passed through to vision-capable models only. Non-vision models receive `invalid_request_error`.
- The `count_tokens` endpoint returns a heuristic estimate (1 token ≈ 4 chars), not an exact count. Real tokenization is planned for v1.5.

### Troubleshooting

**"Connection refused"** — server isn't running or is bound to a different port. Check `litert-lm serve --help` and your `--port` flag.

**"not_found_error: model … not found"** — the model name in your `claude --model` argument doesn't match the loaded model's id. Either pass `--model <loaded-id>` or start the server with `--accept-any-model` to route everything to the loaded one.

**"overloaded_error"** — the concurrency cap is full. Either wait, or raise `--max-concurrent`.

**Long generations time out around 4 minutes 15 seconds** — this is a known Claude Code behavior when SSE has no traffic. The server emits `ping` events every 10 s during long generations to mitigate; if you still hit it, reduce `max_tokens` or split the task.

### Where to look next

- **Plain-English overview** for sharing with teammates: [`docs/OVERVIEW.md` in the companion repo](https://github.com/managers-can-code/litert-lm-claude-code/blob/main/docs/OVERVIEW.md)
- **Risks, limitations, and protocol-drift mitigations**: [`docs/RISKS.md`](https://github.com/managers-can-code/litert-lm-claude-code/blob/main/docs/RISKS.md)
- **Formal design document** (problem, architecture, trade-offs, decision log): [`docs/PRD.md`](https://github.com/managers-can-code/litert-lm-claude-code/blob/main/docs/PRD.md)
- **Optional Claude Code plugin** for zero-config setup (slash commands, MCP server, debug subagent): [`plugin/litert-lm/`](https://github.com/managers-can-code/litert-lm-claude-code/tree/main/plugin/litert-lm)
- **Tier 3 reproduction runner** — drives a real Claude Code session against your real `litert_lm.Engine` and writes a transcript: [`tier3-runner/`](https://github.com/managers-can-code/litert-lm-claude-code/tree/main/tier3-runner)
- **Validation reports** — the empirical evidence this integration works end-to-end: [`reports/`](https://github.com/managers-can-code/litert-lm-claude-code/tree/main/reports)
<!-- END claude-code-integration -->
