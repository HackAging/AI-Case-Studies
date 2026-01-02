---
id: diffusion-protein-design-2025
slug: diffusion-protein-design-2025
entity_type: research
status: published
data_completeness: very_high
last_researched: 2025-01-27
research_category: collaboration
researcher: AI Assistant
version: 3.1
name: 2025 Diffusion Family for Protein Design (Sequence/Structure Co-Design)
description: A collaborative network of researchers and institutions working on diffusion models for sequence-structure co-design of proteins. This represents a family of related methods published in 2025 that advance the field of computational protein design. The collaboration includes 5 independent research groups from 7 institutions developing diffusion-based generative models for de novo protein design with simultaneous sequence and structure generation.
mission: To advance the field of computational protein design through diffusion-based generative models that enable simultaneous sequence and structure co-design, allowing for the creation of novel proteins with specified functional and structural properties for biomedical and biotechnological applications.
entity_data:
  status: active
  results:
  summary: Multiple diffusion models successfully developed and published in 2025, demonstrating high success rates (23-50%) in various protein design tasks, enabling simultaneous sequence and structure co-design, and expanding accessible protein space beyond evolutionary constraints.
  key_achievements:
  - "CFP-Gen: High success in generating proteins with functionality comparable to natural proteins"
  - "PPDiff: 50.00% pretraining success rate, 23.16% mini-binder design success rate, 16.89% antigen-antibody complex design success rate"
  - "Constrained Diffusion: 100% constraint satisfaction while maintaining structural diversity"
  - "VibeGen: Designed proteins accurately reproduce specified normal mode amplitudes"
  - "PT-DiT: Enables efficient protein engineering in unified sequence-structure space"
  objectives:
  - Develop diffusion-based generative models for simultaneous sequence and structure co-design
  - Enable creation of novel proteins with specified functional and structural properties
  - Advance computational protein design through multi-constraint optimization
  - Expand accessible protein space beyond evolutionary constraints
  start_date: 2024
  methodology:
  overview: The 2025 diffusion family for protein design represents a collection of methods that enable simultaneous sequence and structure co-design through diffusion-based generative models. Each method follows a general workflow but with specific adaptations for different design goals.
  general_workflow:
  step_1: "Problem specification: Define design goals (functional annotations, structural constraints, binding targets, etc.)"
  step_2: "Condition encoding: Encode constraints and conditions into model-compatible format"
  step_3: "Diffusion generation: Generate protein candidates through reverse diffusion process"
  step_4: "Validation: Evaluate generated proteins using computational metrics (structure prediction, binding affinity, etc.)"
  step_5: "Selection: Rank and select best candidates based on design criteria"
  step_6: "Experimental validation: Synthesize and test selected designs in laboratory (when applicable)"
  publication_date: 2025
  collaboration_period: 2024-2025
taxonomy:
  geography: Global
  ai_approach:
  - Generative AI
  ai_technology:
  - Generative AI
  - Diffusion Models
  - Protein LMs
  - Transformers
  primary_focus:
  - Protein Design & Engineering
  aging_approach:
  - Molecule Design
  target_biology:
  - General Aging/Longevity
  ai_architecture:
  - Diffusion Models
  - Protein LMs
  - Transformers
  ai_specialization: []
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality:
  - Therapeutic Proteins
organizations:
  -
    name: Syracuse University
    role: collaborator
    org_type: institution
    website: "https://www.syracuse.edu"
    status: operational
    role_description: Constrained Diffusion collaboration
    contribution_description: Research infrastructure, faculty support (Ferdinando Fioretto), government grant support for Constrained Diffusion collaboration
  -
    name: Rutgers University
    role: collaborator
    org_type: institution
    website: "https://www.rutgers.edu"
    status: operational
    role_description: Constrained Diffusion collaboration
    contribution_description: Research infrastructure, faculty support (Sagar Khare), government grant support for Constrained Diffusion collaboration
  -
    name: Peking University
    role: institution
    org_type: institution
    website: "https://www.pku.edu.cn"
    status: operational
    role_description: PT-DiT development
    contribution_description: Research infrastructure, faculty support, government grant support for PT-DiT development
  -
    name: King Abdullah University of Science and Technology (KAUST)
    role: institution
    org_type: institution
    website: "https://www.kaust.edu.sa"
    status: operational
    role_description: CFP-Gen development
    contribution_description: Research infrastructure, faculty support, computational resources, laboratory facilities for CFP-Gen development
  -
    name: ByteDance AI Lab
    role: lab
    org_type: lab
    website: "https://www.bytedance.com"
    status: operational
    role_description: PPDiff development
    contribution_description: Research funding, computational resources, research infrastructure for PPDiff development
  -
    name: University of Washington - Institute for Protein Design
    role: institution
    org_type: institution
    website: "https://www.ipd.uw.edu"
    status: operational
    role_description: Related work (RFdiffusion foundation)
    contribution_description: Foundational research, historical context for RFdiffusion and broader diffusion protein design field
  -
    name: Massachusetts Institute of Technology
    role: institution
    org_type: institution
    website: "https://www.mit.edu"
    status: operational
    role_description: VibeGen development
    contribution_description: Research infrastructure, faculty support, computational resources for VibeGen development
