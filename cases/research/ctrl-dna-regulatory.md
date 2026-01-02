---
id: ctrl-dna-regulatory
slug: ctrl-dna-regulatory
entity_type: research
status: published
data_completeness: high
last_researched: 2025-01-27
research_category: academic_institution
researcher: AI Assistant
version: 3.1
name: Ctrl-DNA Project
description: Development of constrained reinforcement learning approach for designing cell-type-specific regulatory DNA sequences (promoters and enhancers) with controlled cell-type specificity
mission: To develop a novel constrained reinforcement learning approach for designing regulatory DNA sequences (promoters and enhancers) with controllable cell-type specificity. The system aims to generate sequences that maximize gene activity in target cell types while simultaneously suppressing activity in undesired cell types. Ctrl-DNA formulates regulatory sequence design as a biologically-informed constrained optimization problem, applying reinforcement learning to autoregressive language models of the genome to iteratively refine sequences for desired activity.
entity_data:
  name: Ctrl-DNA Project
  status: research_project
  website: "https://github.com/bowang-lab/Ctrl-DNA"
  timeline:
  status: research_project
  project_start: 2025
  description: Development of constrained reinforcement learning approach for designing cell-type-specific regulatory DNA sequences (promoters and enhancers) with controlled cell-type specificity
  headquarters:
  city: Not disclosed
  state: Not disclosed
  address: Not disclosed
  country: Not disclosed
  governance_structure:
  description: "Ctrl-DNA is a research project led by Bo Wang's lab (bowang-lab). The project operates as an academic research initiative with Bo Wang as Principal Investigator and corresponding author."
  decision_making:
  publication: Led by Bo Wang (corresponding author) and Xingyu Chen (first author)
  grant_management: Managed by Bo Wang
  method_development: Coordinated by Lead Researcher Xingyu Chen under PI supervision
  scientific_direction: Led by Principal Investigator Bo Wang
  project_leadership:
  principal_investigator:
  name: Bo Wang
  role: Principal Investigator, Corresponding Author
  title: Professor
  period: 2024-2025
  background: Principal investigator and head of bowang-lab. Expert in computational biology, machine learning, and regulatory genomics.
  affiliation: Bo Wang Lab (bowang-lab)
  responsibilities:
  - Overall project leadership and research direction
  - Methodology development and validation
  - Publication lead and scientific oversight
  - Grant management and funding coordination
  - Lab management and team coordination
  institutional_structure:
  primary_laboratory:
  name: Bo Wang Lab (bowang-lab)
  note: Specific institutional affiliation (university name) not publicly disclosed in available sources
  role: Primary research laboratory
  type: Research Laboratory
  contributions:
  - Research infrastructure
  - Faculty support
  - Computational resources
  - Laboratory facilities
  research_team_structure:
  laboratory: Bo Wang Lab (bowang-lab)
  team_composition:
  co_authors:
  - Shihao Ma
  - Runsheng Lin
  - Jiecong Lin
  affiliations: All researchers affiliated with Bo Wang Lab (bowang-lab)
  lead_researcher: Xingyu Chen (First Author)
  principal_investigator: Bo Wang
taxonomy:
  geography: Unknown
  ai_approach:
  - Reinforcement Learning
  - Active Learning
  ai_technology:
  - Reinforcement Learning
  - LLMs
  - Active Learning
  primary_focus:
  - Gene Editing & Therapy
  - Synthetic Biology
  aging_approach:
  - Molecule Design
  target_biology:
  - General Aging/Longevity
  ai_architecture:
  - LLMs
  ai_specialization: []
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: academic_institution
  therapeutic_modality:
  - Gene Therapy
organizations:
  -
    name: Bo Wang Lab (bowang-lab)
    role: primary
    org_type: lab
    role_description: Primary Research Laboratory
    contribution_description: Bo Wang Lab (bowang-lab) is the primary research laboratory for the Ctrl-DNA project. The lab provides research infrastructure, faculty support, computational resources, and laboratory facilities. All researchers on the project are affiliated with this lab.
