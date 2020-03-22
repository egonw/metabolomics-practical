# Metabolomics

[prev](./identification.md) | [toc](./README.md) | [next](pathways.md)


[MetaboLights](https://www.ebi.ac.uk/metabolights/) is a database
for metabolomics data hosted at the European Bioinformatics Institute.

ATP is a metabolite found in many biological processes. The compound
can be found in MetaboLights with the identifier
[MTBLC15422](https://www.ebi.ac.uk/metabolights/MTBLC15422). Under
the section `Biology` the studies are found, with identifiers starting
with the prefix `MTBLS`.

1. how many human studies found ATP? <button onclick="toggleAnswer('q1')">Answer</button><span id="q1" style="visibility: hidden">Fourteen, at the time of writing, with MTBLS87 being the oldest identifier.</span>
1. in how may other species has this metabolite be found? <button onclick="toggleAnswer('q2')">Answer</button><span id="q2" style="visibility: hidden">The page lists more than 10 other species.</span>

MetaboLights follows the [ISA framework](https://isa-tools.org/),
where ISA is short for Investigation, Study, and Assay. Following this standard, the information
about the study, investigations, and assays are stored in structured data (tabular files
in ISATab, and in a hierarchical model in ISAJSON). Additional file may be provided for
additional information. For example, MetaboLights uses files that start with the
prefix `m_` where information about the metabolites are collected.

## Unexpected similarities

One of the studies where ATP was found is [MTBLS88](https://www.ebi.ac.uk/metabolights/MTBLS88).
This study compares human blood samples with
[Schizosaccharomyces](https://en.wikipedia.org/wiki/Schizosaccharomyces).

---

[prev](./identification.md) | [toc](./README.md) | [next](pathways.md)

Copyright 2020 (C) Egon Willighagen - CC-BY Int. 4.0
