# bio-410-final-project
## Background
The data consists of 6 samples from the organism Zaire ebolavirus. This organism is a highly infectious human pathogen and a member of the Filoviridae family. The virus is known for causing severe hemorrhagic fever in humans and its ability to infect cells depends on a surface protein called glycoprotein (GP). Research by Uedo et al. (2017) shows that the virus can even evolve during outbreaks to spread more easily! From studying the 2014-2015 West African epidemic, researchers found a specific mutation, A82V, that helped the virus be more efficient at entering human cells. This study really showed how small changes in a virus's genetic code can help it adapt to new hosts and cause a larger outbreak of infection.

Source

Ueda, M. T., Kurosaki, Y., Izumi, T., Nakano, Y., Oloniniyi, O. K., Yasuda, J., Koyanagi, Y., Sato, K., & Nakagawa, S. (2017). Functional mutations in spike glycoprotein of Zaire ebolavirus associated with an increase in infection efficiency. Genes to Cells, 22(2), 148–159. https://doi.org/10.1111/gtc.12463

## Purpose 
The purpose of this project is to create a phylogenetic tree from 6 samples of Zaire ebolavirus in order to determine the evolutionary relationships between the samples. By performing a multiple sequence alignment and constructing a phylogenetic tree, I am to determine the evolutionary relationships between these samples and identify how they have diverged from one another.

## Methods 
The sequencing reads themselves came from the Next Generation Sequecing (NGS) process. I obtained them under the file named diana.zip. These FASTQ files were then assembled into contigs using MEGAHIT and this process was repeated for all six samples. The resulting data went into the final.contigs.fa file. Then, by using the BioStrings and DESIPHER packages in R studio, I imported the contigs. I filtered the data to include only sequences longer than 5,000 base pairs to remove small or incomplete fragments. Next, I performed an alignment of the assembled sequences with the AlignSeqs function and this allowed me to compare any similarities and differences. The alignment was saved as an HTML file. Finally, I constructed the phylogenetic tree using the Maximum Likelihood (ML) method via the TreeLine function. This created the most probable evolutionary relationship between the samples. 


## Results
here is the phylogenetic tree
insert image here (see markov cheat sheet)

![phylogenetic tree](image.jpg)

The tree reveals 2 prominent branches that extend. Samples 2 and 3 are closely related to each other and form their own distinct lineage. Samples 1, 4, 5, 6, and 7 form the other separate cluster. Within this cluster, 1 and 6 are closely related, 4 and 7 are closely related, and 5 is more on its own. Based on this, the tree likely is representing 2 individuals or 2 distinct strains of the virus. Overall, the tree shows the samples diverged into 2 clades which means that the samples involve at least 2 genetically distinct lineages of Zaire ebolavirus. 
