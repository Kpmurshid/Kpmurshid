## Hi there 👋

# I'm Muhammed Murshid KP

**Bioinformatics Engineer | NGS Pipeline Development | Clinical & Computational Genomics | Structural Bioinformatics | Software Engineering**

I build the pipelines and tools that turn raw sequencing data into interpretable results. At **Decipher Genomics & Research** (Ahmedabad), I'm the primary pipeline architect across clinical, microbial, and population-scale genomics projects. Outside client work, I write open-source software and do structural and computational research, with roots in molecular dynamics and drug discovery.

🌐 **Website:** [kpmurshid.in](https://kpmurshid.in) | 📝 **Blog:** [kpmurshid.in/blog](https://kpmurshid.in/blog) | 🗂️ **Portfolio:** [kpmurshid.in/portfolio](https://kpmurshid.in/portfolio) | 🧰 **Tools:** [kpmurshid.in/tools](https://kpmurshid.in/tools)

---

### 🚀 Featured Project

**[vcfilt](https://github.com/Kpmurshid/vcfilt)** is a zero-allocation streaming VCF filter written in Go.

* Processes ~**147,000 variants/sec**, **12.2x faster than bcftools** on an 18 GB VCF (1.8M variants)
* Zero heap allocations in the hot path (verified with `go test -benchmem`)
* I/O-bound even at a single thread; the speedup holds from 1 to 48 threads
* Preprint on bioRxiv (April 2026): [10.64898/2026.04.14.718370](https://doi.org/10.64898/2026.04.14.718370)
* Write-up on the blog: how the zero-allocation design works, with benchmarks

---

### 🧰 Tools on the Site

* **ClinVar Variant History** *(in progress)*: search a gene or variant and see how its classification changed over time (e.g. VUS → Likely Pathogenic → Pathogenic), bounded to the ACMG SF v3.3 gene panel (84 genes). Built with Next.js, with a Turso-hosted database updated from monthly ClinVar snapshots.

More tools are planned. Check [kpmurshid.in/tools](https://kpmurshid.in/tools) for updates.

---

### 🔬 What I Work On

* **Clinical genomics**: WES/WGS germline (including trio/family) and somatic pipelines, variant filtering, annotation, and ACMG/AMP-aligned interpretation
* **Genome assembly & annotation**: de novo bacterial and eukaryotic (yeast) assembly, reference-based bacterial WGS
* **Metagenomics**: 16S/ITS amplicon profiling, shotgun taxonomic and functional workflows
* **Transcriptomics**: RNA-seq alignment, quantification, and differential expression
* **Polygenic risk scores**: PRS platform for nutrigenomics reporting
* **QC & tooling**: Sanger sequencing QC, fastp-based QC pipelines with a live tracking dashboard
* **Structural bioinformatics**: protein–ligand docking, MD trajectory analysis (RMSD, Rg, H-bonds, distance matrices), mutation impact with structural and energy-based methods
* **AI/ML for biology**: feature engineering, dimensionality reduction, classification models

---

### 💼 Experience

* **Bioinformatic Analyst**, Decipher Genomics & Research, Ahmedabad (Sep 2025 – present)
* **Research Assistant, Computational Drug Discovery**, Telscie Genetics (protein–ligand docking, GROMACS MD)
* **Research Scholar, Structural Bioinformatics**, CCS Haryana Agricultural University (protein folding MD; contributed to a published study on protein energy landscapes)
* **Bioinformatics Intern**, Loncure Pvt Ltd

**Education:** MSc Bioinformatics, CCS Haryana Agricultural University | BSc, SKUAST-K, Srinagar Kashmir

---

### ⚙️ Engineering Practices

* Nextflow DSL2 pipelines, modular and reproducible
* HPC processing with SLURM
* Containerized workflows with Docker and Singularity
* Go, Python, R, and Bash for tooling and analysis
* Git-based development and collaboration

---

### 🛠️ Tools & Technologies

**Languages**
Go, Python, R, Bash, TypeScript

**Data / ML**
pandas, numpy, scikit-learn, TensorFlow, Keras

**NGS / Genomics**
BWA-MEM2, SPAdes, samtools, bcftools, GATK, VEP, SnpEff, CNVkit, DeepVariant, AnnotSV, Manta, mosdepth, CAPICE, fastp

**RNA-seq**
HISAT2, STAR, featureCounts, HTSeq, DESeq2

**Metagenomics**
QIIME2, DADA2, Kraken2, MetaPhlAn, Prokka, eggNOG-mapper, dbCAN, Prodigal, GraftM

**Structural Biology**
GROMACS, PyMOL, FoldX / PyFoldX

**Web / Data**
Next.js, Tailwind CSS, SQLite / libSQL

**Workflow & Systems**
Nextflow, SLURM, Docker, Singularity, Linux, Git, SSH

---

### 🎯 Current Direction

* Building ACMG-aligned variant interpretation workflows
* Developing fast, reproducible CLI tools for genomics (vcfilt and beyond)
* Shipping interactive genomics tools on [kpmurshid.in](https://kpmurshid.in)
* Applying AI/ML to mutation impact and protein–ligand interaction analysis
* Integrating multi-omics and structural data for predictive insights

---

### 🤝 Connect

[Website](https://kpmurshid.in) | [LinkedIn](https://www.linkedin.com/in/kpmurshid) | [GitHub](https://github.com/Kpmurshid) | [Email](mailto:murshidcherooth@gmail.com)
