## 🧬 In Silico Design of a Multi-Epitope Vaccine for Group A Streptococcus (GAS)

This repository details the complete in silico research pipeline for designing, validating, and analyzing a novel multi-epitope subunit vaccine candidate against Group A Streptococcus (GAS), the cause of numerous human diseases.

**Author:** Rakesh Kumar A  
**Affiliation:** Department of Life Sciences, Garden City University, Bangalore, India

-----

### 📄 Live Research Paper

The full, interactive research paper is published online.

**[Live Research Paper](https://rakesh8050.github.io/Insilico-vaccine-for-Group-A-Streptococcus-GAS-Infection-/)** 

-----

# Interactive Report: In Silico Vaccine Design for Group A Streptococcus

This is a single-page interactive web application that serves as a concise, explorable version of a scientific report. Instead of a traditional document, this project transforms a complex research paper on the *in silico* design of a multi-epitope vaccine for Group A Streptococcus (GAS) into a dynamic and accessible experience.

The application allows you to explore key data visualizations, such as the vaccine's molecular blueprint, a sortable table of selected epitopes, and an interactive simulation of its immune response. This format is designed for a quick and engaging overview of the research findings.

You can view the live demo here:

**[Interactive Report](https://rakesh8050.github.io/Insilico-vaccine-for-Group-A-Streptococcus-GAS-Infection-/vaccine-explorer.html)**

-----

### 1\. Abstract

Group A Streptococcus (GAS), or *Streptococcus pyogenes*, is a major human pathogen responsible for a wide spectrum of diseases, from common pharyngitis to life-threatening conditions like necrotizing fasciitis and streptococcal toxic shock syndrome (STSS), which carries a mortality rate exceeding 35%. Despite its global impact, **no licensed vaccine is currently available**.

This research leverages a comprehensive pipeline of immunoinformatics, structural bioinformatics, and molecular simulation tools to design and validate a chimeric, multi-epitope vaccine. The vaccine targets key GAS virulence factors—**M protein** and **Fibronectin-Binding Protein A (FbaA)**—by integrating predicted B-cell and T-cell epitopes with a potent adjuvant. The final construct was rigorously validated for its physicochemical properties, structural integrity, and its potential to elicit a robust and lasting immune response through molecular docking and in silico immune simulations.

-----

### 2\. Methodology

The project followed a systematic in silico pipeline, from target identification to final validation.

#### Step 1: Target Protein Identification and Retrieval

  * **Target Proteins:** M protein and FbaA protein, key virulence factors in GAS.
  * **Database:** Protein sequences in FASTA format were retrieved from UniProt.
      * **M protein (UniProt ID):** P12379.1
      * **FbaA protein (UniProt ID):** Q93R11

#### Step 2: Epitope Prediction

  * **Tool:** The Immune Epitope Database (IEDB) was used for prediction.
  * **T-Cell Epitopes:**
      * **Cytotoxic T-Lymphocyte (CTL/MHC-I):** 9-mer epitopes predicted to bind MHC-I alleles and activate CD8+ T-cells.
      * **Helper T-Lymphocyte (HTL/MHC-II):** 15-mer epitopes predicted to bind MHC-II alleles and activate CD4+ T-cells.
  * **B-Cell Epitopes:** Linear B-cell epitopes were predicted to stimulate humoral immunity.

#### Step 3: Immunoinformatics Screening

All predicted epitopes were filtered based on the following criteria:

  * **Antigenicity:** VaxiJen v2.0 (threshold \> 0.4).
  * **Allergenicity:** AllerTOP v2.0 (predicted as non-allergen).
  * **Toxicity:** ToxinPred (predicted as non-toxin).
  * **Interferon-γ Induction:** IFNepitope server (selected IFN-γ positive epitopes).

#### Step 4: Multi-Epitope Vaccine Construction

The final vaccine was constructed by combining the best-performing epitopes.

  * **Adjuvant:** 50S ribosomal protein L7/L12 was added to the N-terminus to enhance the immune response.
  * **Linkers:**
      * **EAAAK:** A rigid linker connecting the adjuvant to the first epitope.
      * **AAY:** Used to connect CTL epitopes.
      * **GPGPG:** Used to connect HTL epitopes, providing flexibility.


#### Step 5: Physicochemical and Structural Analysis

  * **Physicochemical Properties:** Calculated using the ProtParam tool (Molecular Weight, pI, Instability Index, GRAVY).
  * **Solubility:** Predicted using the SOLUPROT server.
  * **Secondary Structure:** Predicted using the PSIPRED server.
  * **Tertiary (3D) Structure:** Modeled using the Robetta server.
  * **Structural Validation:** The 3D model was validated using MOLPROBITY to generate a Ramachandran plot and assess stereochemical quality.

#### Step 6: Molecular Docking

  * **Tool:** HADDOCK v2.2 server.
  * **Objective:** To assess the binding affinity and interaction of the vaccine construct with key immune receptors.
  * **Receptors:**
      * **Toll-Like Receptor 4 (TLR4):** For innate immune recognition.
      * **MHC-I (HLA-A\*02:01):** For CTL response.
      * **MHC-II (HLA-DRB1\*01:01):** For HTL response.

#### Step 7: Immune Simulation

  * **Tool:** C-ImmSim server.
  * **Objective:** To predict the in vivo immune response profile following vaccination.
  * **Simulation:** The server simulated the response over 350 days with three injection exposures, tracking immunoglobulin levels, T-cell and B-cell populations, and cytokine production.

#### Step 8: In Silico Cloning

  * **Codon Optimization:** The vaccine's amino acid sequence was reverse-translated and codon-optimized for expression in the *E. coli* (K12 strain) system using the JCat server.
  * **Cloning:** The optimized gene sequence was inserted into the pET28a(+) expression vector using SnapGene.

-----

### 3\. Key Results

#### Vaccine Construct Summary

  * **Length:** 601 amino acids
  * **Molecular Weight:** 61.6 kDa
  * **Theoretical pI:** 6.08
  * **Stability:** Stable (Instability Index: 31.72)
  * **Nature:** Hydrophilic (GRAVY score: -0.428)
  * **Thermostability:** High (Aliphatic Index: 62.33)
  * **Solubility:** Predicted to be soluble upon expression.

#### Structural Validation

The Ramachandran plot analysis showed that **94.16% of residues were in the most favored regions**, confirming a high-quality and stereochemically sound 3D model.


#### Molecular Docking

The vaccine construct demonstrated **strong and stable binding to all three immune receptors (TLR4, MHC-I, and MHC-II)**, characterized by numerous non-bonded contacts and hydrogen bonds. This indicates a high potential for effective immune recognition and presentation.


#### Immune Simulation

The simulation predicted a **robust immune response**, characterized by:

  * A strong primary response and the development of long-lasting memory.
  * High levels of immunoglobulins (IgG1, IgG2, IgM).
  * Sustained activation of B-cells, Helper T-cells, and Cytotoxic T-cells.
  * Significant production of key cytokines, especially IFN-γ.


#### In Silico Cloning

The vaccine gene was successfully optimized (CAI of 1.0, GC content of 51.30%) and cloned into the pET28a(+) vector, confirming its potential for high-level expression in a bacterial system.


-----

### 4\. Conclusion

This project successfully designed and validated a promising multi-epitope vaccine candidate against Group A Streptococcus using a robust in silico pipeline. The designed vaccine demonstrated excellent antigenic properties, structural stability, and the potential to elicit a strong, specific, and long-lasting immune response. These findings provide a strong foundation for its future experimental validation.

-----

### 5\. Future Scope

The next critical steps for this research involve moving from computational analysis to experimental validation:

  * **In Vitro Synthesis:** Synthesize the designed vaccine protein.
  * **Experimental Validation:** Conduct in vitro and in vivo studies in animal models to confirm its safety, immunogenicity, and protective efficacy.
  * **Clinical Trials:** If successful, proceed to human clinical trials to establish it as a viable vaccine against GAS infections.

-----

### 6\. License

This project is licensed under the MIT License. See the LICENSE file for details.
