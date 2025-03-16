---
title: "Instruct-SkillMix: A Powerful Pipeline for LLM Instruction Tuning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Simon Park
- Anirudh Goyal
- Sanjeev Arora

# Author notes (optional)

date: "2025-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).


# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent

# Publication name and optional abbreviated publication name.
publication: ICLR, 2025 & \[Oral\] Compositional Learning Workshop at NeurIPS 2024
publication_short: ICLR 2025. \[Oral\] Compositional Learning Workshop at NeurIPS 2024

abstract: We introduce Instruct-SkillMix, an automated approach for creating diverse, high quality SFT data. The Instruct-SkillMix pipeline involves two stages, each leveraging an existing powerful LLM (1) Skill extraction, which uses the LLM to extract core "skills" for instruction-following, either from existing datasets, or by directly prompting the model; (2) Data generation, which uses the powerful LLM to generate (instruction, response) data that exhibit a randomly chosen pair of these skills. Here, the use of random skill combinations promotes diversity and difficulty. Vanilla SFT (i.e., no PPO, DPO, or RL methods) on data generated from Instruct-SkillMix leads to strong gains on instruction following benchmarks such as AlpacaEval 2.0, MT-Bench, and WildBench. With just 4K examples, LLaMA-3-8B-Base achieves 42.76% length-controlled win rate on AlpacaEval 2.0. To our knowledge, this achieves state-of-the-art performance among all models that have only undergone SFT (no RL methods) and competes with proprietary models such as Claude 3 Opus and LLaMA-3.1-405B-Instruct. Ablation studies also suggest plausible reasons for why creating open instruction-tuning datasets via naive crowd-sourcing has proved difficult. Introducing low quality answers ("shirkers") in 20% of Instruct-SkillMix examples causes performance to plummet, sometimes catastrophically. The Instruct-SkillMix pipeline is flexible and is adaptable to other settings.

# Summary. An optional shortened abstract.
summary: ' '

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
links:
 - name: pdf
   url: https://arxiv.org/abs/2408.14774

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
