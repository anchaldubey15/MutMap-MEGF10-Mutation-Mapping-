# MEGF10 Bioinformatics Analysis  

---

## ⚙️ Tools & Libraries  

### Databases & Web Tools  
- **NCBI** – Sequence retrieval  
- **UniProt** – Protein data (Q96KG7)  
- **BLASTp** – Similarity search  
- **Clustal Omega** – Multiple sequence alignment  
- **Jalview** – Visualization of conservation scores  
- **MEGA** – Phylogenetic tree construction  

### Python Libraries  
- `biopython` – Sequence parsing, phylogenetics  
- `pandas` – Variant data handling  
- `requests` – API queries  
- `collections` – Efficient data structures  
- `matplotlib` – Data visualization  

---

## 🧬 Bioinformatics Pipeline  

![Pipeline](https://github.com/anchaldubey15/MutMap-MEGF10-Mutation-Mapping-/blob/main/Bio_info_pipeline.png)  

**Steps:**  
1. Sequence retrieval (NCBI, UniProt)  
2. BLASTp analysis  
3. Multiple sequence alignment (Clustal Omega)  
4. Conservation scoring (Jalview)  
5. Phylogenetic tree construction (MEGA)  
6. Python-based variant and mutation analysis (Biopython + Pandas)  

---

## 📊 Key Results  

### 1. Multiple Sequence Alignment (MSA)  

![Jalview](https://github.com/anchaldubey15/MutMap-MEGF10-Mutation-Mapping-/blob/main/JalView_results.png)  

- Conserved cysteine motifs critical for **EGF domain stability**.  
- Strong conservation in residues **200–800 aa** (extracellular EGF repeats).  
- Divergence at N-terminal and C-terminal regions suggests species-specific adaptations.  

---

### 2. Phylogenetic Tree  

![Phylogenetic Tree](https://github.com/anchaldubey15/MutMap-MEGF10-Mutation-Mapping-/blob/main/Phylogentic_Tree.png)  

- Mammals (human, mole-rat, sheep) show **highest conservation** with human MEGF10.  
- Birds and reptiles form distant clusters.  
- Amphibians diverge further, highlighting evolutionary conservation but limited therapeutic modeling value.  

---

### 3. Mutation Mapping (ClinVar + PROSITE Domains)  

![Mutation Map 1](https://github.com/anchaldubey15/MutMap-MEGF10-Mutation-Mapping-/blob/main/Mutation_map_1.png)  
![Mutation Map 2](https://github.com/anchaldubey15/MutMap-MEGF10-Mutation-Mapping-/blob/main/Mutation_map_2.png)  

- **Pathogenic/likely pathogenic variants cluster within EGF-like repeats (100–830 aa)**.  
- Cysteine-rich motifs are mutational “hotspots” → folding disruption.  
- **EMI domain (30–107 aa):** mixed tolerance.  
- **Cytoplasmic tail (>850 aa):** mostly **VUS (variants of uncertain significance)**.  
- Suggests **extracellular domain failure** is central to EMARDD pathogenesis.  

---

## 📌 Interpretation  

- **EGF-like repeats = Achilles heel** → pathogenic mutations disrupt disulfide bonding.  
- **Therapeutic strategies**:  
  - *Truncating mutations*: gene replacement / mRNA therapy / read-through drugs.  
  - *Missense cysteine mutations*: pharmacological chaperones or CRISPR-based correction.  
- **Patient stratification**: prioritize those with EGF-domain loss-of-function variants for trials.  
- Many **tail-region VUS** likely benign → deprioritize for immediate therapeutic targeting.  

---

## 🐍 Python Analysis  

The **Python notebook (`Python_analysis.ipynb`)** integrates mutation data, domain structure, and ClinVar annotations.  

Key features:  
- Parsing ClinVar + UniProt variant files  
- Mapping mutations onto **PROSITE domains**  
- Visualization of mutation clustering  
- Data-driven insights into **disease mechanisms**  

---

## 📖 References  

- [NCBI Gene – MEGF10](https://www.ncbi.nlm.nih.gov/gene/84466)  
- [UniProt – MEGF10](https://www.uniprot.org/uniprotkb/Q8TE58/entry)  
- [OMIM – MEGF10](https://www.omim.org/entry/611194)  
- [Human Protein Atlas](https://www.proteinatlas.org/ENSG00000164161-MEGF10/tissue)  
- [GTEx Portal](https://gtexportal.org/home/gene/MEGF10)  
- [InterPro Domain Structure](https://www.ebi.ac.uk/interpro/entry/UniProt/Q8TE58/)  


## 📂 Repository Structure  

```bash
├── files/                        # Project files
│   ├── Project_report.pdf         # Comprehensive report (literature + analysis)
│   ├── MEGF10_variants_domains.csv
│   ├── Python_analysis.ipynb      # Biopython & Pandas analysis
│   ├── MEGF10_uniprot_data.txt
│   ├── Prosite_results_summary.txt
│
├── data/                         # Input & raw bioinformatics data
│   ├── MEGF10.fasta               # FASTA sequence (protein + nucleotide)
│   ├── BLAST_results.txt
│   ├── ClustalOmega_alignment.aln
│   ├── ClinVar_results.csv
│
├── results_images/               # Outputs & figures
│   ├── Bioinformatics_Pipeline.png
│   ├── JalView_results.png
│   ├── Phylogenetic_Tree.png
│   ├── Mutation_map_1.png
│   ├── Mutation_map_2.png
│
└── README.md                     # This file

## 👩‍🔬 Author

**Anchal Dubey**  
MSc Biotechnology  
This project was developed as part of a bioinformatics learning module on Biopython in bioinformatics.
---

