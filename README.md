# Metabolic-Model-of-Pseudomonas-putida-KT2440
Pseudomonas putida KT2440 is a versatile bacterium known for its ability to degrade aromatic compounds, produce organic acids, and contribute to bioremediation processes. This Metabolic Model (GEM) for P. putida KT2440 is aimed at simulating the metabolic behavior of this bacterium to understand its metabolic network and optimize it for biotechnological applications such as biofuel production, biodegradation, and industrial chemical synthesis.

Model Documentation: [PPU_Model](https://1drv.ms/x/c/82e11bf00f8ea8cf/EVeHvyZ0z2ZHvUd4_58L0dABH9neKiB0Peu-2xDo1CZh2w?e=dWcDdJ)
## Model Description:
This model represents the metabolic network of Pseudomonas putida KT2440 with a focus on carbon metabolism. 

**Objective Function**: Acetyl-CoA carboxylase

**Biological Compartments** : The model is structured to include key compartments to reflect cellular organization and facilitate the distribution of metabolic fluxes:

* Cytoplasm (c)
* Extracellular (e)
  
**Reactions and Metabolites**:
The model encompasses ***147*** reactions and ***108*** metabolites, covering pathways such as:

Central Carbon Metabolism: Glycolysis, TCA cycle, pentose phosphate pathway.\
Nitrogen Metabolism: Nitrogen fixation.\
Oxidative Phosphorylation 

## Data Sources, Tools, and Databases:
KEGG: Kyoto Encyclopedia of Genes and Genomes.\
BiGG Models: Biochemical Genetic Network Models for metabolic networks.\
UNIPROT: Protein sequence and function database.\
COBRApy: Python library for Constraint-Based Optimization.

### Constraints and Assumptions:
Objective Function: The model is built with acetyl-CoA carboxylase as an objective function. Alternative objectives include organic acid production (e.g., succinate, acetate) for biotechnological applications.

## Constraints:

Oxygen uptake and nutrient availability (e.g., glucose, nitrogen, phosphorus) are constrained based on typical growth conditions.
Substrate limitations (carbon sources, nitrogen, etc.) to simulate specific industrial conditions or media.

## Model Construction and Curation:
The Pseudomonas putida KT2440 Metabolic model was constructed using gene annotations, metabolic pathways, and biochemical data sourced from publicly available databases. The curation steps include:

**Extraction and Validation of Reactions**: Reactions were extracted from KEGG and BiGG databases and validated against the genome sequence of P. putida KT2440 from NCBI.

**Filling Gaps**: 

**Stoichiometric Consistency Checks**: Quality control measures were applied to ensure that the model is stoichiometrically and charge-balanced.\
Curation Steps: 

Extracted reactions: From KEGG, BiGG. 
Validation and gap-filling: Added missing reactions for known pathways. 
Quality checks: Ensured that the reactions followed mass and charge balance.

## Simulation Protocols:
The model can be used for a variety of metabolic simulations, including:

**Flux Balance Analysis (FBA)**: To predict optimal flux distributions under different conditions, such as nutrient availability or changes in media composition.<br/>
**Gene Knockout Analysis**: To simulate the impact of gene deletions or knockouts on metabolism, and identify potential targets for metabolic engineering or synthetic biology.

## Results and Findings (Preliminary Simulations):
Preliminary FBA simulations have shown that P. putida KT2440 has a high Malonyl-CoA yield when grown on glucose, with optimized pathways for carbon source assimilation.<br/>

## Check the PPU_Analysis file for more information.##

## Limitations and Future Work:
### Limitations:
* Incomplete Genome Annotation: Some pathways may still lack detailed annotation due to incomplete genome data.
  
* Simplified Assumptions: Some assumptions, such as reaction constraints and compartmentalization, may limit the model's accuracy in simulating complex physiological conditions.

* Simplified Transport Reactions: Errors or omissions in transport reactions can misrepresent metabolite exchange across compartments. Some transporters may have been assigned incorrect stoichiometry or directionality, affecting intracellular flux distributions. Lack of explicit transport mechanisms for cofactors (e.g., NADH, ATP) may lead to unrealistic energy balance.

* Assumptions in Reaction Constraints: Some reactions may have been constrained arbitrarily, which could lead to inaccurate flux predictions. Reversibility constraints may not reflect physiological reality, impacting metabolic feasibility.

### Future Work:
Pathway Refinement: Future work will focus on refining the aromatic degradation, Fatty Acid and organic acid production pathways.
Incorporation of Regulatory Elements: The addition of regulatory mechanisms for better simulation of metabolic control in response to environmental cues.

References:\
KEGG: Kyoto Encyclopedia of Genes and Genomes - Pseudomonas putida pathways.<br/> 
BiGG Models: Biochemical Genetic Network Models for metabolic networks.<br/>
UNIPROT: Protein sequence and function data for Pseudomonas putida.<br/>
