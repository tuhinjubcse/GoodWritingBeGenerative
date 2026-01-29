This repository accompanies the study “Can Good Writing Be Generative? Expert-Level AI Writing Emerges through Fine-Tuning on High Quality Books” appeared at ACM CHI 2026. The project investigates whether large language models (LLMs) can convincingly mimic the style of celebrated authors and be preferred over expert human writers.


## Repository Structure

| Directory/File      | Description                                                                                                                                           |
|---------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
| `Writing_Prompts/`  | 50 text files, each named after an author (e.g., `Alice_Munro.txt`). Each file contains 20 excerpts by that author, a description of their style, and a content specification for new writing. |
| `data/`             | Anonymized JSON files grouped by evaluation type (quality vs. style), AI condition (few‑shot vs. fine‑tuned) and judge type (expert vs. lay). Each record includes the pair of excerpts, metadata, the judge’s preference and rationale. |
---

## Using the Data and Prompts

- **Writing prompts:** Use the files under `Writing_Prompts/` to examine or replicate author‑style mimicry. Each file provides 20 original passages and a description of the author’s voice. When prompting language models, include the content specification, examples and desired length.

- **Evaluation data:** The JSON files in `data/` can be used for modelling style transfer or testing AI/human discrimination. Each entry stores the two excerpts, metadata indicating which is human vs. AI, and the judge’s decision. Use these datasets only for non‑commercial, research purposes since some passages are copyrighted.


If you use this repository or the accompanying data, please cite the papers:

```
        @misc{chakrabarty_ginsburg_dhillon_2025,
          author       = {Chakrabarty, Tuhin and Ginsburg, Jane C. and Dhillon, Paramveer},
          title        = {Readers Prefer Outputs of AI Trained on Copyrighted Books over Expert Human Writers},
          year         = {2025},
          note         = {Manuscript in preparation},
          }

        @misc{chakrabarty2026goodwritinggenerativeexpertlevel,
            title={Can Good Writing Be Generative? Expert-Level AI Writing Emerges through Fine-Tuning on High-Quality Books}, 
            author={Tuhin Chakrabarty and Paramveer S. Dhillon},
            year={2026},
            eprint={2601.18353},
            archivePrefix={arXiv},
            primaryClass={cs.AI},
            url={https://arxiv.org/abs/2601.18353}, 
}

          