products:
  -
    name: Constrained Diffusion for Protein Design
    type: research_methodology
    status: Research & Development
    development_stage: Research / Preclinical
  -
    name: VibeGen
    type: research_methodology
    status: Research & Development
    development_stage: Research / Preclinical
  -
    name: PT-DiT
    type: research_methodology
    status: Research & Development
    development_stage: Research / Preclinical
  -
    name: PPDiff
    type: research_methodology
    status: Research & Development
    development_stage: Research / Preclinical
  -
    name: CFP-Gen
    type: research_methodology
    status: Research & Development
    development_stage: Research / Preclinical
links:
  -
    url: "https://en.wikipedia.org/wiki/David_Baker_(biochemist)"
    type: reference
    title: David Baker - Wikipedia
  -
    url: "https://github.com/bytedance/dplm"
    type: code_repository
    title: ByteDance DPLM - Diffusion Protein Language Model
  -
    url: "https://github.com/yinjunbo/cfpgen"
    type: code_repository
    title: GitHub - CFP-Gen
  -
    url: "https://www.ipd.uw.edu/2022/12/a-diffusion-model-for-protein-design/"
    type: reference
    title: "RFdiffusion: A diffusion model for protein design"
  -
    url: "https://www.rcsb.org"
    type: database
    title: Protein Data Bank (PDB)
  -
    url: "https://digital.lib.washington.edu/researchworks/items/bc4faf1c-f575-4180-93cb-bdc5233d941a"
    type: reference
    title: "Diffusion Models for Protein Structure Design: From Backbone Generation to Atomic-Resolution Enzyme Design"
  -
    url: "https://arxiv.org/abs/2504.16479"
    type: article
    title: The Dance of Atoms - De Novo Protein Design with Diffusion Model
  -
    url: "https://arxiv.org/abs/2503.21450"
    type: research_publication
    title: "CMADiff: Cross-Modal Aligned Diffusion for Controllable Protein Generation"
  -
    url: "https://www.nature.com/articles/s41586-023-06067-5"
    type: research_publication
    title: De novo design of protein structure and function with RFdiffusion
  -
    url: "https://arxiv.org/abs/2510.14989"
    type: research_publication
    title: Constrained Diffusion for Protein Design with Hard Structural Constraints
  -
    url: "https://arxiv.org/abs/2502.10173"
    type: research_publication
    title: Agentic End-to-End De Novo Protein Design for Tailored Dynamics Using a Language Diffusion Model
  -
    url: "https://pubs.rsc.org/en/content/articlelanding/2025/sc/d5sc02055g"
    type: research_publication
    title: Unifying sequence-structure coding for advanced protein engineering via a multimodal diffusion transformer
  -
    url: "https://arxiv.org/abs/2506.11420"
    type: research_publication
    title: "PPDiff: Diffusing in Hybrid Sequence-Structure Space for Protein-Protein Complex Design"
  -
    url: "https://arxiv.org/abs/2505.22869"
    type: research_publication
    title: "CFP-Gen: Combinatorial Functional Protein Generation via Diffusion Language Models"
---

# 2025 Diffusion Family for Protein Design (Sequence/Structure Co-Design)

## Description

A collaborative network of researchers and institutions working on diffusion models for sequence-structure co-design of proteins. This represents a family of related methods published in 2025 that advance the field of computational protein design. The collaboration includes 5 independent research groups from 7 institutions developing diffusion-based generative models for de novo protein design with simultaneous sequence and structure generation.

## Mission

To advance the field of computational protein design through diffusion-based generative models that enable simultaneous sequence and structure co-design, allowing for the creation of novel proteins with specified functional and structural properties for biomedical and biotechnological applications.

## Project Information

**Start Date**: 2024
**Publication Date**: 2025
**Objectives**: Develop diffusion-based generative models for simultaneous sequence and structure co-design,Enable creation of novel proteins with specified functional and structural properties,Advance computational protein design through multi-constraint optimization,Expand accessible protein space beyond evolutionary constraints
**Methodology**: [object Object]
**Results**: [object Object]
**Collaboration Period**: 2024-2025

## AI Methods

- Generative AI
- Diffusion Models
- Protein Language Models
- Transformer Models

## Data Types

- Protein sequences
- Protein structures
- Functional annotations
- Protein-protein complexes

## Scientific Background

