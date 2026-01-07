---
layout: page
title: TF Binding
description: 
img: assets/img/publication_preview/tf_binding.png
importance: 2
category: bioinformatics
---
For my graduate course, COMP 561, introduction to bioinformatics, we had a final project where we were tasked with trying to predict the binding sites of transcription factors based on open chromatin region data (ChIP-seq), using physical features to improve prediction. For my project, we created an extensible framework that can test many different Machine Learning models (both classical and deep learning-based), enabling users to compare which architecture works best at predicting transcription factors. We concluded that this classification task remains difficult if motif scores are overlapping (i.e. high motif scores), and likely requires sequence data as well.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/publication_preview/tf_binding.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    CNN model architecture used in TF binding project.
</div>

More details are available in my report, found here:
<iframe src="/assets/pdf/tf_binding.pdf" width="100%" height="600px" style="border: none;" title="TF Binding">
    <!-- Fallback content for very old browsers or iframes are unsupported -->
    Your browser does not support iframes. <a href="/assets/pdf/tf_binding.pdf">Download the PDF</a>.
</iframe>
and my GitHub found: <a href="https://github.com/ehuan2/tf-binding">https://github.com/ehuan2/tf-binding</a>.
