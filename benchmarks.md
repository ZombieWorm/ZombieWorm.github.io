---
layout: default
title: Benchmarks
permalink: /benchmarks/
---

# GPU Performance Benchmarks

{% include benchmark-card.html title="RTX 5080 Usage" slug="5080-feedback" content="<p>Benchmark results showing AWQ quantization performance on RTX 5080 with VRAM usage and token throughput metrics.</p><ul><li>FP16: 18.2 tokens/s, ~84GB VRAM</li><li>AWQ-4bit: 41.7 tokens/s, ~38GB VRAM (52% savings)</li></ul>" %}

__________________
QWEN3.5
Summary| Very capable model perfect for larger tasks and small projects
Tool| llamaCPP
prompt speed|
t/s|
VRAM usage| 99% max
from| unsloth
type| 9B GGUF
__________________
Nemotron3 Nano
Summary| Blazing fast - pefect for rapid chats and time priority
Tool| llamaCPP
prompt speed| 941 // 7050 // 1061
t/s| 196 // 204
VRAM usage| 99% max
from| nvidia
type| 4B GGUF
___________________


