# Sequence Analysis Terminology

## Core File Formats
**FASTA (.fa / .fasta)**  
Sequence files containing DNA/RNA/protein. No quality scores.

**FASTQ (.fq / .fastq)**  
Raw sequencing reads with per-base quality scores.

**SAM (Sequence Alignment Map)**  
Text-based alignment format.

**BAM**  
Binary, compressed SAM.

**CRAM**  
Highly compressed alignment referencing FASTA.

**VCF (Variant Call Format)**  
Variant information (SNPs, indels, SVs).

**BCF**  
Binary compressed VCF.

**BED**  
Genomic interval format.

**GFF / GTF**  
Genome annotation formats.

**TSV / CSV**  
General tabular data formats.

---

## Sequencing Concepts
**Read** – A sequenced fragment of DNA or RNA.  
**Read length** – Number of bases in a read.  
**Paired-end (PE)** – Two reads per DNA fragment.  
**Single-end (SE)** – One read per fragment.  
**Coverage / Depth** – Average number of reads covering each base.  
**Insert size** – Distance between paired-end reads.  
**Barcode / Index** – Short sequences for sample identification.  
**UMI (Unique Molecular Identifier)** – Tags for deduplication.  
**Adapter** – Technical sequence attached during library prep.

---

## Preprocessing & Quality Control
**QC (Quality Control)** – Assess read quality.  
**Trimming** – Remove adapters or low-quality bases.  
**Filtering** – Remove reads based on quality or length.  
**Deduplication** – Remove PCR duplicates.

---

## Mapping & Alignment
**Alignment / Mapping** – Positioning reads on a reference genome.  
**Aligner** – Software for alignment (e.g., BWA, Bowtie2, STAR, Minimap2).  
**Reference genome** – Standard genome assembly.  
**Indexing** – Preparing reference for alignment.  
**CIGAR string** – Encodes match/mismatch/gap operations.  
**MAPQ (Mapping Quality)** – Confidence of alignment.

---

## Variant Calling & Genomics
**Variant caller** – Detects variants (e.g., GATK, FreeBayes).  
**SNP** – Single nucleotide polymorphism.  
**Indel** – Insertion or deletion.  
**CNV** – Copy number variation.  
**SV (Structural Variant)** – Large genomic changes.  
**Genotype (GT)** – Variant genotype per sample.  
**Depth (DP)** – Read depth supporting a variant.  
**Allele frequency (AF)** – Fraction of reads with alternate allele.

---

## RNA-seq Terms
**Transcriptome** – All RNA transcripts.  
**Gene counts** – Reads mapped to genes.  
**TPM / FPKM / RPKM** – Expression normalization.  
**Splice junction** – Boundary between exons.  
**Alignment-free quantification** – Tools like Salmon, Kallisto.  
**Differential Expression (DE)** – Comparing expression levels.

---

## Assembly Terminology
**De novo assembly** – Building a genome without a reference.  
**Contig** – Assembled continuous sequence.  
**Scaffold** – Linked contigs with possible gaps.  
**N50** – Metric for assembly contiguity.

---

## Pipeline & Workflow Terms
**Workflow / pipeline** – Set of processing steps.  
**Container** – Reproducible environment (Docker, Singularity).  
**Metadata** – Sample information.  
**Batch effect** – Technical variation between batches.  
**Normalization** – Adjusting data to reduce technical bias.

---

## Common Tools
**FastQC** – Read quality assessment.  
**MultiQC** – QC aggregation.  
**BWA / Bowtie2 / STAR / Minimap2** – Aligners.  
**SAMtools** – Work with SAM/BAM files.  
**Picard** – Duplicate marking and BAM utilities.  
**GATK** – Variant discovery toolkit.  
**BCFtools** – Variant file manipulation.  
**Bedtools** – Genome interval operations.  
**IGV** – Genome browser for visualization.

---

## Bioinformatics Concepts
**k-mer** – Subsequence of length k.  
**Error rate** – Base calling error frequency.  
**Bias** – Systematic effects (GC bias, PCR bias).  
**Batch correction** – Removing batch effects (e.g., ComBat).
