## Introduction

When developing a new assembler, we often need to run other assemblers and to
compare the results. However, it is not always easy to run others' tools and
assembling a large genome may take days or even weeks. To save developers'
time, here we provide stable links to multiple public long-read assemblies and
their input data if possible. "Stable links" refer to links provided by NCBI,
Zenodo, FigShare, etc, which can't be modified by data owners. FTP links or
links to S3/GCP buckets are not stable.

## Assemblies

### CHM13: homozygous human

|Data                |Assembler        |Version |Source                            |Link|
|:-------------------|:----------------|-------:|:---------------------------------|:---|
|HiFi                |[Flye][Flye]     |2.8     |Dev website                       |[Zenodo](https://zenodo.org/record/3965035/files/flye.v28.chm13.hifi.30x.fasta.gz?download=1)|
|[HiFi][CHM13-hifi1] |Falcon           |1.8.1   |Cheng et al                       |[Zenodo](https://zenodo.org/record/4393631/files/CHM13.HiFi.Falcon-1.8.1.fa.gz?download=1)|
|[HiFi][CHM13-hifi1] |[HiCanu][canu]   |2.1     |Cheng et al                       |[Zenodo](https://zenodo.org/record/4393631/files/CHM13.HiFi.HiCanu-2.1.fa.gz?download=1)|
|[HiFi][CHM13-hifi1] |[hifiasm][hifiasm]|0.12   |Cheng et al                       |[Zenodo](https://zenodo.org/record/4393631/files/CHM13.HiFi.hifiasm-0.12.fa.gz?download=1)|
|[HiFi][CHM13-hifi1] |[Peregrine][pg]  |0.1.6.1 |Cheng et al                       |[Zenodo](https://zenodo.org/record/4393631/files/CHM13.HiFi.Peregrine-0.1.6.1.fa.gz?download=1)|
|ONT                 |[Canu][canu]+[Helen][helen]|1.8+0.1|[Shafin et al][sh-pmid]  |[Zenodo](https://zenodo.org/record/4393631/files/CHM13.ONT.Canu-1.8_Helen.fa.gz?download=1)|
|ONT                 |[Flye][Flye]+[Helen][helen]|2.4.2+0.1|[Shafin et al][sh-pmid]|[Zenodo](https://zenodo.org/record/4393631/files/CHM13.ONT.Flye-2.4.2_Helen.fa.gz?download=1)|
|ONT                 |[Flye][Flye]     |2.8     |Dev website                       |[Zenodo](https://zenodo.org/record/3965035/files/flye.v28.chm13.ont.120x.fasta.gz?download=1)|
|ONT                 |[Shasta][shasta]+[Helen][helen]|0.1.0|[Shafin et al][sh-pmid]|[Zenodo](https://zenodo.org/record/4393631/files/CHM13.ONT.Shasta-0.1.0_Helen.fa.gz?download=1)|
|[ONT][CHM13-ont2]+SR|[WengenD][Wengen]|0.2     |[Di Genova et al][Wengan-pmid]    |[Zenodo](https://zenodo.org/record/3779515/files/CHM13.WenganD.ILL_UL_R3.fa.gz?download=1)   |
|CLR                 |Falcon           |        |                                  |[NCBI](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/000/983/455/GCA_000983455.1_CHM13_Draft_Assembly/GCA_000983455.1_CHM13_Draft_Assembly_genomic.fna.gz)|

### HG00733: heterozygous human

|Data                  |Assembler        |Version|Type     |Source                                 |Link|
|:---------------------|:----------------|------:|:--------|:--------------------------------------|:---|
|[HiFi][HG00733-hifi]  |Falcon           |1.8.1  |Primary  |Cheng et al                            |[Zenodo](https://zenodo.org/record/4393631/files/HG00733.HiFi.Falcon-1.8.1.pri.fa.gz?download=1)|
|[HiFi][HG00733-hifi]  |[HiCanu][canu]   |2.1    |Primary  |Cheng et al                            |[Zenodo](https://zenodo.org/record/4393631/files/HG00733.HiFi.HiCanu-2.1.pri.fa.gz?download=1)|
|[HiFi][HG00733-hifi]+[SRpat][HG00733-sr-pat]+[SRmat][HG00733-sr-mat]|[HiCanu][canu]|2.1 |Phased|Cheng et al|[hap1](https://zenodo.org/record/4393631/files/HG00733.HiFi.HiCanu-2.1.hap1.fa.gz?download=1), [hap2](https://zenodo.org/record/4393631/files/HG00733.HiFi.HiCanu-2.1.hap2.fa.gz?download=1)|
|[HiFi][HG00733-hifi]  |[hifiasm][hifiasm]|0.12  |Primary  |Cheng et al                            |[Zenodo](https://zenodo.org/record/4393631/files/HG00733.HiFi.hifiasm-0.12.pri.fa.gz?download=1)|
|[HiFi][HG00733-hifi]+[SRpat][HG00733-sr-pat]+[SRmat][HG00733-sr-mat]|[hifiasm][hifiasm]|0.12|Phased|Cheng et al|[hap1](https://zenodo.org/record/4393631/files/HG00733.HiFi.hifiasm-0.12.hap1.fa.gz?download=1), [hap2](https://zenodo.org/record/4393631/files/HG00733.HiFi.hifiasm-0.12.hap2.fa.gz?download=1)|
|[HiFi][HG00733-hifi]  |[Peregrine][pg]  |0.1.6.1|Primary  |Cheng et al                            |[Zenodo](https://zenodo.org/record/4393631/files/HG00733.HiFi.Peregrine-0.1.6.1.pri.fa.gz?download=1)|
|[HiFi][HG00733-hifi]+[SRpat][HG00733-sr-pat]+[SRmat][HG00733-sr-mat]|[Peregrine][pg]|0.1.6.1|Phased|Cheng et al|[hap1](https://zenodo.org/record/4393631/files/HG00733.HiFi.Peregrine-0.1.6.1.hap1.fa.gz?download=1), [hap2](https://zenodo.org/record/4393631/files/HG00733.HiFi.Peregrine-0.1.6.1.hap2.fa.gz?download=1)|
|[HiFi][HG00733-hifi]+[HiC][HG00733-hic]|[DipAsm][da]+[Peregrine][pg]||Phased|[Garg et al][da-pmid]|[hap1](https://zenodo.org/record/4393631/files/HG00733.HiFi_HiC.DipAsm_Peregrine.hap1.fa.gz?download=1), [hap2](https://zenodo.org/record/4393631/files/HG00733.HiFi_HiC.DipAsm_Peregrine.hap2.fa.gz?download=1)|
|[HiFi][HG00733-hifi]+StrandSeq|[PGAS][pgas]+[Peregrine][pg]||Phased   |[Porubsky et al][ss-pmid]  |[hap1](https://zenodo.org/record/4393631/files/HG00733.HiFi_StrandSeq.PGAS_Peregrine.hap1.fa.gz?download=1), [hap2](https://zenodo.org/record/4393631/files/HG00733.HiFi_StrandSeq.PGAS_Peregrine.hap2.fa.gz?download=1)|
|ONT                   |[Canu][canu]+[Helen][helen]    |1.8+0.1  |Collapsed|[Shafin et al][sh-pmid]|[Zenodo](https://zenodo.org/record/4393631/files/HG00733.ONT.Canu-1.8_Helen.pri.fa.gz?download=1)|
|ONT                   |[Flye][Flye]+[Helen][helen]    |2.4.2+0.1|Collapsed|[Shafin et al][sh-pmid]|[Zenodo](https://zenodo.org/record/4393631/files/HG00733.ONT.Flye-2.4.2_Helen.pri.fa.gz?download=1)|
|ONT                   |[Shasta][shasta]+[Helen][helen]|0.1.0+0.1|Collapsed|[Shafin et al][sh-pmid]|[Zenodo](https://zenodo.org/record/4393631/files/HG00733.ONT.Shasta-0.1.0_Helen.pri.fa.gz?download=1)|
|[CLR][HG00733-clr]    |Falcon-Unzip     |       |Primary  |[Kronenberg et al][FP-preprint]        |[NCBI](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/775/GCA_012067775.1_HG00733.Unzip_primary/GCA_012067775.1_HG00733.Unzip_primary_genomic.fna.gz)|
|[CLR][HG00733-clr]+HiC|Falcon-Phase     |       |Phased   |[Kronenberg et al][FP-preprint]        |[hap1](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/855/GCA_012067855.1_HG00733.phase0_contigs/GCA_012067855.1_HG00733.phase0_contigs_genomic.fna.gz), [hap2](https://ftp.ncbi.nlm.nih.gov/genomes/all/GCA/012/067/805/GCA_012067805.1_HG00733.phase1_contigs/GCA_012067805.1_HG00733.phase1_contigs_genomic.fna.gz)|
|[CLR][HG00733-clr]    |[WengenD][Wengen]|0.2    |Collapsed|[Di Genova et al][Wengan-pmid]         |[Zenodo](https://zenodo.org/record/3779515/files/HG00733.WenganD.PAC-SequelI.fa.gz?download=1)|

[CHM13-hifi1]: https://www.ncbi.nlm.nih.gov/sra?term=(((SRR11292120)%20OR%20SRR11292121)%20OR%20SRR11292122)%20OR%20SRR11292123
[Flye]: https://github.com/fenderglass/Flye
[canu]: https://github.com/marbl/canu
[pg]: https://github.com/cschin/Peregrine
[pgas]: https://github.com/ptrebert/project-diploid-assembly
[helen]: https://github.com/kishwarshafin/helen
[da]: https://github.com/shilpagarg/DipAsm
[hifiasm]: https://github.com/chhylp123/hifiasm
[shasta]: https://github.com/chanzuckerberg/shasta
[Flye-pmid]: https://pubmed.ncbi.nlm.nih.gov/30936562/
[da-pmid]: https://pubmed.ncbi.nlm.nih.gov/33288905/
[ss-pmid]: https://pubmed.ncbi.nlm.nih.gov/33288906/
[sh-pmid]: https://pubmed.ncbi.nlm.nih.gov/32686750/
[Falcon-pmid]: https://pubmed.ncbi.nlm.nih.gov/27749838/
[FP-preprint]: https://www.biorxiv.org/content/10.1101/327064v2
[CHM13-ont2]: https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel3/rel3.fastq.gz
[Wengen]: https://github.com/adigenova/wengan
[Wengan-pmid]: https://pubmed.ncbi.nlm.nih.gov/33318652/
[HG00733-clr]: https://www.ncbi.nlm.nih.gov/sra/?term=SRR7615963
[HG00733-hifi]: https://www.ebi.ac.uk/ena/data/view/ERX3831682
[HG00733-sr-pat]: https://www.ebi.ac.uk/ena/data/view/ERR3241754
[HG00733-sr-mat]: https://www.ebi.ac.uk/ena/data/view/ERR3241755
[HG00733-hic]: https://www.ncbi.nlm.nih.gov/sra/?term=SRR11347815
