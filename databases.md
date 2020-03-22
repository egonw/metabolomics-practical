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

The key databases are the folling

* [Human Metabolomics Database](http://hmdb.ca) (HMDB)
* [Chemical Entities of Biological Interest](https://www.ebi.ac.uk/chebi/) (ChEBI)
* [LIPID MAPS](https://lipidmaps.org/)

More general databases include the following two:

* [PubChem](https://pubchem.ncbi.nlm.nih.gov/)
* [ChemSpider](https://www.chemspider.com/)

## Questions

What are the database identifiers for ChEBI, HMDB, and PubChem for the following
compounds:

1. glycine found in human protein? <button onclick="toggleAnswer('q1')">Answer</button><span id="q1" style="visibility: hidden">CHEBI:15428, HMDB0000123, 750</span>
2. paracetamol? <button onclick="toggleAnswer('q2')">Answer</button><span id="q2" style="visibility: hidden">CHEBI:46195, HMDB0001859, 1983</span>

# Stereoisomers

The [stereochemistry](https://en.wikipedia.org/wiki/Stereochemistry) of a chemical
compound determines the spatial orientation of atoms in the molecule.

## Questions

What are the database identifiers for ChEBI, HMDB, and PubChem for the following
compounds:

3. does butane have stereoisomers? <button onclick="toggleAnswer('q3')">Answer</button><span id="q3" style="visibility: hidden">Yes, the single bonds can be rotated freely, it has various rotamers.</span>
4. does 2-butene have stereoisomers? <button onclick="toggleAnswer('q4')">Answer</button><span id="q4" style="visibility: hidden">Yes, the double bond can be <i>cis</i> and <i>trans</i>.</span>
5. what are they ChEBI identifiers of the stereoisomers of lysine?<button onclick="toggleAnswer('q5')">Answer</button><span id="q5" style="visibility: hidden">CHEBI:16855 and CHEBI:18019 (CHEBI:25094 is a non-existing entity used to specify a compuond with unknown stereochemistry)</span>

# Charge states

ChEBI has different entries in the database for different the protonated and deprotonated
compound. 

## Questions

6. what are the ChEBI identifiers for acetic acid and acetate? <button onclick="toggleAnswer('q6')">Answer</button><span id="q6" style="visibility: hidden">CHEBI:15366 and CHEBI:30089</span>

# Isotopes

Most ChEBI entries represent the chemical structure and the mass is given for the structure where
all atoms have the most abundant isotope (e.g. <sup>12</sup>C and <sup>1</sup>H). However, it can
also have entries for compounds with a specific isotope. Of course, with different identifiers.

## Questions

7. what are the ChEBI identifiers water and heavy water? <button onclick="toggleAnswer('q7')">Answer</button><span id="q7" style="visibility: hidden">CHEBI:15377 and CHEBI:33813</span>


---

[toc](./README.md) | [next](identification.md)

Copyright 2020 (C) Egon Willighagen - CC-BY Int. 4.0
