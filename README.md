```
                         ..             ...... .
                     .:..:             ......:...   ...
                     =-..                     .     .:--.
                  .:-:               ..:--.    .::..::
                 :-                      .    ...:--::.      .
               .-:                               ..:::...    ::
              -*: ..                              ...  ..::-:..
             :#=. .                ...            .....:---=--.
           .--:.                   .              .:=+=-::::-:
          .+=                                  ...:. .::..-=-
          :+-        :-=-.       .......:      .:+=:  ..:--.
         .:.        .=+=-..:-=====-----.:.  :::--#@%+-:=+=:
         ...        .=+-::*+=**###*+==-:..::-=*%++@@@%****+:
           ..       :=+-.-*##%%%%%%####*+*+-::**#*@@@@@@#*++:
             .      -=+*+-:+#%%@@@%%%%%#*=:::=+##%@@@@@@@**+-.
               .   -+-::-:..:-+#%%%%%###*+++**#%@@@@@@@@@**+-:--.
               ..  ++-=+===-:::-=*#%@@%#*=--..-++*#@@@@@@*+%#@@%#.
                :: +*++=:-- ..=::-*%@@%#+-=+--+##*#%@@@@@**@@@@#@-
               -*=.=*+=. -+:-=+==-+#@@@%%#**#%%%@@@@@@@@@%#%#@@%#
               .+*+=*++===++****++*#%@@@@@@@%@@@@@@@@@@@@%#@#*@%.
                :+#=*****#####%##**#@@@@@@@@@@@@@@@@@@@@@**%%%@-
                  +++**###%%%%%##**%@@@@%@@@@@@@@@@@@@@@@+*@@@@
                   +-***##%%@@%##--*%@@#+%@%@@@@@@@@@@@%+=+#%#:
                   *-:#*##%%%%%#*+=:=*+#%@@@@@@@@@@@@%*+==*.
                   .: -*###%%%%#*:  .. ..=**+*@@@@@%*+=-=-#=
                       :=*##*-:....:-=+--=:.  -#%#*=------%#
                         :==.   ::-+*##%%%#*+. -+=--:::-:=@@
                               =+++****#%@@@#:  --::....:*@@:   .
                               :+***=:.:*#%#:    .:.   :*@@@+   .:.
                                .-=++=:.:==-.    ..   :*%@@@+   ....
                                  ..:........ .     .=#%%@%%=   ......
                                                  .=*%%%%%%*:   ........
                                               .-+*###%%%%*-    .....     .:..
                          .     ..        .::-++**###%%%#*-    ......        .....
                        ..       ---:::::-=++++**######*+-     .....
                        .          --------==+++***####*+-     ...
                 :.   .           .-====-==+++++*****++-      ...
            .  ...   .             .-=+++++++++++*++++=      ..
        ...        ..             .:::=+*****+++**++*+
     .:..         .               .----=*###******#*-
  ....                             -++==*#%##***##=
::.                                .**##*####**#+.
                                    :#######***-
                                     =#####*#*.
                                      +*#**#=
                                      .****-
                                       -+=.
                                        :
```

# Muhammed Murshid KP

**Bioinformatics Engineer** · NGS pipelines · Clinical & computational genomics · Structural bioinformatics · Software engineering

> Life is written in variation: a single base, a gene, a pathway, a whole community.

I build the pipelines and the software underneath them: clinical WES/WGS, genome assembly, metagenomics and polygenic risk scoring. At Decipher Genomics & Research (Ahmedabad) I'm the primary pipeline architect across clinical, microbial and population-scale genomics projects. Outside client work I write open-source tools, ship interactive genomics software, and do structural research with roots in molecular dynamics and drug discovery.