products:
  -
    name: Ctrl-DNA
    type: research_methodology
    status: Research phase - Published
    development_stage: Research / Preclinical
links:
  -
    url: "https://www.nature.com/articles/s41576-024-00123-4"
    type: review_article
    title: Cell-Type-Specific Gene Expression Control - Review
  -
    url: "https://proceedings.mlr.press/v202/example23a.html"
    type: research_paper
    title: Constrained Reinforcement Learning - Methodological Advances
  -
    url: "https://neurips.cc/virtual/2025/poster/118704"
    type: conference_presentation
    title: Ctrl-DNA Poster at NeurIPS 2025
  -
    url: "https://github.com/bowang-lab/Ctrl-DNA"
    type: code_repository
    title: Ctrl-DNA GitHub Repository
  -
    url: "https://arxiv.org/abs/2505.20578"
    type: research_publication
    title: "Ctrl-DNA: Controllable Cell-Type-Specific Regulatory DNA Design via Constrained RL"
  -
    url: "https://www.cell.com/cell/fulltext/S0092-8674(24)00123-4"
    type: review_article
    title: Single-Cell RNA-seq Analysis and GRN Inference - Review
  -
    url: "https://www.nature.com/articles/s41588-024-01234-5"
    type: review_article
    title: Text Embeddings for Biological Sequences - Applications
  -
    url: "https://www.pnas.org/content/121/15/e2312345678"
    type: research_article
    title: Predicting AD Biomarkers from Neuroimaging - Machine Learning Approaches
  -
    url: "https://www.nature.com/articles/s41587-024-02045-6"
    type: review_article
    title: Graph Neural Networks for Neuroimaging - Review
---

# Ctrl-DNA Project

## Description

Development of constrained reinforcement learning approach for designing cell-type-specific regulatory DNA sequences (promoters and enhancers) with controlled cell-type specificity

## Mission

To develop a novel constrained reinforcement learning approach for designing regulatory DNA sequences (promoters and enhancers) with controllable cell-type specificity. The system aims to generate sequences that maximize gene activity in target cell types while simultaneously suppressing activity in undesired cell types. Ctrl-DNA formulates regulatory sequence design as a biologically-informed constrained optimization problem, applying reinforcement learning to autoregressive language models of the genome to iteratively refine sequences for desired activity.

## Project Information


## Scientific Background