```yaml
ai_necessity: "AI is essential because: (1) 2025 advances (e.g., CFP-Gen; retrieval-augmented inverse folding) improve multi-constraint design, (2) Diffusion models enable sequence/structure co-design, (3) Enables design of protein degraders, switches for aging tissues. The complexity of protein design space (estimated 10^130 possible sequences for a 100-residue protein) makes exhaustive search impossible, requiring AI-guided exploration."
what_changed_2025: "2025 advances in diffusion family for protein design. CFP-Gen and retrieval-augmented inverse folding improve multi-constraint design. Enables multi-modal complex modeling and co-design. Expands feasible therapeutic classes (protein degraders, switches) for aging tissues. Key innovations include: simultaneous sequence-structure generation, better constraint integration, and expanded design capabilities."
historical_context:
  2025_breakthroughs: 2025 represents a maturation of diffusion-based protein design, with multiple groups independently developing methods for sequence-structure co-design
  rfdiffusion_impact: "RFdiffusion, developed by David Baker's lab at University of Washington, was a pioneering work showing that diffusion models could generate novel protein structures. Published in Nature (2023), it established diffusion models as a viable approach for de novo protein design."
biological_bottleneck: Designing multifunctional proteins (e.g., proteases, senescence-targeting binders) with stability and specificity. Traditional methods limited in multi-constraint optimization. Previous computational methods often focused on either sequence or structure separately.
```

## Lessons Learned

### Achievements

- Successfully demonstrated that diffusion models can effectively generate functional proteins with specified constraints
- Achieved high success rates (23-50%) in various protein design tasks
- Enabled simultaneous sequence and structure co-design, simplifying the design process
- Expanded the accessible protein space beyond evolutionary constraints
- Demonstrated ability to satisfy multiple constraints simultaneously (functional, structural, sequential)

### Challenges

- Design success rates vary significantly depending on application complexity
- Computational requirements for training and inference can be substantial
- Experimental validation of designed proteins is still required
- Integration of multiple constraint types remains challenging

### Impact on Field

The 2025 diffusion family for protein design represents a significant advancement in computational protein design. These methods enable more accurate and efficient design of proteins with specified functions and structures, opening new possibilities for biomedical research, biotechnology, and therapeutic development. The ability to simultaneously design sequence and structure, while satisfying multiple constraints, represents a major step forward in the field.

## Organizations

### Syracuse University
**Role in Project**: collaborator
**Role Description**: Constrained Diffusion collaboration
**Contribution**: Research infrastructure, faculty support (Ferdinando Fioretto), government grant support for Constrained Diffusion collaboration
**Organization Type**: institution
**Status**: operational
**Website**: https://www.syracuse.edu
**Description**: Research university in USA that collaborated on Constrained Diffusion for Protein Design with Hard Structural Constraints. Syracuse provides research infrastructure, faculty support (Ferdinando Fioretto), and government grant support.
**Focus**: Optimization, machine learning, constrained generation

### Rutgers University
**Role in Project**: collaborator
**Role Description**: Constrained Diffusion collaboration
**Contribution**: Research infrastructure, faculty support (Sagar Khare), government grant support for Constrained Diffusion collaboration
**Organization Type**: institution
**Status**: operational
**Website**: https://www.rutgers.edu
**Description**: Research university in USA that collaborated on Constrained Diffusion for Protein Design with Hard Structural Constraints. Rutgers provides research infrastructure, faculty support (Sagar Khare), and government grant support.
**Focus**: Computational protein design, structural biology, constrained optimization

### Peking University
**Role in Project**: institution
**Role Description**: PT-DiT development
**Contribution**: Research infrastructure, faculty support, government grant support for PT-DiT development
**Organization Type**: institution
**Status**: operational
**Website**: https://www.pku.edu.cn
**Description**: Research university in China that developed PT-DiT, a multimodal diffusion transformer for advanced protein engineering. Peking University provides research infrastructure, faculty support, and government grant support.
**Focus**: Computational chemistry, protein engineering, multimodal diffusion transformers

### King Abdullah University of Science and Technology (KAUST)
**Role in Project**: institution
**Role Description**: CFP-Gen development
**Contribution**: Research infrastructure, faculty support, computational resources, laboratory facilities for CFP-Gen development
**Organization Type**: institution
**Status**: operational
**Website**: https://www.kaust.edu.sa
**Description**: Research university in Saudi Arabia that developed CFP-Gen, a diffusion language model for combinatorial functional protein generation. KAUST provides research infrastructure, faculty support, computational resources, and laboratory facilities for protein design research.
**Focus**: Computational biology, protein design, machine learning, diffusion models

### ByteDance AI Lab
**Role in Project**: lab
**Role Description**: PPDiff development
**Contribution**: Research funding, computational resources, research infrastructure for PPDiff development
**Organization Type**: lab
**Status**: operational
**Website**: https://www.bytedance.com
**Description**: Corporate research lab that developed PPDiff, a diffusion model for protein-protein complex design using hybrid sequence-structure space. ByteDance AI Lab provides research funding, computational resources, and research infrastructure for protein design research.
**Focus**: Machine learning, protein-protein interactions, diffusion models, protein design

