# Heading 1 🧬 Multi-Epitope Vaccine Design Against Group A Streptococcus (GAS)

The research paper is live at https://rakesh-kumar-a.github.io/Insilico-design-of-GAS-Vaccine/

This repository presents a comprehensive in silico pipeline for the design, structural validation, and immunological characterization of a multi-epitope vaccine candidate targeting Group A Streptococcus (GAS).

Authors: Rakesh Kumar A

Department of Life Sciences, Garden City University, Bangalore, India

📄 Abstract
Group A Streptococcus (GAS) is a globally significant bacterial pathogen that causes a wide spectrum of diseases, yet no licensed vaccine is currently available. This project uses immunoinformatics, structural bioinformatics, and molecular simulation tools to construct and validate a multi-epitope vaccine targeting key GAS virulence factors. The final construct integrates:

Target Proteins: M protein and FbaA protein (UniProt IDs: P12379.1, Q93R11)

T-cell and B-cell epitopes (MHC-I, MHC-II, Linear)

Adjuvant: 50S ribosomal protein L7/L12 to enhance immunogenicity

Linkers: EAAAK, AAY, and GPGPG to ensure proper separation and presentation of epitopes

🔬 Methodology Overview
Step

Description

🎯 Target Protein

Accession: P12379.1, Q93R11 (GAS M protein & FbaA protein) <br> Retrieved from UniProt.

🧩 Epitope Prediction

MHC-I & MHC-II epitopes predicted using IEDB. Screened for immunogenicity, antigenicity, non-toxicity, and non-allergenicity.

🧱 Vaccine Construction

Sequence constructed using Adjuvant + CTL epitopes + HTL epitopes with appropriate linkers. Codon-optimized using JCat and cloned in silico into the pET28a(+) vector.

⚗️ Bioinformatics Analysis

ProtParam: Physicochemical properties. <br> PSIPRED: Secondary structure. <br> Robetta: Tertiary structure prediction. <br> MOLPROBITY: Structural validation.

🧬 Molecular Interactions

HADDOCK docking with: <br> • TLR4 (innate immunity) <br> • MHC-I (CD8+ T cell response) <br> • MHC-II (CD4+ T helper cell activation)

🧪 Immune Simulation

C-ImmSim: Predicted robust humoral and cellular responses, with increased memory T and B cells, key cytokines (IFN-γ), and antibody levels (IgM, IgG).

🧪 Final Construct (Summary)

Length - 601 amino acids

MW - 61.6 kDa

pI - 6.08

Instability Index - 31.72 (stable)

GRAVY - (-0.428) (hydrophilic)

🔬 Conclusion & Future Scope
This project successfully designed a promising multi-epitope vaccine candidate against Group A Streptococcus using a robust in silico pipeline. The designed vaccine demonstrated excellent antigenic properties, structural stability, and the potential to elicit a strong, long-lasting immune response.

Future work would involve synthesizing the vaccine for in vitro and in vivo studies to experimentally validate its safety and efficacy in animal models, which is a critical next step toward clinical trials.