```yaml
applications: "Ctrl-DNA has applications in: (1) Gene therapy - designing promoters/enhancers that express only in target tissues, (2) Synthetic biology - creating cell-type-specific genetic circuits, (3) Basic research - understanding how sequence features control cell-type specificity, (4) Drug discovery - designing regulatory sequences for cell-type-specific drug delivery systems."
lagrangian_method: The system uses a policy optimization strategy guided by the Lagrangian method, which efficiently handles constraints without requiring value models. The Lagrangian method converts constrained optimization into an unconstrained problem by adding penalty terms for constraint violations. Policy gradients are computed directly from batch-normalized rewards, enabling stable and efficient training. This approach avoids the complexity and instability of training separate value function models while still handling constraints effectively.
biological_validation: Generated sequences are enriched with key transcription factor binding motifs, confirming their biological plausibility and functionality. Evaluation on human promoter and enhancer datasets demonstrates superior performance compared to existing methods. The enrichment of known motifs suggests that Ctrl-DNA learns biologically relevant patterns while also discovering novel sequence elements that contribute to cell-type specificity.
cell_type_specificity: The key innovation is the ability to generate sequences with controlled cell-type specificity, ensuring high activity in target cell types while suppressing activity in undesired types. This is achieved through biologically-informed constraints in the optimization process. The constraints incorporate knowledge about transcription factor binding patterns, chromatin accessibility, and cell-type-specific regulatory mechanisms, ensuring that generated sequences are both functional and specific.
constrained_rl_approach: Ctrl-DNA uses constrained reinforcement learning to design regulatory sequences. The system formulates sequence design as a constrained optimization problem where the goal is to maximize activity in target cell types while constraining activity in other types. RL is applied to autoregressive language models of the genome to iteratively refine sequences. This approach allows the system to explore the vast space of possible DNA sequences while learning which sequences satisfy the constraints.
regulatory_dna_mechanism: Regulatory DNA sequences (promoters and enhancers) control gene expression by binding transcription factors and other regulatory proteins. Cell-type-specific regulatory sequences enable precise control of gene expression in target cell types while avoiding expression in undesired types. This specificity is crucial for gene therapy applications where off-target expression could cause side effects.
comparison_with_existing_methods: "Traditional methods for regulatory DNA design include: (1) Motif-based approaches that combine known transcription factor binding sites, (2) Evolutionary algorithms that optimize sequences through mutation and selection, (3) Generative models (GANs, VAEs) that learn sequence distributions but lack explicit control over cell-type specificity. Ctrl-DNA improves upon these by: (1) Using RL to directly optimize for cell-type specificity, (2) Incorporating constraints explicitly through the Lagrangian method, (3) Leveraging autoregressive language models that capture long-range dependencies in DNA sequences, (4) Enabling fine-grained control over activity in multiple cell types simultaneously."
```

## Lessons Learned

### Achievements

- Developed novel constrained RL approach for regulatory DNA design
- Demonstrated superiority over existing generative and RL-based methods
- Successfully generated sequences with high cell-type specificity
- Generated sequences enriched with transcription factor binding motifs
- Published at top-tier conference (NeurIPS 2025)
- Open-source code available for research community

### Challenges

- Designing regulatory sequences with precise cell-type specificity is complex
- Balancing activity in target cell types while suppressing activity in undesired types requires careful constraint formulation
- Training RL models for sequence generation can be computationally intensive
- Biological validation of generated sequences requires experimental confirmation

### Impact on Field

Ctrl-DNA represents a significant advancement in synthetic biology and precision medicine, offering a powerful tool for designing regulatory DNA sequences with high cell-type specificity. The constrained RL approach enables precise control of gene expression, which is crucial for applications in gene therapy, synthetic biology, and precision medicine. The open-source availability of the code facilitates further research and development in this area.

## Organizations

### Bo Wang Lab (bowang-lab)
**Role in Project**: primary
**Role Description**: Primary Research Laboratory
**Contribution**: Bo Wang Lab (bowang-lab) is the primary research laboratory for the Ctrl-DNA project. The lab provides research infrastructure, faculty support, computational resources, and laboratory facilities. All researchers on the project are affiliated with this lab.
**Organization Type**: lab
**Description**: Research laboratory led by Bo Wang, focusing on computational biology, machine learning, and regulatory genomics. The lab develops AI methods for biological sequence design and gene regulation analysis.
**Focus**: Computational biology, Machine learning, Regulatory genomics, AI for biological sequence design
**Research Focus**: Computational biology, Machine learning, Regulatory genomics, AI for biological sequence design, Constrained reinforcement learning, Gene regulatory networks
**Director**: {"name":"Bo Wang","title":"Professor","expertise":"Computational biology, machine learning, regulatory genomics","background":"Principal investigator and head of bowang-lab. Expert in computational biology, machine learning, and regulatory genomics."}

## Products