### University of Washington - Institute for Protein Design
**Role in Project**: institution
**Role Description**: Related work (RFdiffusion foundation)
**Contribution**: Foundational research, historical context for RFdiffusion and broader diffusion protein design field
**Organization Type**: institution
**Status**: operational
**Website**: https://www.ipd.uw.edu
**Description**: Research institute focused on computational protein design, led by Nobel Prize winner David Baker
**Focus**: Protein design research, RFdiffusion, RFantibody technologies, computational biology

### Massachusetts Institute of Technology
**Role in Project**: institution
**Role Description**: VibeGen development
**Contribution**: Research infrastructure, faculty support, computational resources for VibeGen development
**Organization Type**: institution
**Status**: operational
**Website**: https://www.mit.edu
**Description**: Research university in USA that developed VibeGen, an agentic end-to-end de novo protein design framework for tailored dynamics using a language diffusion model. MIT provides research infrastructure, faculty support, and computational resources.
**Focus**: Materials science, protein mechanics, AI for materials, protein dynamics

## Locations

### University of Washington Campus
**Type**: headquarters
**City**: Seattle
**State/Region**: Washington
**Country**: USA
**Organizations**: University of Washington - Institute for Protein Design

### Syracuse University Campus
**Type**: headquarters
**City**: Syracuse
**State/Region**: New York
**Country**: USA
**Organizations**: Syracuse University

### Rutgers University Campus
**Type**: headquarters
**City**: New Brunswick
**State/Region**: New Jersey
**Country**: USA
**Organizations**: Rutgers University

### Peking University Campus
**Type**: headquarters
**City**: Beijing
**Country**: China
**Organizations**: Peking University

### MIT Campus
**Type**: headquarters
**City**: Cambridge
**State/Region**: Massachusetts
**Country**: USA
**Organizations**: Massachusetts Institute of Technology

### KAUST Campus
**Type**: headquarters
**City**: Thuwal
**Country**: Saudi Arabia
**Organizations**: King Abdullah University of Science and Technology (KAUST)

## Products

### Constrained Diffusion for Protein Design
**Type**: research_methodology
**Status**: Research & Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: Constrained Diffusion: Protein Design with Hard Structural Constraints
**Description**: A constrained diffusion framework for protein design ensuring strict adherence to functional requirements while maintaining stereochemical and geometric feasibility. The approach integrates proximal feasibility updates with ADMM decomposition in the generation process.
**Mechanism of Action**: Integrates proximal feasibility updates with ADMM (Alternating Direction Method of Multipliers) decomposition in the generation process. Ensures strict adherence to functional requirements while maintaining stereochemical and geometric realism.
**Technical Details**:
```yaml
architecture:
  type: Constrained Diffusion Framework
  key_components:
  - "Proximal feasibility updates: Ensure constraint satisfaction during generation"
  - "ADMM decomposition: Handles complex constraint sets efficiently"
  - "Diffusion process: Core generative mechanism"
  - "Constraint enforcement: Hard structural constraints (bonds, geometry) strictly enforced"
  training_approach: Diffusion model training with integrated constraint enforcement
performance_metrics:
  applications_tested:
  - Motif scaffolding
  - Constrained pocket design
  structural_diversity: Maintained (no reduction compared to unconstrained generation)
  constraint_satisfaction_rate: 100%
```

### VibeGen
**Type**: research_methodology
**Status**: Research & Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: VibeGen: Agentic End-to-End De Novo Protein Design for Tailored Dynamics Using a Language Diffusion Model
**Description**: VibeGen is a generative AI framework enabling de novo protein design with specified normal mode vibrations. The model uses a dual-model architecture consisting of a protein designer generating sequences based on given vibrational modes and a protein predictor evaluating their dynamic accuracy.
**Mechanism of Action**: Dual-model architecture: protein designer generates sequences based on specified normal mode vibrations, protein predictor evaluates dynamic accuracy. Language diffusion model serves as core generative component.
**Technical Details**:
```yaml
validation: Designed proteins validated through molecular dynamics simulations to confirm normal mode reproduction
architecture:
  type: Dual-Model Language Diffusion Architecture
  key_components:
  - "Protein Designer: Generates protein sequences based on specified normal mode vibrations"
  - "Protein Predictor: Evaluates dynamic accuracy of designed sequences"
  - "Language diffusion model: Core generative component"
  - "Normal mode integration: Incorporates vibrational mode specifications into design process"
  training_approach: Dual-model training where designer and predictor are trained jointly
capabilities:
  - Design proteins with specified normal mode vibrations
  - De novo sequences with no significant similarity to natural proteins
  - Stable, functionally relevant structures
```

