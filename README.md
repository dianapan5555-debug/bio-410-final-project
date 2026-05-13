# bio-410-final-project
## Background
The data consists of 6 samples from the organism Zaire ebolavirus. This organism is a highly infectious human pathogen and a member of the Filoviridae family. The virus is known for causing severe hemorrhagic fever in humans and its ability to infect cells depends on a surface protein called glycoprotein (GP). Research by Uedo et al. (2017) shows that the virus can even evolve during outbreaks to spread more easily! From studying the 2014-2015 West African epidemic, researchers found a specific mutation, A82V, that helped the virus be more efficient at entering human cells. This study really showed how small changes in a virus's genetic code can help it adapt to new hosts and cause a larger outbreak of infection.

Source
Ueda, M. T., Kurosaki, Y., Izumi, T., Nakano, Y., Oloniniyi, O. K., Yasuda, J., Koyanagi, Y., Sato, K., & Nakagawa, S. (2017). Functional mutations in spike glycoprotein of Zaire ebolavirus associated with an increase in infection efficiency. Genes to Cells, 22(2), 148–159. https://doi.org/10.1111/gtc.12463

## Purpose 
The purpose of this project is to create a phylogenetic tree from 6 samples of Zaire ebolavirus in order to determine the evolutionary relationships between the samples. By performing a multiple sequence alignment and constructing a phylogenetic tree, I am to determine the evolutionary relationships between these samples and identify how they have diverged from one another.

## Methods 
The sequencing reads themselves came from the Next Generation Sequecing (NGS) process. These FASTQ files were assembled into contigs using MEGAHIT and this process was repeated for all six samples to reconstruct (provide link megahit website). Then, by using the DESIPHER package in R studio, I imported the contigs and filtered for longer sequences. I performed an alignment of the assembled sequences with the AlignSeqs function and this allowed me to compare any similarities and differences. The alignment saved as an html file. Finally, I constructed the phylogenetic tree using the Maximum Likelihood (ML) method via the TreLine function in DECIPHER. This calculated the most probable evolutionary relationship between the samples. 
then alignment using r package DESIPHER
for each source of data, state which files was in the repository corresponded to the data (ex. assembled reads are in x folder and raw sequencing reads are in y folder (the one with my name)

## Results
here is the phylogenetic tree
insert image here (see markov cheat sheet)

![phylogenetic tree](image.jpg)

explain which samples are closely related to each other, how many individuals did these samples probably come from based on the phylogenetic tree
