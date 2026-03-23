# HistoRAG: Designing a Methodologically Informed Retrieval-Augmented Generation System for Historical Research

**Journal of Digital History** submission repository

## Authors

- Noah J. Kim-Baumann [![ORCID](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0009-0004-6368-3061), Humboldt-Universität zu Berlin
- Torsten Hiltmann [![ORCID](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6757-6210), Humboldt-Universität zu Berlin

## Abstract

This article presents HistoRAG, a Retrieval-Augmented Generation framework designed for historical research. Through a case study analysing *Der Spiegel* (1950–1979) and the computerisation discourse of the early Federal Republic, we demonstrate three methodological interventions — separated retrieval and generation, temporal windowing, and LLM-as-judge evaluation — that embed historiographical principles into system architecture. The framework preserves source traceability and interpretive authority while enabling historians to work with large corpora at scale.

## Repository Structure

- `article.ipynb` — The article notebook (narrative, hermeneutic, and data layers)
- `media/` — Images and figures used in the article
- `script/` — Supporting data and analysis scripts
- `corpus_data/` — Corpus data (yearly CSV files from *Der Spiegel*)
- `requirements.txt` — Python dependencies
- `runtime.txt` — Python runtime version specification
- `.github/workflows/` — JDH preflight validation action

## Running the Notebook

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/noahjb27/spiegelragged_jdh/main?filepath=article.ipynb)

```bash
pip install -r requirements.txt
jupyter notebook article.ipynb
```

## Preflight Validation

The repository includes a GitHub Actions workflow that validates the notebook against JDH submission guidelines. Trigger it manually from the Actions tab or it runs on push.

## License

This article is published under the [Creative Commons Attribution License (CC-BY)](https://creativecommons.org/licenses/by/4.0/).
