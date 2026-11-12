# Lee Juwon

I build **LLM systems and developer tools** with an emphasis on reproducible
experiments, measurable performance, and clear engineering trade-offs.

Computer Science & Engineering at Ewha Womans University.

## Featured work

### [Phase-Aware Offloading for Single-GPU VERL Training](https://github.com/2Ju1/verl-phase-aware-offloading)

Extended `verl` with phase-aware model residency, CPU AdamW, and bounded
asynchronous gradient streaming for memory-efficient full-parameter GRPO.

- Reduced the Actor-backward peak by **27.9%** and end-to-end step time by
  **12.1%** with a 16 MiB streaming pipeline.
- Enabled Qwen2.5-1.5B training on a GPU with 11.90 GiB usable capacity where
  all-GPU and CPU-Adam-without-streaming configurations reached OOM.
- Preserved experiment configurations, raw evidence, failure cases, and known
  limitations for reproducibility.

### [Agentic LLM Latency Benchmark](https://github.com/2Ju1/agentic-llm-latency-benchmark)

Built a reproducible benchmark that separates the effects of context growth,
prefix stability, output length, and tool latency on LLM response time.

- Measured TTFT growth from **0.084 s to 0.458 s** as controlled context grew
  from 90 to 24,717 prompt tokens.
- Combined client-side latency with vLLM Prometheus metrics to distinguish KV
  recomputation, cache reuse, prefill, and decode costs.
- Added a versioned experiment spec, CLI, unit tests, and automated CI checks.

## Engineering interests

- LLM inference and training systems
- Developer tooling and reproducible evaluation
- Performance measurement and resource-efficient systems
- Interfaces that are understandable to both developers and LLMs

## Elsewhere

- [Technical notes and project write-ups](https://whoami-juwon.tistory.com/)

