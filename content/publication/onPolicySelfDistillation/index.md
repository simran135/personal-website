---
title: "Rethinking On-Policy Self-Distillation for Thinking Models"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Narutatsu Ri
- Yinghui He
- Liam Fowl
- Sanjeev Arora

# Author notes (optional)

date: "2026-07-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).


# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent

# Publication name and optional abbreviated publication name.
publication: FoGen Workshop at ICML 2026
publication_short: FoGen Workshop at ICML 2026

abstract: "Self-distillation is a promising recipe for self-improvement in language models. In this setting, a model can serve as its own teacher when given privileged information, such as a solution to a math problem. This seems especially appealing for thinking models, which can use test-time reasoning to absorb the privileged information. Surprisingly, we show that privileged self-distillation degrades thinking models on long reasoning traces: across five Qwen3 and OLMo thinking models evaluated on AIME24, AIME25, and HMMT25, privileged-context distillation causes a relative drop of up to 17% in avg@16 accuracy. The degradation scales with the amount of privileged context withheld from the student and is most pronounced at long rollout budgets, where thinking models otherwise obtain their largest gains. This failure mode is not specific to self-distillation: on-policy distillation (OPD) improves thinking models, but privileged OPD reverses these gains. Our diagnostics link this failure mode to how privileged teacher context reshapes learning at high-entropy forking positions, where multiple continuations remain plausible and may lead to different reasoning paths. Privileged context lowers fork rates in thinking-model rollouts but not in instruction-model rollouts. This leads to an interesting dichotomy, where privileged context can help instruction-tuned models but hurts stronger thinking models. The effect is visible when the student begins a self-correction branch, where privileged OPD penalizes sampled reconsideration tokens that vanilla OPD supports. Thinking models trained with a privileged teacher produce fewer verification, backtracking, and hedging markers, even after length normalization. These findings indicate that self-distillation for strong thinking models requires attention to token-level signal, especially around correction and reasoning steps."

# Summary. An optional shortened abstract.
summary: ' '

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: arXiv
   url: https://arxiv.org/abs/2607.05184

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
---
