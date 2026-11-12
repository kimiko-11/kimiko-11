---
layout: kc-page
title: "Research"
permalink: /research/
description: "Research by Kimaya Chavan — confidence-aware perception, distribution shift and computer vision."
redirect_from:
  - /publications/
---

<div class="kc-page">
<div class="kc-container">

<header class="kc-page__header">
<p class="kc-page__eyebrow">Research &amp; artifacts</p>
<h1 class="kc-page__title">Research</h1>
<p class="kc-page__intro">Research projects, experiments and technical artifacts.</p>
</header>

<div class="kc-list">

<article class="kc-item">
<p class="kc-item__meta">In progress</p>
<h2>Confidence-Aware Perception Under Distribution Shift</h2>
<p>Exploring how perception systems can estimate when their predictions become unreliable when the data they encounter differs from their training environment.</p>
<ul class="kc-tags">
<li>Computer Vision</li><li>Deep Learning</li><li>Perception</li><li>Robustness</li><li>Physical AI</li>
</ul>
</article>

<article class="kc-item">
<p class="kc-item__meta">Fellowship proposal</p>
<h2>Risk-Adaptive Deepfake &amp; Synthetic Identity Detection for KYC Systems</h2>
<p>A proposal for the TIH–IoT CHANAKYA Fellowship to build a KYC fraud detection system that does not rely on a single deepfake classifier. It layers cryptographic freshness checks, behavioural interaction integrity, identity continuity across sessions, audio-visual consistency analysis and conditional physiological signals, with each layer adding independent risk evidence to one explainable score. A frequency-residual preprocessing module exposes high-frequency artifacts that RGB-based models miss, and costlier checks run only when risk stays ambiguous, keeping latency low for mobile-first banking and fintech onboarding.</p>
<ul class="kc-tags">
<li>Deepfake Detection</li><li>KYC</li><li>Synthetic Identity</li><li>Explainable AI</li><li>Frequency Analysis</li><li>FinTech</li>
</ul>
</article>

<article class="kc-item">
<p class="kc-item__meta">Artifact</p>
<h2><a href="https://github.com/kimiko-11/IPD-Acidtrace" target="_blank" rel="noopener noreferrer">AcidTrace</a></h2>
<p>A blockchain-based traceability system for the acid supply chain. Every transfer from source to end user is recorded as a block linked by SHA-256 hashes to the previous transfer, so the full movement of a batch can be followed end to end. A balance check flags an anomaly whenever acid is unaccounted for, and a Flask API, role-specific web dashboards and a chain explorer make the records visible to the people in the chain.</p>
<ul class="kc-tags">
<li>Blockchain</li><li>Supply Chain</li><li>Traceability</li><li>Anomaly Detection</li><li>Flask</li><li>Next.js</li>
</ul>
</article>

<article class="kc-item">
<p class="kc-item__meta">Earlier work</p>
<h2><a href="https://github.com/kimiko-11/OCR-Based-Document-Understanding-System" target="_blank" rel="noopener noreferrer">OCR &amp; Document Understanding</a></h2>
<p>DocExtract-Bench, a reproducible framework that compares rule-based, zero-shot LLM (Llama 3.2, 1B) and hybrid extraction on 626 SROIE receipts, all fed by the same Tesseract 5 OCR output. The central finding is methodological: under exact-match scoring the LLM looks clearly better (macro F1 0.512 vs. 0.418), but under an OCR-noise-tolerant edit-distance criterion the rule-based extractor edges ahead (0.612 vs. 0.602) while running about 39,000 times faster. The LLM's robust advantage is limited to company names. A separate ablation also found that classical preprocessing degraded Tesseract 5 accuracy on clean scans by 26% relative CER.</p>
<ul class="kc-tags">
<li>Document AI</li><li>OCR</li><li>Information Extraction</li><li>LLM Evaluation</li><li>Tesseract</li>
</ul>
</article>

</div>

</div>
</div>
