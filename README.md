In Silico Design of a Multi-Epitope Vaccine for Group A Streptococcus (GAS)
📖 Overview
This project details a comprehensive in silico approach to designing a novel multi-epitope vaccine (MEV) against Group A Streptococcus (GAS), the bacterium responsible for a wide range of human diseases, from common strep throat to life-threatening conditions like necrotizing fasciitis and streptococcal toxic shock syndrome (STSS). Given the significant global health burden of GAS and the current lack of an effective vaccine, this research leverages bioinformatics and immunoinformatics tools to develop a promising vaccine candidate.

The core of this project was to identify highly immunogenic epitopes from key GAS virulence factors (M protein and FbaA protein) and construct a chimeric vaccine that could elicit a robust and specific immune response. The entire process, from protein selection to final validation, was conducted computationally.

🛠️ Methodology & Workflow
The vaccine design followed a structured bioinformatics pipeline, utilizing a suite of specialized web servers and software.

Protein Identification & Retrieval: Target protein sequences (M protein, FbaA protein) were identified from literature and retrieved from the NCBI and UniProt databases.

Epitope Prediction: The Immune Epitope Database (IEDB) was used to predict potential B-cell and T-cell (CTL and HTL) epitopes.

Immunogenicity Screening: Predicted epitopes were rigorously screened for antigenicity (VaxiJen v2.0), allergenicity (AllerTOP 2.0), toxicity (ToxinPred), and their ability to induce IFN-γ.

Vaccine Construction: The most promising non-toxic, non-allergenic, and highly antigenic epitopes were selected. They were linked together using AAY and GPGPG linkers to form a multi-epitope chain. A 50S ribosomal protein adjuvant was added at the N-terminus with an EAAAK linker to enhance the immune response.

Physicochemical & Structural Analysis:

Properties: The vaccine's molecular weight, theoretical pI, stability, and solubility were analyzed using ProtParam and SOLUprot.

Structure Prediction: The secondary structure was predicted with PSIPRED, and the 3D tertiary structure was modeled using the Robetta server.

Validation: The quality of the 3D model was validated using a Ramachandran plot analysis via MOLPROBITY.

Molecular Docking: The HADDOCK server was used to perform protein-protein docking between the vaccine construct and key immune receptors (TLR4, MHC-I, and MHC-II) to evaluate binding affinity and interaction.

Immune Simulation: The C-ImmSim server simulated the immune response to the vaccine over time, predicting the generation of antibodies, T-cell populations, and cytokine levels.

In Silico Cloning: Finally, the vaccine's amino acid sequence was reverse-translated, and its codons were optimized for expression in an E. coli (K12) system using the JCAT server. The optimized gene was then inserted into a pET-28a(+) expression vector using SnapGene.

📊 Key Results & Visuals
1. Final Vaccine Construct

A chimeric protein was designed, consisting of an adjuvant, CTL epitopes, and HTL epitopes joined by specific linkers to ensure proper folding and presentation.

2. 3D Structure & Validation

The tertiary structure of the vaccine was modeled and validated to be of high quality, with 94.16% of its residues in the Ramachandran favored region.

3. Molecular Docking with Immune Receptors

The vaccine construct showed strong and stable binding interactions with TLR4, MHC-I, and MHC-II, suggesting it can be effectively recognized by the immune system.

MEV docked with TLR-4

MEV docked with MHC-I

MEV docked with MHC-II







4. Immune Simulation

In silico simulation predicted a robust immune response following vaccination, characterized by high levels of antibodies (IgG1, IgG2, IgM), a strong memory B-cell and T-cell response, and elevated levels of key cytokines like IFN-γ.

5. In Silico Cloning

The optimized gene for the vaccine construct was successfully cloned into the pET28a(+) expression vector, demonstrating the feasibility of its production in a lab setting.

🔬 Conclusion & Future Scope
This project successfully designed a promising multi-epitope vaccine candidate against Group A Streptococcus using a robust in silico pipeline. The designed vaccine demonstrated excellent antigenic properties, structural stability, and the potential to elicit a strong, long-lasting immune response.

Future work would involve synthesizing the vaccine for in vitro and in vivo studies to experimentally validate its safety and efficacy in animal models, which is a critical next step toward clinical trials.

👨‍💻 Author
Rakesh Kumar A