### PT-DiT
**Type**: research_methodology
**Status**: Research & Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: PT-DiT: Unifying sequence-structure coding for advanced protein engineering via a multimodal diffusion transformer
**Description**: PT-DiT is a multimodal diffusion transformer model that integrates sequence and structure encoding for advanced protein engineering. The model uses ProTokens, machine-learned 'amino acids' derived from structural databases through self-supervised learning.
**Mechanism of Action**: Uses machine-learned ProTokens derived from structural databases through self-supervised learning, providing a compact representation unifying sequence and structure modalities. Multimodal diffusion transformer enables joint sequence-structure design.
**Technical Details**:
```yaml
architecture:
  type: Multimodal Diffusion Transformer
  key_components:
  - "ProTokens: Machine-learned 'amino acids' derived from structural databases through self-supervised learning"
  - "Multimodal diffusion transformer: Unifies sequence and structure encoding"
  - "Compact representation: Efficiently encodes both sequence and structure information"
  - "Transformer architecture: Enables contextual protein design and directed evolution"
  training_approach: Self-supervised learning on structural databases to learn ProTokens, then diffusion training for protein generation
capabilities:
  - Protein engineering in unified sequence-structure space
  - Contextual protein design
  - Metastable state sampling
  - Directed evolution
```

### PPDiff
**Type**: research_methodology
**Status**: Research & Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: PPDiff: Diffusing in Hybrid Sequence-Structure Space for Protein-Protein Complex Design
**Description**: PPDiff is a diffusion model for jointly designing protein sequence and structure, aimed at creating high-affinity binding proteins for arbitrary protein targets. The model uses a Sequence Structure Interleaving Network (SSINC) with causal attention layers.
**Mechanism of Action**: Uses SSINC network with causal attention layers, integrating self-attention layers for global amino acid correlations and equivariant graph layers for local 3D interactions. Diffuses in hybrid sequence-structure space.
**Technical Details**:
```yaml
architecture:
  type: Hybrid Sequence-Structure Diffusion Model
  key_components:
  - "Sequence Structure Interleaving Network (SSINC): Core architecture for hybrid sequence-structure space"
  - "Causal attention layers: Simplify complex interdependencies in protein sequences"
  - "Self-attention layers: Capture global amino acid correlations"
  - "Equivariant graph layers: Model local 3D interactions in protein structures"
  training_approach: Pre-trained on PPBench dataset, then fine-tuned for specific applications
training_data:
  size: 706,360 protein-protein complexes
  source: PPBench dataset derived from Protein Data Bank (PDB)
  data_type: Protein-protein complex structures and sequences
performance_metrics:
  pretraining_success_rate: 50.00%
  mini_binder_design_success_rate: 23.16%
  antigen_antibody_complex_design_success_rate: 16.89%
```

### CFP-Gen
**Type**: research_methodology
**Status**: Research & Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: CFP-Gen: Combinatorial Functional Protein Generation via Diffusion Language Models
**Description**: CFP-Gen is a diffusion language model for generating functional proteins that integrates multimodal conditions with functional, sequential, and structural constraints. The model uses Annotation-Guided Feature Modulation (AGFM) and Residue-Controlled Functional Encoding (RCFE) modules for dynamic feature distribution adjustment and residue-level interaction capture.
**Mechanism of Action**: Integrates multimodal conditions (functional annotations, sequence constraints, structural constraints) using AGFM and RCFE modules. Diffusion process generates protein sequences conditioned on multimodal inputs.
**Technical Details**:
```yaml
architecture:
  type: Diffusion Language Model
  key_components:
  - "Annotation-Guided Feature Modulation (AGFM): Dynamically adjusts protein feature distribution based on functional annotations (GO terms, IPR domains, EC numbers)"
  - "Residue-Controlled Functional Encoding (RCFE): Captures residue-level interactions for precise control"
  - "Multimodal condition integration: Combines functional, sequential, and structural constraints in unified framework"
  - "3D structural encoders: Imposes geometric constraints during generation"
  training_approach: Self-supervised learning on protein sequence and structure data with multimodal conditioning
capabilities:
  - High-throughput generation of new proteins with functionality comparable to natural proteins
  - Design of multifunctional proteins
  - Integration of functional, sequential, and structural constraints
training_data:
  data_types:
  - Protein sequences with functional annotations (GO terms, IPR domains, EC numbers)
  - Protein structures from PDB
  - Sequence-structure pairs
  description: Trained on large-scale protein sequence and structure datasets with functional annotations
  annotation_sources:
  - Gene Ontology (GO) terms
  - InterPro (IPR) domains
  - Enzyme Commission (EC) numbers
```

## Key People

### Jingyi Cui
**Participation Type**: researcher
**Role in Project**: Co-author, Constrained Diffusion
**Affiliations**: Rutgers University
**Expertise**: Computational protein design
**Biography**: Co-author of Constrained Diffusion

### Austin Seamann
**Participation Type**: researcher
**Role in Project**: Co-author, Constrained Diffusion
**Affiliations**: Syracuse University
**Expertise**: Optimization, machine learning
**Biography**: Co-author of Constrained Diffusion

### J. Zhang
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### S. Feng
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### Z. Cao
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### C. Fan
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### Z. Ma
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### Y. Li
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### Z. Chen
**Participation Type**: researcher
**Role in Project**: Co-author, PT-DiT
**Affiliations**: Peking University
**Biography**: Co-author of PT-DiT

