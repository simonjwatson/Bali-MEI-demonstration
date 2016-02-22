# Bali MEI Practical Demonstration

Here we'll look at the **H3N2** isolates sampled in **Bali** by phylogenetically placing them in the context of the global isolates.

If you'll remember from the talk, we got no sequence back for the HA and NA gene segments, so we will look at the PB2 gene segment, which we got 17 sequences back.

### Phylogenetically placing the Balinese H3N2 PB2 sequences

1. Download all files by clicking on the "Download ZIP" button at the top right

The Balinese sequences can be found in the `Bali-sequences` folder as `Bali-MEI.H3N2.PB2.fas`

This is a plain text FASTA file and can be opened in any text editor to view the sequences.

2. Open the FASTA file in a text editor to see how the file looks.

To view the sequences as an alignment we need to download an alignment viewer. A good one is `AliView` which can be downloaded from http://www.ormbunkar.se/aliview/

3. Download AliView and use it to open the FASTA file.

You'll see that the sequences have already been aligned and trimmed to the coding region of the PB2 gene.

Now we need some background sequences from the rest of the world to place ours in a global context. A good repository for influenza sequences is the Influenza Resource Database (IRD) http://www.ncbi.nlm.nih.gov/genomes/FLU/Database/nph-select.cgi?go=database which is run by the NCBI.

4. Download a background set for our Bali sequences. Make sure you set:
```
sequence Type: Nucleotide
Type: A
Host: Human
Country: Continents: Africa, Asia, Europe, Oceania, South America
Segment: 1 (PB2)
Subtype: H3
Subtype: N2
Full-length only
Collection date from: 2012
Collapse identical sequences
```

We are excluding the North American sequences because there are so many of them, and this way we can keep our dataset to a manageable size. In reality you'd want to include them.

You should get a window with 208 nucleotide sequences after collapsing.

5. Download these by changing to `Coding Region` and clicking `Download`

6. Open the file you downloaded in `AliView`

You'll see that they're all aligned nicely for you, as we selected `Coding Region` in the download menu. These should also align nicely with our Bali sequences.

7. Combine 
