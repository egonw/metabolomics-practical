# Metabolite Identification

[prev](./databases.md) | [toc](./README.md) | [next](omics.md)

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

## Mass spectrometry

[Mass spectrometry](https://en.wikipedia.org/wiki/Mass_spectrometry) is an analytical
methods that uses the [mass-to-charge ratio](https://en.wikipedia.org/wiki/Mass_spectrometry)
to characterize compounds. During a mass spectral analysis it is common that
the compound breaks down in smaller fragments, resulting in multiple peaks. The masses
of the fragments or compound specific. But even then, with just a mass spectrum
it is not easy to identify a compound.

1. why will we not see lysine (C₆H₁₄N₂O₂) in a mass spectrum? <button onclick="toggleAnswer('q1')">Answer</button><span id="q1" style="visibility: hidden"> Because it is not charged. However, we can see its protonated and deprotoned counterparts.</span>

### Monoisotopic masses

The monoisotopic mass is the mass of a compound with all atoms having a single,
major isotopic mass for each element. For example, the monoisotopic mass of
hydroxyurea is 76.02728.

2. how many compound in ChEBI have this monoisotopic mass? (use the advanced search functionality) <button onclick="toggleAnswer('q2')">Answer</button><span id="q2" style="visibility: hidden"> Two: CHEBI:38662 and CHEBI:44423</span>

You can experiment with the range in the advanced search. Making it slightly larger
increases the number of search hits. Try searching for the range 76.0 to 76.5.

### Molecular formula

Lysine has the molecular formula C₆H₁₄N₂O₂. If the mass spectrum gives us a [M+H]+ peak
matching it molecular formula C₆H₁₅N₂O₂+ then it could be lysine. But with only the
chemical formula, we do not know how the atoms are bound to each other. That is, we
do not know what the correct stereoisomer is. In fact, we do not even know what the
correct constitutional isomer is.

3. how many compound entries does ChEBI return if you search for the chemical formula C₆H₁₄N₂O₂? (use the advanced search functionality) <button onclick="toggleAnswer('q3')">Answer</button><span id="q3" style="visibility: hidden"> ChEBI lists 30116 entries with this chemical formula (at the time of writing)</span>





---

[prev](./databases.md) | [toc](./README.md) | [next](omics.md)

Copyright 2020-2022 (C) Egon Willighagen - CC-BY Int. 4.0