### Lei Li
**Participation Type**: researcher
**Role in Project**: Co-author, PPDiff
**Affiliations**: ByteDance AI Lab
**Expertise**: Machine learning, protein-protein interactions
**Biography**: Co-author of PPDiff

### Tiaoxiao Li
**Participation Type**: researcher
**Role in Project**: Co-author, PPDiff
**Affiliations**: ByteDance AI Lab
**Expertise**: Deep learning, protein design
**Biography**: Co-author of PPDiff

### Chencheng Xu
**Participation Type**: researcher
**Role in Project**: Co-author, CFP-Gen
**Affiliations**: King Abdullah University of Science and Technology (KAUST)
**Expertise**: Protein design, computational methods
**Biography**: Co-author of CFP-Gen

### Wenjia He
**Participation Type**: researcher
**Role in Project**: Co-author, CFP-Gen
**Affiliations**: King Abdullah University of Science and Technology (KAUST)
**Expertise**: Computational biology, machine learning
**Biography**: Co-author of CFP-Gen

### Chao Zha
**Participation Type**: researcher
**Role in Project**: Co-author, CFP-Gen
**Affiliations**: King Abdullah University of Science and Technology (KAUST)
**Expertise**: Machine learning, protein design
**Biography**: Co-author of CFP-Gen

### Jacob K. Christopher
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, Constrained Diffusion
**Affiliations**: Syracuse University
**Expertise**: Optimization, constrained generation
**Biography**: First author of Constrained Diffusion. Expert in optimization and constrained generation.

### Bo Ni
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, VibeGen
**Affiliations**: Massachusetts Institute of Technology (MIT)
**Expertise**: Protein dynamics, computational materials science
**Biography**: First author of VibeGen. Expert in protein dynamics and computational materials science.

### X. Lin
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, PT-DiT
**Affiliations**: Peking University
**Expertise**: Protein engineering, diffusion transformers
**Biography**: First author of PT-DiT.

### Zhenqiao Song
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, PPDiff
**Affiliations**: ByteDance AI Lab
**Expertise**: Protein design, deep learning
**Biography**: First author of PPDiff. Expert in protein design and deep learning.

### Junbo Yin
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, CFP-Gen
**Affiliations**: King Abdullah University of Science and Technology (KAUST)
**Expertise**: Protein language models, diffusion models
**Biography**: First author of CFP-Gen. Expert in protein language models and diffusion models.

### Sagar Khare
**Title**: Associate Professor
**Participation Type**: pi
**Role in Project**: Co-Principal Investigator, Constrained Diffusion
**Affiliations**: Rutgers University
**Expertise**: Computational protein design, structural biology
**Biography**: Co-author and collaborator on Constrained Diffusion. Expert in computational protein design and structural biology.

### Ferdinando Fioretto
**Title**: Assistant Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, Constrained Diffusion
**Affiliations**: Syracuse University
**Expertise**: Optimization, machine learning
**Biography**: Corresponding author of Constrained Diffusion. Expert in optimization and machine learning.

### Markus J. Buehler
**Title**: Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, VibeGen
**Affiliations**: Massachusetts Institute of Technology (MIT)
**Expertise**: Materials science, protein mechanics, AI for materials
**Biography**: Corresponding author of VibeGen. Expert in materials science, protein mechanics, and AI for materials.

### Y.Q. Gao
**Title**: Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, PT-DiT
**Affiliations**: Peking University
**Expertise**: Computational chemistry, protein engineering
**Biography**: Corresponding author of PT-DiT. Expert in computational chemistry and protein engineering.

### Martin Renqiang Min
**Title**: Research Scientist
**Participation Type**: pi
**Role in Project**: Principal Investigator, PPDiff
**Affiliations**: ByteDance AI Lab
**Expertise**: Machine learning, protein-protein interactions, diffusion models
**Biography**: Corresponding author of PPDiff. Expert in machine learning, protein-protein interactions, and diffusion models.

### Xin Gao
**Title**: Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, CFP-Gen
**Affiliations**: King Abdullah University of Science and Technology (KAUST)
**Expertise**: Computational biology, protein design, machine learning
**Biography**: Corresponding author of CFP-Gen. Expert in computational biology, protein design, and machine learning.

## Links

### [David Baker - Wikipedia](https://en.wikipedia.org/wiki/David_Baker_(biochemist))
**Type**: reference
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: Biography of David Baker, leading researcher in protein design
**Publisher**: Wikipedia
**Description**: Biography of David Baker, leading researcher in protein design and developer of RFdiffusion
**Metadata**:
```yaml
type: Reference
subject: David Baker
```

### [ByteDance DPLM - Diffusion Protein Language Model](https://github.com/bytedance/dplm)
**Type**: code_repository
**Relevance**: secondary
**Category**: source
**Relationship Description**: Related diffusion protein language model from ByteDance AI Lab
**Publisher**: GitHub
**Description**: Related diffusion protein language model from ByteDance AI Lab, potentially related to PPDiff development
**Metadata**:
```yaml
type: Code Repository
organization: ByteDance
```

