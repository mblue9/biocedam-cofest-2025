# Improving how we describe and discover Bioinformatics tools 

**Project for ISMB/ECCB 2025 CollaborationFest**

**Co-Leads:**

*(Core expertise for this project in bold)*

- [Maria Doyle](https://github.com/mblue9/) (**Bioconductor**, University of Limerick 🇮🇪)
- [Sebastian Lobentanzer](https://github.com/slobentanzer) (**LLMs/MCPs**, Helmholtz Munich 🇩🇪)

**Core Participants**

*(Contributing expertise and guidance)*

- [Hervé Ménager](https://github.com/hmenager) (**EDAM/bio.tools**, Institut Pasteur and Institut Français de Bioinformatique 🇫🇷)

**Remote Support**:

- [Claire Rioualen](https://github.com/rioualen/) (**EDAM/bio.tools**, Institut Français de Bioinformatique 🇫🇷)
- [Vince Carey](https://github.com/vjcitn) (**Bioconductor**, Harvard Medical School 🇺🇸)
- [Lori Shepherd](https://github.com/lshep) (**Bioconductor**, Roswell Park Comprehensive Cancer Center 🇺🇸) 

**Join us (during or after CoFest):**

[Bioconductor Zulip](https://chat.bioconductor.org) channel #edam-collaboration

## Overview
Finding the right bioinformatics software can be tricky. [Bioconductor alone has over 3,000 R packages](https://bioconductor.org/packages/release/BiocViews.html#___Software), each with its own focus, but describing them in a way that’s consistent and searchable is a challenge.

One approach we’re exploring is [**biocEDAM**](https://github.com/vjcitn/biocEDAM), an experimental R package (in active development on GitHub) that already works with OpenAI’s GPT‑4o to extract and suggest [EDAM ontology](https://edamontology.org/) terms for Bioconductor packages. These tags improve discoverability and interoperability across the ecosystem.

However, using OpenAI requires an API key and billing setup, which can be a barrier. At CoFest we want to build on this foundation by adding [**Gemini's free tier**](https://dev.to/garciadiazjaime/gemini-api-the-free-tier-that-makes-developers-happy-28nk) (via [Ellmer](https://ellmer.tidyverse.org/)) as an additional backend, offering a no‑cost, key‑free option that makes the tool easier for anyone to try. We’ll also refine prompts and test it on more packages.

We’re also keen to explore future approaches, such as how [**Model Context Protocols (MCPs)**](https://modelcontextprotocol.io/introduction) might help LLMs access package metadata, and to hear from domain specialists on which terms best describe tools in their fields.  

While our current tooling uses EDAM, we know EDAM alone doesn’t cover everything, input from people experienced in combining ontologies (like Wikidata or domain vocabularies) would be very welcome.

## Goals

**Core Goals (2‑day focus)**

- Explore adding Gemini backend support to `biocEDAM`
- Test `biocEDAM` on additional Bioconductor packages
- Collect feedback on EDAM term coverage and prompt quality
- Discuss how MCPs could support ontology‑aware metadata

**Stretch Goals (if time allows)**

- Abstract the LLM interface to support multiple providers
- Outline a follow‑up community blog post to share CoFest outcomes
- Sketch how MCP integration might look in future tooling

## Participants

**All welcome! You might be:**

- An R developer interested in tooling
- An ontology or metadata expert
- An LLM/NLP practitioner curious about applied use cases
- A Bioconductor package developer or user
- A domain expert with ideas on how your field’s software should be described

## Getting Started (Beginner-Friendly)
We welcome contributors of all experience levels — including beginners!

If you're new to ontologies, R, or LLMs, here are a few simple ways to contribute:

- Try running biocEDAM on a Bioconductor package (we can help you pick one!)
- Review the EDAM terms it suggests - do they make sense?
- Suggest improvements to the prompts or tag mappings
- Join discussions on how software in your field should be described
- We’ll be on-site (Maria & Sebastian) and happy to guide you through setup or answer questions. Just drop by!

## Input
- [Google doc here](https://docs.google.com/document/d/1wc6Gt0zsrNWJkL13Fp3GvMOtoj2rDxCBgFnqbLnhuxU/edit?usp=sharing). Feel free to add your name if you're interested in this project, and to start connecting with others. You're also welcome to add any questions or comments.

## Links
- [biocEDAM on GitHub](https://github.com/vjcitn/biocEDAM)
- [BioHackathon 2024 Preprint](https://osf.io/preprints/biohackrxiv/dsgnw_v1)
- [Background blog post on EDAM tagging](https://vjcitn.github.io/vjcblog/posts/2025-05-09-edam/)

## Further Reading
- For broader context on Bioconductor’s direction and engineering practices:  
**Bioconductor: Planning a third decade of comprehensive support for genomic data science**  
V.J. Carey, *Patterns*, 11 July 2025  
[https://doi.org/10.1016/j.patter.2025.101319](https://doi.org/10.1016/j.patter.2025.101319)