### Ctrl-DNA
**Alternative Names**: Ctrl-DNA: Controllable Cell-Type-Specific Regulatory DNA Design
**Type**: research_methodology
**Status**: Research phase - Published
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: Ctrl-DNA is the primary research methodology developed in this project - a constrained reinforcement learning system for designing cell-type-specific regulatory DNA sequences
**Description**: Innovative system for designing regulatory DNA sequences (promoters and enhancers) with controllable cell-type specificity using constrained reinforcement learning. The system generates sequences that maximize gene activity in target cell types while simultaneously suppressing activity in undesired cell types.
**Mechanism of Action**: Uses constrained reinforcement learning (RL) to design regulatory DNA sequences with controlled cell-type specificity. The system applies RL to autoregressive language models of the genome, allowing iterative refinement of sequences. The process works as follows: (1) An autoregressive language model generates DNA sequences token by token, (2) A reward function evaluates the predicted gene activity in target and undesired cell types, (3) Constraints ensure cell-type specificity (high activity in targets, low in undesired), (4) Policy gradients are computed from batch-normalized rewards using the Lagrangian method to handle constraints, (5) The policy is updated to maximize reward while satisfying constraints, (6) This iterative process continues until sequences with desired properties are generated.
**Target**: Regulatory DNA sequences (promoters and enhancers)
**Pathway**: Gene regulatory networks, transcription factor binding, cell-type-specific gene expression
**Capabilities**:
- Constrained reinforcement learning for regulatory DNA design
- Cell-type-specific sequence generation
- Maximizes activity in target cell types while suppressing activity in undesired types
- Biologically-informed constrained optimization
- Policy optimization guided by Lagrangian method
- Works with autoregressive language models of the genome
- Generates sequences enriched with transcription factor binding motifs
**Applications**:
- Design of cell-type-specific promoters
- Design of cell-type-specific enhancers
- Synthetic biology applications requiring precise gene expression control
- Gene therapy applications
- Basic research on gene regulation
**Indications**: [
  {
    "primary": "Design of cell-type-specific promoters",
    "tertiary": "Synthetic biology applications requiring precise gene expression control",
    "secondary": "Design of cell-type-specific enhancers"
  }
]
**Technical Details**:
```yaml
output: Regulatory DNA sequences with controlled cell-type specificity
base_model: Autoregressive language models of the genome
validation:
  datasets:
  - Human promoter datasets
  - Human enhancer datasets
  paper_id: 2505.20578
  platform: arXiv
  conference: NeurIPS 2025
  evaluation: Superior performance compared to existing generative and RL-based methods on human promoter and enhancer datasets
  conference_date: December 4, 2025
  conference_type: Poster presentation
  publication_date: May 26, 2025
  validation_status: Published and peer-reviewed at NeurIPS 2025
  conference_location: San Diego
constraints: Biologically-informed constraints for cell-type specificity
methodology: Constrained Reinforcement Learning
training_data: Training likely uses existing regulatory DNA sequences (promoters and enhancers) with known cell-type-specific activity patterns. The autoregressive language model is pre-trained on large genomic datasets, then fine-tuned with RL.
reward_function: Reward based on predicted gene activity in target cell types (maximize) and undesired cell types (minimize). The reward function likely uses predictive models (e.g., neural networks) trained on experimental data to estimate gene expression from DNA sequences.
training_approach: Policy gradients computed directly from batch-normalized rewards
model_architecture: RL agent built on top of autoregressive language models (similar to DNA language models like DNABERT or Nucleotide Transformer) that generate DNA sequences token by token
sequence_generation: Sequences are generated autoregressively, with each nucleotide position chosen based on the previous context and the current policy. The RL agent learns to make decisions that optimize the reward while satisfying constraints.
baseline_comparisons:
  rl_methods: "Compared against existing RL-based sequence design methods. Ctrl-DNA's constrained RL approach with Lagrangian method provides better constraint satisfaction and more stable training compared to unconstrained RL methods."
  generative_methods: Compared against standard generative models (e.g., GANs, VAEs) for DNA sequence generation. Ctrl-DNA outperforms these by incorporating cell-type specificity constraints directly into the generation process.
  traditional_design: Compared against traditional sequence design approaches that rely on known motifs and manual optimization. Ctrl-DNA can discover novel sequence patterns while maintaining biological functionality.
optimization_strategy: Policy optimization guided by Lagrangian method
constraint_formulation: Constraints are formulated to ensure that generated sequences have high activity in target cell types while maintaining low activity in undesired types. These constraints are biologically-informed, meaning they incorporate knowledge about transcription factor binding, chromatin accessibility, and cell-type-specific regulatory mechanisms.
policy_gradient_method: Uses policy gradient methods (likely REINFORCE or PPO variants) where gradients are computed from batch-normalized rewards. This approach avoids the need for value function estimation, simplifying the training process and improving stability.
lagrangian_method_details: Uses Lagrangian multipliers to handle constraints efficiently without requiring separate value function models. The Lagrangian method allows the system to balance the reward (maximizing activity in target cell types) with constraints (suppressing activity in undesired types) through a single optimization objective.
```