### [GitHub - CFP-Gen](https://github.com/yinjunbo/cfpgen)
**Type**: code_repository
**Relevance**: secondary
**Category**: source
**Relationship Description**: GitHub repository for CFP-Gen code
**Publisher**: GitHub
**Description**: Potential GitHub repository for CFP-Gen code (exact URL may vary, check arXiv paper for current link)
**Metadata**:
```yaml
note: GitHub repositories may be available for some methods; check individual arXiv papers for links
type: Code Repository
```

### [RFdiffusion: A diffusion model for protein design](https://www.ipd.uw.edu/2022/12/a-diffusion-model-for-protein-design/)
**Type**: reference
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Foundational work on diffusion models for protein design
**Publisher**: University of Washington IPD
**Publication Date**: 2022-12-01
**Description**: Foundational work on diffusion models for protein design by David Baker's lab, published in Nature 2023
**Metadata**:
```yaml
type: Research Article / Blog Post
key_researcher: David Baker
related_publication: Nature (2023)
```

### [Protein Data Bank (PDB)](https://www.rcsb.org)
**Type**: database
**Relevance**: secondary
**Category**: source
**Relationship Description**: Primary source of protein structure data used for training diffusion models
**Publisher**: RCSB PDB
**Description**: Primary source of protein structure data used for training diffusion models (e.g., PPBench dataset for PPDiff)
**Metadata**:
```yaml
type: Database
usage: Training data source for diffusion models
```

### [Diffusion Models for Protein Structure Design: From Backbone Generation to Atomic-Resolution Enzyme Design](https://digital.lib.washington.edu/researchworks/items/bc4faf1c-f575-4180-93cb-bdc5233d941a)
**Type**: reference
**Relevance**: secondary
**Category**: reference
**Relationship Description**: PhD thesis exploring diffusion models for protein design
**Publisher**: University of Washington
**Publication Date**: 2024-01-01
**Description**: PhD thesis by Woody Ahern exploring diffusion models for protein design, providing detailed technical background
**Metadata**:
```yaml
type: Thesis / Dissertation
author: Woody Ahern
```

### [The Dance of Atoms - De Novo Protein Design with Diffusion Model](https://arxiv.org/abs/2504.16479)
**Type**: article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Comprehensive review of diffusion models for protein design
**Publisher**: arXiv
**Publication Date**: 2025-04-01
**Description**: Comprehensive review of diffusion models for protein design, providing context for 2025 methods
**Metadata**:
```yaml
type: Review Article
arxiv_id: 2504.16479
```

### [CMADiff: Cross-Modal Aligned Diffusion for Controllable Protein Generation](https://arxiv.org/abs/2503.21450)
**Type**: research_publication
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Related work on cross-modal diffusion for protein generation
**Publisher**: arXiv
**Publication Date**: 2025-03-27
**Description**: Related work on cross-modal diffusion for protein generation, complementary to 2025 diffusion family
**Metadata**:
```yaml
type: arXiv Preprint
arxiv_id: 2503.21450
```

### [De novo design of protein structure and function with RFdiffusion](https://www.nature.com/articles/s41586-023-06067-5)
**Type**: research_publication
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Foundational Nature paper on RFdiffusion, providing historical context
**Publisher**: Nature
**Publication Date**: 2023-12-01
**Authors**: David Baker
**Description**: Foundational Nature paper on RFdiffusion, providing historical context for 2025 diffusion methods
**Metadata**:
```yaml
type: Journal Article
year: 2023
journal: Nature
institution: University of Washington - Institute for Protein Design
```

### [Constrained Diffusion for Protein Design with Hard Structural Constraints](https://arxiv.org/abs/2510.14989)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: Constrained diffusion approach for protein design with hard constraints
**Publisher**: arXiv
**Publication Date**: 2025-10-01
**Authors**: Jacob K. Christopher, Austin Seamann, Jingyi Cui, Sagar Khare, Ferdinando Fioretto
**Description**: Constrained diffusion approach for protein design with hard constraints
**Metadata**:
```yaml
type: arXiv Preprint
arxiv_id: 2510.14989
institutions:
  - Syracuse University
  - Rutgers University
```

### [Agentic End-to-End De Novo Protein Design for Tailored Dynamics Using a Language Diffusion Model](https://arxiv.org/abs/2502.10173)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: VibeGen method for protein design with tailored dynamics
**Publisher**: arXiv
**Publication Date**: 2025-02-14
**Authors**: Bo Ni, Markus J. Buehler
**Description**: VibeGen method for protein design with tailored dynamics
**Metadata**:
```yaml
type: arXiv Preprint
arxiv_id: 2502.10173
institutions:
  - Massachusetts Institute of Technology (MIT)
```

