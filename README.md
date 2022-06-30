# Reference Genomes
Examples for downloading reference genomes using wget command.
****

Current example is based on human genome (Homo sapiens - GRCh38, release 106) from emsembl (http://ensemblgenomes.org).

Other genomes can be downloaded here:
* Vertebrates genome as mice (http://asia.ensembl.org/info/data/ftp/index.html/). 
* Plants genomes as arabidiosis, rice, grape (http://plants.ensembl.org/info/data/ftp/index.html). 
* Bacteria genomes as pseudomonas  (https://bacteria.ensembl.org/info/data/ftp/index.html)
* Fungi genomes as saccharomyces (https://fungi.ensembl.org/info/data/ftp/index.html).
* Protist genomes as phytophthora (http://protists.ensembl.org/info/data/ftp/index.html).
* Metazoa genomes as drosophila (http://metazoa.ensembl.org/info/data/ftp/index.html).

<!-- http://ftp.ensembl.org/pub/release-106/fasta/homo_sapiens/dna/ -->

(1) For transcriptome analisys using STAR, we will need both dna-fasta and gft/gff3 files.
```
wget http://ftp.ensembl.org/pub/current_fasta/homo_sapiens/dna/Homo_sapiens.GRCh38.dna_sm.primary_assembly.fa.gz

wget http://ftp.ensembl.org/pub/release-106/gtf/homo_sapiens/Homo_sapiens.GRCh38.106.abinitio.gtf.gz
#or
wget http://ftp.ensembl.org/pub/release-106/gff3/homo_sapiens/Homo_sapiens.GRCh38.106.abinitio.gff3.gz

```

(2) In the case of transcriptome analisys using Kallisto or Salmon, we will only need cdna-fasta.
```
wget http://ftp.ensembl.org/pub/current_fasta/homo_sapiens/cdna/Homo_sapiens.GRCh38.cdna.abinitio.fa.gz
```

(3) For other type of analysis that would involved non-coding rna, this is the file
```
wget http://ftp.ensembl.org/pub/current_fasta/homo_sapiens/ncrna/Homo_sapiens.GRCh38.ncrna.fa.gz
```