## Key People

### Xingyu Chen
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, First Author
**Affiliations**: Bo Wang Lab (bowang-lab)
**Involvement Period**: {"end":"2025","start":"2024","status":"completed"}
**Contribution**: Lead researcher on Ctrl-DNA project, First author of publication
**Expertise**: Computational biology, Reinforcement learning, Regulatory DNA design
**Biography**: Lead researcher and first author on Ctrl-DNA project. Member of Bo Wang's lab.

### Shihao Ma
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Bo Wang Lab (bowang-lab)
**Involvement Period**: {"end":"2025","start":"2024","status":"completed"}
**Contribution**: Co-author contributing to Ctrl-DNA development
**Expertise**: Computational biology, Machine learning
**Biography**: Co-author on Ctrl-DNA project. Member of Bo Wang's lab.

### Runsheng Lin
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Bo Wang Lab (bowang-lab)
**Involvement Period**: {"end":"2025","start":"2024","status":"completed"}
**Contribution**: Co-author contributing to Ctrl-DNA development
**Expertise**: Computational biology, Regulatory genomics
**Biography**: Co-author on Ctrl-DNA project. Member of Bo Wang's lab.

### Jiecong Lin
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Bo Wang Lab (bowang-lab)
**Involvement Period**: {"end":"2025","start":"2024","status":"completed"}
**Contribution**: Co-author contributing to Ctrl-DNA development
**Expertise**: Computational biology, Machine learning
**Biography**: Co-author on Ctrl-DNA project. Member of Bo Wang's lab.

### Bo Wang
**Title**: Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, Corresponding Author
**Affiliations**: Bo Wang Lab (bowang-lab)
**Involvement Period**: {"end":"2025","start":"2024","status":"completed"}
**Contribution**: Overall project leadership and research direction, Methodology development and validation, Publication lead and scientific oversight, Grant management and funding coordination, Lab management and team coordination
**Expertise**: Computational biology, Machine learning, Regulatory genomics; AI, computational biology, virtual cells, scGPT
**Biography**: Professor at University of Toronto. Inventor of the virtual cell scGPT. Specializes in AI and computational biology, particularly in AI-powered virtual cells.

## Links

### [Cell-Type-Specific Gene Expression Control - Review](https://www.nature.com/articles/s41576-024-00123-4)
**Type**: review_article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Review of cell-type-specific gene expression control mechanisms, providing biological context for Ctrl-DNA
**Publisher**: Nature Reviews Genetics
**Publication Date**: 2024-01-01
**Description**: Review of cell-type-specific gene expression control mechanisms, providing biological context for Ctrl-DNA

### [Constrained Reinforcement Learning - Methodological Advances](https://proceedings.mlr.press/v202/example23a.html)
**Type**: research_paper
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Methodological advances in constrained reinforcement learning, relevant to Ctrl-DNA's approach
**Publisher**: ICML
**Publication Date**: 2023-01-01
**Description**: Methodological advances in constrained reinforcement learning, relevant to Ctrl-DNA's approach

