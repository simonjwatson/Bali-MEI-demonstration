# Bali MEI Practical Demonstration

Here we'll look at the **H3N2** isolates collected in **Bali**, by phylogenetically placing them in the context of the global isolates.

If you'll remember from the talk, we got no sequence back for the HA and NA gene segments, so we will look at the PB2 gene segment, for which we got 17 sequences back.

### Phylogenetically placing the Balinese H3N2 PB2 sequences

1. Download all files by clicking on the `Download ZIP` button at the top right

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

  You should get a window with `208 nucleotide sequences after collapsing`.

5. Download these by changing to `Coding Region` and clicking `Download`

  If you weren't able to download them, you can find them in a pre-downloaded file called `IVR-sequences.fa` in the `IVR-sequences` folder.

6. Open the file you downloaded in `AliView`

  You'll see that they're all aligned nicely for you, as we selected `Coding Region` in the download menu. These should also align nicely with our Bali sequences.

  We also want to download an outgroup sequence that we can use to orient our phylogenetic tree. To do this we are going to pick the vaccine strain from 2011.

  We can see this by going to http://www.nextflu.org/H3N2/6y/ and hovering over the bold X.

  You'll see the 2011 H3N2 vaccine strain was `A/Victoria/361/2011`

7. Go to GenBank http://www.ncbi.nlm.nih.gov/genbank/ and download the PB2 segment of this vaccine strain.

  If you're unable to download it, you can find a pre-downloaded file called `A_Victoria_361_2011.fas` in the folder `outgroup`

  We now want to combine the 3 files we have into one alignment:
  ```
  A_Victoria_361_2011
  IVR-sequences.fa
  Bali-MEI.H3N2.PB2.fas
  ```

8. Open any one of these files in `AliView` then append the others by going to the `Edit` menu and selecting `Add sequences from file`. Add the other 2 files.

  You'll see that the sequences are not all aligned with respect to each other.

9. Automatically align the sequences by going to `Align` and selecting `Realign everything`. This may take a few minutes.

  Once it's finished, close the dialog box. You'll see that they are all nicely aligned but that the outgroup sequence has extra sequence beyond the coding region.

10. Remove the extra non-coding sequence by highlighting the columns in `AliView` and going to `Edit` then `Delete selected`.

11. Save this combined file by going to `File` then `Save as FASTA`.

  If you were unable to create the aligned and trimmed file, a pre-prepared file called `combined.H3N2.PB2.fas` is in the folder `combined`.
