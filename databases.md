# Metabolite Databases

[toc](./README.md) | [next](identification.md)

<script>
  function toggleAnswer(id) {
  var answer = document.getElementById(id);
  if (answer.style.visibility === "hidden" ||
      answer.style.visibility === "none") {
    answer.style.visibility = "visible";
  } else {
    answer.style.visibility = "hidden";
  }
}
</script>

The key metabolite databases are the following list:

* [Human Metabolomics Database](http://hmdb.ca) (HMDB): focuses on human metabolites
* [Chemical Entities of Biological Interest](https://www.ebi.ac.uk/chebi/) (ChEBI): focuses on accurate description of the chemistry
* [LIPID MAPS](https://lipidmaps.org/): focuses on lipids in any species
* [LOTUS](https://lotus.naturalproducts.net/): focuses on natural products

More general databases include the following two, but because also human samples contain non-human metabolites, they are of relevance.
They both have a chemistry focus but link out to many useful databases:

* [PubChem](https://pubchem.ncbi.nlm.nih.gov/): [114 million](https://pubchem.ncbi.nlm.nih.gov/docs/statistics) chemical structures, by the American [NCBI](https://www.ncbi.nlm.nih.gov/)
* [ChemSpider](https://www.chemspider.com/): >100 millsion structures, and like PubChem, but by the British [RSC](https://www.rsc.org/)
* [Wikidata](https://scholia.toolforge.org/chemical/): 1.3 million structures; a machine-readable sister of Wikipedia (via Scholia interface)

## Questions

What are the database identifiers for ChEBI, HMDB, and PubChem for the following
compounds:

1. glycine found in human protein? <button onclick="toggleAnswer('q1')"> Answer</button><span id="q1" style="visibility: hidden"> <a href="https://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI:15428">CHEBI:15428</a>, <a href="https://hmdb.ca/metabolites/HMDB0000123">HMDB0000123</a>, <a href="https://pubchem.ncbi.nlm.nih.gov/compound/750">750</a></span>
2. paracetamol? <button onclick="toggleAnswer('q2')"> Answer</button><span id="q2" style="visibility: hidden"> CHEBI:46195, HMDB0001859, 1983</span>

# Stereoisomers

The [stereochemistry](https://en.wikipedia.org/wiki/Stereochemistry) of a chemical
compound determines the spatial orientation of atoms in the molecule.

## Questions

3. does butane have stereoisomers? <button onclick="toggleAnswer('q3')"> Answer</button><span id="q3" style="visibility: hidden"> Yes, the single bonds can be rotated freely, it has various rotamers.<br /><img src="https://www.simolecule.com/cdkdepict/depict/bot/svg?smi=CCCC" width="300"/></span>
4. does 2-butene have stereoisomers? <button onclick="toggleAnswer('q4')"> Answer</button><span id="q4" style="visibility: hidden"> Yes, the double bond can be <i>cis</i> and <i>trans</i>.</span>
5. what are they ChEBI identifiers of the stereoisomers of lysine?<button onclick="toggleAnswer('q5')"> Answer</button><span id="q5" style="visibility: hidden"> CHEBI:16855 and CHEBI:18019 (CHEBI:25094 is a non-existing entity used to specify a compuond with unknown stereochemistry)</span>

# Charge states

ChEBI has different entries in the database for different the protonated and deprotonated
compound. 

## Questions

6. what are the ChEBI identifiers for acetic acid and acetate? <button onclick="toggleAnswer('q6')">Answer</button><span id="q6" style="visibility: hidden"> CHEBI:15366 and CHEBI:30089</span>

# Isotopes

Most ChEBI entries represent the chemical structure and the mass is given for the structure where
all atoms have the most abundant isotope (e.g. <sup>12</sup>C and <sup>1</sup>H). However, it can
also have entries for compounds with a specific isotope. Of course, with different identifiers.

## Questions

7. what are the ChEBI identifiers for water and heavy water? <button onclick="toggleAnswer('q7')">Answer</button><span id="q7" style="visibility: hidden"> CHEBI:15377 and CHEBI:33813</span>

# Spectral databases

There are many databases that have spectra for small compounds, two of them are:

* [MassBank Europe](https://massbank.eu/MassBank/) (for mass spectra)
* [NMRShiftDb](https://nmrshiftdb.nmr.uni-koeln.de/) (for NMR spectra)

8. how many peaks does the <sup>1</sup>H NMR spectrum of isopropanol have? <button onclick="toggleAnswer('q8')">Answer</button><span id="q8" style="visibility: hidden"> Two. The hydroxyl proton is not visible in polar solvents, so we only see peaks at 4.04 ppm and 1.22 ppm.</span>
9. at what m/z value does glycine the highest peak? <button onclick="toggleAnswer('q9')">Answer</button><span id="q9" style="visibility: hidden"> That actually depends on the method used. The [M+h]+ peak is around 76, while the [M-H]- peak is around 74. Why do we not measure the [M] peak?</span>


---

[toc](./README.md) | [next](identification.md)

Copyright 2020-2022 (C) Egon Willighagen - CC-BY Int. 4.0