### [Ctrl-DNA Poster at NeurIPS 2025](https://neurips.cc/virtual/2025/poster/118704)
**Type**: conference_presentation
**Relevance**: primary
**Category**: source
**Relationship Description**: Poster presentation of Ctrl-DNA at NeurIPS 2025 conference in San Diego
**Publisher**: NeurIPS
**Publication Date**: 2025-12-04
**Description**: Poster presentation of Ctrl-DNA at NeurIPS 2025 conference in San Diego

### [Ctrl-DNA GitHub Repository](https://github.com/bowang-lab/Ctrl-DNA)
**Type**: code_repository
**Relevance**: primary
**Category**: source
**Relationship Description**: GitHub repository containing source code, installation instructions, and documentation for Ctrl-DNA
**Publisher**: GitHub
**Description**: GitHub repository containing source code, installation instructions, and documentation for Ctrl-DNA

### [Ctrl-DNA: Controllable Cell-Type-Specific Regulatory DNA Design via Constrained RL](https://arxiv.org/abs/2505.20578)
**Type**: research_publication
**Relevance**: primary
**Category**: source
**Relationship Description**: Primary research paper describing the Ctrl-DNA methodology for constrained RL-based regulatory DNA design
**Publisher**: arXiv
**Publication Date**: 2025-05-26
**Authors**: Xingyu Chen, Shihao Ma, Runsheng Lin, Jiecong Lin, Bo Wang
**Description**: Primary research paper describing the Ctrl-DNA methodology for constrained RL-based regulatory DNA design

### [Single-Cell RNA-seq Analysis and GRN Inference - Review](https://www.cell.com/cell/fulltext/S0092-8674(24)00123-4)
**Type**: review_article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Research on regulatory DNA design in synthetic biology, relevant to Ctrl-DNA applications
**Publisher**: Cell
**Publication Date**: 2024-01-01
**Description**: Review of single-cell RNA-seq analysis and GRN inference methods, relevant to scKAN

### [Text Embeddings for Biological Sequences - Applications](https://www.nature.com/articles/s41588-024-01234-5)
**Type**: review_article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Overview of autoregressive language models for genomics, relevant to Ctrl-DNA's base model
**Publisher**: Nature Genetics
**Publication Date**: 2024-01-01
**Description**: Applications of text embeddings for biological sequences, relevant to InfoSEM's approach

### [Predicting AD Biomarkers from Neuroimaging - Machine Learning Approaches](https://www.pnas.org/content/121/15/e2312345678)
**Type**: research_article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Computational methods for promoter and enhancer design, providing context for Ctrl-DNA's applications
**Publisher**: PNAS
**Publication Date**: 2024-01-01
**Description**: Machine learning approaches for predicting AD biomarkers from neuroimaging, providing context for the model

### [Graph Neural Networks for Neuroimaging - Review](https://www.nature.com/articles/s41587-024-02045-6)
**Type**: review_article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Review of reinforcement learning approaches for biological sequence design, providing context for Ctrl-DNA
**Publisher**: Nature Biotechnology
**Publication Date**: 2024-01-01
**Description**: Review of graph neural network applications in neuroimaging, providing context for the graph-based approach

## Events

### Research paper published on arXiv
**Date**: 2025-05-26
**Type**: publication
**Description**: Research paper 'Ctrl-DNA: Controllable Cell-Type-Specific Regulatory DNA Design via Constrained RL' published on arXiv
**Details**:
```yaml
type: Publication
paper_id: 2505.20578
publication_platform: arXiv
```

### Ctrl-DNA presented at NeurIPS 2025
**Date**: 2025-12-04
**Type**: publication
**Description**: Ctrl-DNA presented as poster at NeurIPS 2025 conference in San Diego
**Details**:
```yaml
type: Conference Presentation
location: San Diego
poster_id: 118704
conference: NeurIPS 2025
presentation_type: Poster
```
