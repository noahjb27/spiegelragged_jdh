# HistoRAG: Designing a Methodologically Informed Retrieval-Augmented Generation System for Historical Research — Demonstrated through a Case Study of Der Spiegel (1950–1979) and the Computerisation of the Early Federal Republic

**Journal of Digital History** submission repository

## Authors

- Noah J. Kim-Baumann [![ORCID](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0009-0004-6368-3061), Humboldt-Universität zu Berlin
- Torsten Hiltmann [![ORCID](https://orcid.org/sites/default/files/images/orcid_16x16.png)](https://orcid.org/0000-0002-6757-6210), Humboldt-Universität zu Berlin

## Abstract

This article introduces HistoRAG, a framework for redesigning Retrieval-Augmented Generation (RAG) to support historical research methodology. Standard RAG systems are built for factual question-answering, treating retrieval and generation as a seamless pipeline optimised for speed and accuracy. Historical scholarship, by contrast, demands source sovereignty, interpretive transparency, and temporal sensitivity, values that standard architectures not only fail to support but actively undermine. Drawing on Agre's Critical Technical Practice, we embed these disciplinary commitments into system architecture through three interventions: separated retrieval and generation, which restores the historian's heuristic phase of source evaluation before computational interpretation begins; temporal windowing, which counters the presentist bias of similarity-based retrieval by ensuring proportional representation across the research period; and LLM-as-a-Judge, which introduces transparent, contestable evaluation of source relevance against researcher-defined criteria. We demonstrate the framework through a case study analysing computerisation discourse in Der Spiegel (1950–1979), working with a corpus of 102,189 articles. Empirical evaluation shows that semantic retrieval combined with LLM evaluation surfaces relevant sources that keyword filtering misses, while the LLM-as-a-Judge component proves essential for managing the noise that broadened retrieval introduces. The generation phase produces what we term Zwischentexte (intermediate texts), these are not answers but interpretive proposals that historians can verify, contest, and develop. We argue that the central question for LLMs in digital humanities is not whether machines can "read" but how we design systems that make their interpretive interventions visible and contestable, preserving the scholar's epistemic agency throughout.

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