[kpmurshid.in](https://kpmurshid.in) · [Portfolio](https://kpmurshid.in/portfolio) · [Tools](https://kpmurshid.in/tools) · [Genomics Arena](https://kpmurshid.in/arena) · [Blog](https://kpmurshid.in/blog)

---

## Featured work

### [vcfilt](https://github.com/Kpmurshid/vcfilt): zero-allocation VCF filter in Go
- ~147,000 variants/sec, 12.2x faster than bcftools on an 18 GB VCF (1.8M variants), with identical output
- 7.9x faster on gzip-compressed input; I/O-bound even at one thread, with the speedup holding from 1 to 48 threads
- Zero heap allocations in the hot path, verified with `go test -benchmem`
- Static binary, Docker and Singularity images, MIT licensed
- bioRxiv preprint (April 2026): [10.64898/2026.04.14.718370](https://doi.org/10.64898/2026.04.14.718370) · Software DOI: [10.5281/zenodo.19548662](https://doi.org/10.5281/zenodo.19548662)
- Write-up: [Why I Built a Faster VCF Filter](https://kpmurshid.in/blog/vcfilt-zero-allocation)

### [ClinVar Variant History](https://kpmurshid.in/tools/clinvar-history): live classification timeline
- Tracks how variant classifications change across monthly ClinVar releases for the 84-gene ACMG SF v3.3 panel (341,000+ variants)
- 7,869 classification changes across ten monthly snapshots, with a per-variant trajectory chart
- Most changes reflect ClinVar's aggregate label shifting as submissions arrive, not clinical reinterpretation, and the tool says so
- Next.js front end, Turso-hosted database
- Write-ups: [Tracking ClinVar Reclassifications](https://kpmurshid.in/blog/clinvar-reclassification-history) · [GLA Variants Are Getting a Second Look](https://kpmurshid.in/blog/clinvar-october-gla-update)

### [ASVFlow](https://github.com/Kpmurshid/ASVFlow): paired-end 16S amplicon pipeline
- Modular Nextflow DSL2: QC, optional Cutadapt primer trimming, DADA2 ASV inference
- Optional SILVA taxonomy, alpha/beta diversity, PERMANOVA, and MAFFT/FastTree phylogeny with UniFrac
- Interactive Streamlit dashboard, Apptainer/Singularity containers, MIT licensed, `v1.0.0`
- [Setup and usage guide](https://kpmurshid.in/tools/asvflow)

---

## What I work on

- **Clinical genomics:** WES/WGS germline (trio-aware) and somatic pipelines with SNV/indel (GATK4, DeepVariant), CNV (CNVkit) and SV (Manta) calling; a Python ACMG/AMP classification engine (ClinGen/SVI 2023, HPO/GADO prioritization) with automated PDF/HTML reports
- **Genome assembly & annotation:** de novo bacterial and yeast assembly with decontamination, annotation, AMR profiling (RGI/CARD) and SSR discovery; species identification checks with fastANI
- **Metagenomics & transcriptomics:** 16S profiling (QIIME2/DADA2), shotgun profiling (Kraken2/Bracken, HUMAnN3, MetaWRAP), RNA-seq with DESeq2/edgeR
- **Polygenic risk scores:** a 43-trait PRS platform with GWAS ingestion, allele harmonization and cross-trait normalization on a SQLite variant database
- **QC & tooling:** sequencing QC pipelines with a live dashboard that tracks yield against client requirements
- **Structural bioinformatics:** folding MD with PCA, clustering and autoencoders; protein-ligand docking (AutoDock Vina, RDKit) with GROMACS MD analysis; mutation impact with FoldX
- **AI/ML for biology:** feature engineering, dimensionality reduction, and classification of MD and variant data

---

## Engineering practices

- Modular, reproducible Nextflow DSL2 pipelines
- HPC processing with SLURM
- Containerized workflows with Docker and Singularity/Apptainer
- Go, Python, R, Bash and TypeScript for tooling, analysis and web
- Git-based development, versioned releases, and benchmarked claims

---

## Stack

**Languages** Go · Python · R · Bash · TypeScript
**Workflow & systems** Nextflow · SLURM · Docker · Singularity/Apptainer · Linux · Git
**NGS / genomics** BWA-MEM2 · GATK4 · DeepVariant · bcftools · samtools · VEP · SnpEff · CNVkit · Manta · AnnotSV · mosdepth · fastp · FastQC · MultiQC
**RNA-seq** STAR · HISAT2 · Salmon · Kallisto · featureCounts · DESeq2 · edgeR
**Metagenomics & assembly** QIIME2 · DADA2 · Kraken2 · HUMAnN3 · MetaWRAP · SPAdes · Prokka · BRAKER3 · eggNOG-mapper · InterProScan
**Structural biology** GROMACS · AutoDock Vina · RDKit · PyMOL · FoldX
**Data / ML** pandas · numpy · scikit-learn · TensorFlow · Keras
**Web / data** Next.js · Tailwind CSS · SQLite / libSQL · Streamlit

---

## Experience

- **Bioinformatic Analyst**, Decipher Genomics & Research, Ahmedabad (Sep 2025 to present)
- **Research Assistant, Computational Drug Discovery**, Telscie Genetics (Feb 2025 to Aug 2025)
- **Research Scholar, Structural Bioinformatics**, CCS Haryana Agricultural University (Jan 2023 to Dec 2024): contributed to a published study on protein energy landscapes
- **Bioinformatics Intern**, Loncure Pvt Ltd (Sep 2024 to Oct 2024)

**Education:** MSc Bioinformatics, CCS Haryana Agricultural University, Hisar · BSc Forestry, SKUAST-K, Srinagar

---

## Currently

- Building and hardening clinical WES germline and somatic pipelines
- Developing ACMG-aligned variant interpretation and reporting workflows
- Growing the nutrigenomics and predictive PRS platforms
- Maintaining vcfilt and ASVFlow, and publishing monthly ClinVar updates
- Shipping interactive genomics tools on [kpmurshid.in](https://kpmurshid.in)
- Applying AI/ML to mutation impact and protein-ligand interaction analysis
- Integrating multi-omics and structural data for predictive insights

Open to collaboration on genomics pipelines and tooling.

---

## Connect

[Website](https://kpmurshid.in) · [LinkedIn](https://www.linkedin.com/in/kpmurshid) · [Email](mailto:murshidcherooth@gmail.com)
