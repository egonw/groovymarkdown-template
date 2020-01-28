# Introduction

## Including Groovy code examples

This is how you include a script:

**Script** [code/Example.groovy](code/Example.code.md)
```groovy
@Grab(group='org.openscience.cdk', module='cdk-bundle', version='2.3')
import org.openscience.cdk.smiles.SmilesParser;
import org.openscience.cdk.interfaces.*;
import org.openscience.cdk.*;
sp = new SmilesParser(
  DefaultChemObjectBuilder.getInstance()
)
mol = sp.parseSmiles("CC(=O)OC1=CC=CC=C1C(=O)O")
println "Aspirin has ${mol.atomCount} atoms."
```

And this is how to include the output:

Aspirin has 13 atoms.

## Including references

You can include references by proviing the Wikidata item identifier
for the paper, e.g. like [<a href="#citeref1">1</a>].
