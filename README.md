# ca_onlinedisc
### Conversation Analysis in Online Discussions: Insights for Chat Systems  
**Author:** Marina Pavlova 
---

## Overview  
This repository contains resources and analyses for the thesis project **Conversation Analysis in Online Discussions**.  
The project uses data from Reddit’s *Change My View (CMV)* community and includes pipelines for thread reconstruction, feature extraction, summarization, evaluation of moderation and dialogue patterns.  

---

Repo structure:
_(Not the tidiest, but...)_

- **`Reddit CMV` folder** contains raw and recompiled discussion data:  
  - **notebook** for reconstructing threads from four initial TSV files; 
  - **recompiled threads** as XML files organized into:  
    - `direct_deltas`  
    - `delta_threads`  
    - `deltaless_threads`  
  - **statistics files** with thread-level metrics (thread length, OP length, comments length). 
Does **not** contain 4 initial TSV files that can be found in [DHH24 repo](https://github.com/dhh2024/disc/tree/main):
 - `cmw_comments_sample_1_deltas_thread.tsv`
 - `cmw_comments_sample_1_only_delta_comments.tsv`
 - `cmw_comments_sample_1.tsv`
 - `cmw_submissions_sample_1.tsv`
   
- **`Full pipeline 97` folder** contains the main analysis pipeline applied to a curated dataset of 97 threads:  
- **`100_sample/`** – sample dataset of 97 XML threads used for analysis;
- **`consistency test/`** – notebooks testing consistency of Claude and ChatGPT outputs, evaluation results;
- **`97_all_NLP_features.ipynb`** – notebook for extracting NLP features;  
- **`97_Claude_summaries.ipynb`** – notebook for generating summaries and evaluating the need for moderator interventions; 
- **`97_all_features.xlsx`** – master spreadsheet combining extracted features, summaries, identified patterns;
- a number of **intermediate results** in CSV files;  
- **`pairwise_comparison.xlsx`** – results of pairwise comparisons and statistical tests.  
