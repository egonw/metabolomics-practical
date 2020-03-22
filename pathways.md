# Pathway Analysis

[prev](./omics.md) | [toc](./README.md)

Continuing from the data set we looked at in the [previous section](./omics.md), we first have
to define the two sitations we want to compare. Otherwise, we cannot saw which pathways
are changed when comparing the two situations. Let's compare the read bloos cell samples
with plasma:

```R
rbcColumns = c(
  "Person4_RBC1_POS", "Person4_RBC2_POS",
  "Person4_RBC3_POS", "Person4_RBC4_POS"
)
plasmaColumns = c(
  "Person4_Plasma1_POS", "Person4_Plasma2_POS",
  "Person4_Plasma3_POS", "Person4_Plasma4_POS"
)
```


---

[prev](./omics.md) | [toc](./README.md)

Copyright 2020 (C) Egon Willighagen - CC-BY Int. 4.0
