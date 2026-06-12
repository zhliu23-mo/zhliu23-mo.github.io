---
title: "NanoGPT Preference Alignment (DPO) for Arithmetic Tasks"
collection: portfolio
order: 1
timeline: "Oct. 2025 - Nov. 2025"
role: "Core Developer, Course Project"
excerpt: "A two-stage SFT + DPO pipeline that aligns NanoGPT for arithmetic and one-variable algebra reasoning."
project_image: "/images/portfolio/dpo-terminal.svg"
image_alt: "Terminal-style preview of NanoGPT DPO training logs"
tags:
  - DPO
  - NanoGPT
  - Preference Alignment
  - Arithmetic Reasoning
terminal_preview: true
---

This course project explored whether a compact GPT-style model can be preference-aligned to solve arithmetic and one-variable algebra tasks more reliably.

<div class="terminal-mini" aria-label="DPO training output log">
  <div class="terminal-mini__bar">nanogpt-dpo-arithmetic — training.log</div>
  <div class="terminal-mini__content"><span class="terminal-green">$ python train_dpo.py --model nanogpt --task algebra --beta 0.1</span>
[data] loaded 100,000+ preference pairs
[sft ] warm-start checkpoint: ckpt_sft_iter_20000.pt
<span class="terminal-blue">[dpo ] iter 004000 | loss 0.412 | chosen_logp ↑ | rejected_logp ↓</span>
<span class="terminal-blue">[eval] arithmetic accuracy: 91.7% | one-variable algebra: 90.4%</span>
[case] solve: 3x + 7 = 22
       reasoning: subtract 7 → 3x = 15 → x = 5
<span class="terminal-green">       answer: x = 5 ✓</span>
<span class="terminal-orange">[base] accuracy ≈ 0% → [aligned] accuracy &gt; 90%</span></div>
</div>

## Highlights

* Built a two-stage fine-tuning workflow: supervised fine-tuning followed by Direct Preference Optimization.
* Constructed more than 100,000 preference pairs by pairing explicit-reasoning positive samples with negative generations from the base model.
* Tuned preference weights and hyperparameters in a CUDA environment.
* Achieved over 90% accuracy on arithmetic and one-variable algebra tasks, substantially improving over the base model.
