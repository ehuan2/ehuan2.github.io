---
layout: page
title: VLM-Lens
description: 
img: assets/img/publication_preview/vlm-lens.png
importance: 2
category: nlp
---

VLM-Lens is a toolkit designed to enable systematic benchmarking, analysis, and interpretation of vision-language models (VLMs) by supporting the extraction of intermediate outputs from any layer during the forward pass of open-source VLMs. This allows users to quickly iterate on explainable AI experiments, where they can probe the different embeddings produced at different layers of a VLM quickly and effectively.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/vlm-lens.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example use-case of VLM-Lens, where users can probe any open-source model (e.g.: Qwen-VL) by their layer names (model.layers.14_post_attention_layernorm) for further analysis.
</div>

I was in charge of the preliminary design and implementation of VLM-Lens, opting for a Yaml configuration file which could specify the models, which layers' embedding to probe, and the prompts. I ensured extensibility through the use of carefully designed model classes, while saving it all out to a Sqlite database for further analysis.

This led to an acceptance to the Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing: System Demonstrations held in Suzhou, China. See the Github here: <a href="https://github.com/compling-wat/vlm-lens"> https://github.com/compling-wat/vlm-lens </a> and the paper here: <a href="https://arxiv.org/abs/2510.02292"> https://arxiv.org/abs/2510.02292 </a>.
