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

Using these two groups, we can calculate log fold changes (logFC) with:

```R
logFC = log2(
  apply(mtbls88[,rbcColumns], 1, function(x) sum(x)) /
  apply(mtbls88[,plasmaColumns], 1, function(x) sum(x))
)
hist(logFC, breaks = 50, col="gold")
```

The `hist()` command shows a histogram of of the fold changes:

<img src="./i/Screenshot_20200323_000103.png" width="400px" />

We are going to use this data in [PathVisio](https://pathvisio.github.io/) and need to export it
as a TSV file first. We create a new data matrix, and leave out a few rows:

```R
logFCdata = cbind(
    as.character(mtbls88[,"database_identifier"]),
    logFC
  )[-c(27,47,49,75,77),]
write.table(
  logFCdata, file = "logfc.tsv",
  sep = "\t",
  col.names = c("ChEBI", "logFC"),
  row.names = FALSE, quote = FALSE
)
```

## Finding pathways with PathVisio

Following the same approach for pathway analysis with other omics data, we can use this data
to find potentially interesting pathways. First, download the
[metabolite identifier database](https://bridgedb.github.io/data/gene_database/)
and open that in PathVisio with `Data`, `Select Metabolite Database`.

Then, import the `logfc.tsv` file you created in the previous step into PathVisio
with `Data`, `Import expression data`. The file is TAB separated:

<img src="./i/Screenshot_20200322_235940.png" width="400px" />


The first `CHEBI` column has the identifiers, and they are all `ChEBI` identifiers:

<img src="./i/Screenshot_20200323_000016.png" width="400px" />

If all went well with loading the metabolite identifier database and importing
the expression data, then all 73 data rows should be imported correctly and all identifiers
recognized:

<img src="./i/Screenshot_20200323_000025.png" width="400px" />




---

[prev](./omics.md) | [toc](./README.md)

Copyright 2020 (C) Egon Willighagen - CC-BY Int. 4.0
