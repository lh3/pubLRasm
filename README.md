## Introduction

When developing a new assembler, we often need to run other assemblers and to
compare the results. However, it is not always easy to run others' tools and
assembling a large genome may take days or even weeks. To save developers'
time, here we provide stable links to multiple public long-read assemblies and
their input data if possible. "Stable links" refer to links provided by NCBI,
Zenodo, FigShare, etc that data owners cannot change. FTP links or links to
S3/GCP buckets are not stable.

## Assemblies

### CHM13: homozygous human

|Data                |Assembler        |Version |Source                       |Link|
|:-------------------|:----------------|-------:|:----------------------------|:---|
|HiFi                |[Flye][Flye]     |2.8     |Dev website                  |[Download](https://zenodo.org/record/3965035/files/flye.v28.chm13.hifi.30x.fasta.gz?download=1)|
|ONT                 |[Flye][Flye]     |2.8     |Dev website                  |[Download](https://zenodo.org/record/3965035/files/flye.v28.chm13.ont.120x.fasta.gz?download=1)|
|CLR                 |Falcon           |        |                             |[Download](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/983/455/GCA_000983455.1_CHM13_Draft_Assembly/GCA_000983455.1_CHM13_Draft_Assembly_genomic.fna.gz)|
|[ONT][CHM13-ont2]+SR|[WengenD][Wengen]|0.2     |[Genova et al][Wengan-pmid]  |[Download](https://zenodo.org/record/3779515/files/CHM13.WenganD.ILL_UL_R3.fa.gz?download=1)   |
|[HiFi][CHM13-hifi1] |hifiasm          |0.12    |Cheng et al                  |Download|
|[HiFi][CHM13-hifi1] |HiCanu           |2.1     |Cheng et al                  |Download|

### HG00733: heterozygous human

|Data                  |Assembler        |Version|Type     |Source                         |Link|
|:---------------------|:----------------|------:|:--------|:------------------------------|:---|
|[CLR][HG00733-clr]    |Falcon-Unzip     |       |Primary  |[Kronenberg et al][FP-preprint]|[Download](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/775/GCA_012067775.1_HG00733.Unzip_primary/GCA_012067775.1_HG00733.Unzip_primary_genomic.fna.gz)|
|[CLR][HG00733-clr]+HiC|Falcon-Phase     |       |Phased   |[Kronenberg et al][FP-preprint]|[hap1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/855/GCA_012067855.1_HG00733.phase0_contigs/GCA_012067855.1_HG00733.phase0_contigs_genomic.fna.gz), [hap2](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/805/GCA_012067805.1_HG00733.phase1_contigs/GCA_012067805.1_HG00733.phase1_contigs_genomic.fna.gz)|
|[CLR][HG00733-clr]    |[WengenD][Wengen]|0.2    |Collapsed|[Genova et al][Wengan-pmid]    |[Download](https://zenodo.org/record/3779515/files/HG00733.WenganD.PAC-SequelI.fa.gz?download=1)
|[HiFi][HG00733-hifi]  |hifiasm          |0.12   |Primary  |Cheng et al                    |Download|
|[HiFi][HG00733-hifi]+[SRpat][HG00733-sr-pat]+[SRmat][HG00733-sr-mat]|hifiasm|0.12|Phased|Cheng et al|hap1,hap2|
|[HiFi][HG00733-hifi]  |HiCanu           |2.1    |Primary  |Cheng et al                    |Download|
|[HiFi][HG00733-hifi]+[SRpat][HG00733-sr-pat]+[SRmat][HG00733-sr-mat]|HiCanu |2.1 |Phased|Cheng et al|hap1,hap2|


[CHM13-hifi1]: https://www.ncbi.nlm.nih.gov/sra?term=(((SRR11292120)%20OR%20SRR11292121)%20OR%20SRR11292122)%20OR%20SRR11292123
[Flye]: https://github.com/fenderglass/Flye
[Flye-pmid]: https://pubmed.ncbi.nlm.nih.gov/30936562/
[Falcon-pmid]: https://pubmed.ncbi.nlm.nih.gov/27749838/
[FP-preprint]: https://www.biorxiv.org/content/10.1101/327064v2
[CHM13-ont2]: https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel3/rel3.fastq.gz
[Wengen]: https://github.com/adigenova/wengan
[Wengan-pmid]: https://pubmed.ncbi.nlm.nih.gov/33318652/
[HG00733-clr]: https://www.ncbi.nlm.nih.gov/sra/?term=SRR7615963
[HG00733-hifi]: https://www.ebi.ac.uk/ena/data/view/ERX3831682
[HG00733-sr-pat]: https://www.ebi.ac.uk/ena/data/view/ERR3241754
[HG00733-sr-mat]: https://www.ebi.ac.uk/ena/data/view/ERR3241755