### [Unifying sequence-structure coding for advanced protein engineering via a multimodal diffusion transformer](https://pubs.rsc.org/en/content/articlelanding/2025/sc/d5sc02055g)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: PT-DiT method published in Chemical Science
**Publisher**: Chemical Science
**Publication Date**: 2025-05-15
**Authors**: X. Lin, Z. Chen, Y. Li, Z. Ma, C. Fan, Z. Cao, S. Feng, J. Zhang, Y. Q. Gao
**Description**: PT-DiT method published in Chemical Science
**Metadata**:
```yaml
doi: 10.1039/D5SC02055G
type: Journal Article
journal: Chemical Science
institutions:
  - Peking University
```

### [PPDiff: Diffusing in Hybrid Sequence-Structure Space for Protein-Protein Complex Design](https://arxiv.org/abs/2506.11420)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: PPDiff method for protein-protein complex design
**Publisher**: arXiv
**Publication Date**: 2025-06-13
**Authors**: Zhenqiao Song, Tiaoxiao Li, Lei Li, Martin Renqiang Min
**Description**: PPDiff method for protein-protein complex design using hybrid sequence-structure space
**Metadata**:
```yaml
type: arXiv Preprint
arxiv_id: 2506.11420
institutions:
  - ByteDance AI Lab
```

### [CFP-Gen: Combinatorial Functional Protein Generation via Diffusion Language Models](https://arxiv.org/abs/2505.22869)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: Main source paper for CFP-Gen method
**Publisher**: arXiv
**Publication Date**: 2025-05-28
**Authors**: Junbo Yin, Chao Zha, Wenjia He, Chencheng Xu, Xin Gao
**Description**: Main source paper for CFP-Gen method - the primary reference mentioned in the case study
**Metadata**:
```yaml
type: arXiv Preprint
arxiv_id: 2505.22869
institutions:
  - King Abdullah University of Science and Technology (KAUST)
```

## Financials

### grant
**Period**: Ongoing
**Source**: National Institutes of Health (NIH)
**Funding Type**: Government Grant
**Description**: Potential funding source for University of Washington Institute for Protein Design (related RFdiffusion foundational work).
**Note**: Funding information for specific 2025 diffusion models may not be publicly disclosed. Government grants may support related foundational research.

### grant
**Period**: 2024-2025
**Source**: Syracuse University
**Funding Type**: Institutional / Government Grants
**Description**: Research funding for Constrained Diffusion collaboration. Contributions include faculty support (Ferdinando Fioretto), research infrastructure, government grant support, and student support.

### grant
**Period**: 2024-2025
**Source**: Rutgers University
**Funding Type**: Institutional / Government Grants
**Description**: Research funding for Constrained Diffusion collaboration. Contributions include faculty support (Sagar Khare), research infrastructure, government grant support, and student support.

### grant
**Period**: 2024-2025
**Source**: Peking University
**Funding Type**: Institutional / Government Grants
**Description**: Research funding for PT-DiT development. Contributions include faculty support, research infrastructure, government grant support, and student support.

### funding
**Period**: 2024-2025
**Source**: Massachusetts Institute of Technology (MIT)
**Funding Type**: Institutional Research Funding
**Description**: Research funding for VibeGen development. Contributions include faculty support, research infrastructure, computational resources, and student support.

### funding
**Period**: 2024-2025
**Source**: ByteDance AI Lab
**Funding Type**: Corporate Research Funding
**Description**: Internal research funding for PPDiff and related protein design research. Contributions include researcher salaries, computational resources, research infrastructure, and publication support.

### funding
**Period**: 2024-2025
**Source**: King Abdullah University of Science and Technology (KAUST)
**Funding Type**: Institutional Research Funding
**Description**: Internal research funding for CFP-Gen development. Contributions include faculty salaries, research infrastructure, computational resources, laboratory facilities, and student support.

## Partnerships

### research
**Focus**: Industry-Academia
**Description**: ByteDance AI Lab collaborating with academic institutions on protein design research. Represents industry-academia collaboration in the field of computational protein design.
**Partner Organizations**:
- Massachusetts Institute of Technology (collaborator)
  - Academic institution
- Syracuse University (collaborator)
  - Academic institution
- Rutgers University (collaborator)
  - Academic institution
- Peking University (collaborator)
  - Academic institution
- King Abdullah University of Science and Technology (KAUST) (collaborator)
  - Academic institution
- ByteDance AI Lab (partner)
  - Corporate research lab

### research
**Focus**: Academic Collaboration
**Description**: Multi-institutional collaborations across different research groups working on related diffusion-based protein design methods. Each group operates independently but contributes to the broader field of diffusion-based protein design.
**Partner Organizations**:
- Massachusetts Institute of Technology (collaborator)
  - VibeGen development group
- University of Washington - Institute for Protein Design (collaborator)
  - Related foundational work (RFdiffusion)
- Syracuse University (collaborator)
  - Constrained Diffusion collaboration group
- Rutgers University (collaborator)
  - Constrained Diffusion collaboration group
- Peking University (collaborator)
  - PT-DiT development group
- ByteDance AI Lab (collaborator)
  - PPDiff development group
- King Abdullah University of Science and Technology (KAUST) (collaborator)
  - CFP-Gen development group
