# DEanalysis

# Description:
Performs a complete DESeq2-based RNA-seq differential gene expression (DE) analysis pipeline in R. Use this skill whenever the user wants to: run DESeq2 DE analysis, analyze RNA-seq count data, compare gene expression between conditions/groups, perform PCA on RNA-seq data, make volcano plots from DE results, cluster differentially expressed genes (time-course or multi-group clustering with TCseq), or generate heatmaps of DE gene expression patterns. Also trigger this skill when the user mentions volcano, heatmap, or TCseq clustering in any RNA-seq context. Always use this skill for any multi-step RNA-seq workflow even if only one step is mentioned — the user likely needs the full pipeline.  The raw counts should use the gene id and this script will added gene name based on the gtf file.

# DESeq2 Differential Expression Analysis Pipeline

## pipeline overview 

1. preprocess: Raw counts → DESeq2 → VST normalization → PCA
2. Pairwise DE comparisons → Volcano plots → Sig. DE genes  → Heatmap
3. TCseq clustering (if k > 2) → Heatmap

### Step 1: Setup and Data Loading
#### Required Libraries
#### Define Groups and Replicates
#### Read GTF for Gene Annotation
#### Build Sample Table and Load HTSeq Counts

### Step 2: Filtering, Normalization, and DESeq2 Fitting

### Step 3: PCA Plot

### Step 4: Pairwise DE Comparisons and Volcano Plots
#### Pairwise DE (each treatment vs. base)
#### Volcano Plots

### Step 5: Extract Significant DE Genes

### Step 6: Time-Course Clustering with TCseq (only when k > 2)
#### run TCseq
#### Reorder Clusters by Expression Trajectory

#### Step 7: Heatmap of DE Gene Patterns
##### Option A — Ordered by TCseq Cluster (use after Step 6)
##### Option B — Hierarchical Clustering Heatmap with Cut-Tree






