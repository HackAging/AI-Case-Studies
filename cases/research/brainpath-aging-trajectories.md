---
id: brainpath-aging-trajectories
slug: brainpath-aging-trajectories
entity_type: research
status: published
data_completeness: high
last_researched: 2025-12-23
research_category: collaboration
researcher: AI Assistant
version: 4.0
name: BrainPath
description: Generative framework for predicting individualized brain aging trajectories from MRI scans using parallel transport algorithm to adapt population-level aging trajectories to individual cases
mission: To develop a generative framework capable of predicting individualized brain aging trajectories from a single baseline MRI scan, enabling personalized mapping of brain aging for precision medicine applications.
entity_data:
  name: BrainPath
  status: research_paper
  description: Generative framework for predicting individualized brain aging trajectories from MRI scans using parallel transport algorithm to adapt population-level aging trajectories to individual cases
  institutions:
  - KTH Royal Institute of Technology (4 researchers)
  - Karolinska Institutet (1 Co-PI)
  primary_goal: To develop a generative framework capable of predicting individualized brain aging trajectories from a single baseline MRI scan, enabling personalized mapping of brain aging for precision medicine applications.
  main_objectives:
  - Create a 3D generative model that learns longitudinal brain aging dynamics from population data
  - Predict anatomically accurate MRIs at arbitrary future timepoints from a single baseline scan
  - Enable personalized mapping of brain aging trajectories for individual subjects
  - Identify early biomarkers of neurodegenerative decline before clinical symptoms appear
  - Reduce the need for expensive longitudinal imaging studies by enabling prediction from single timepoint
  research_team_size: 5
  target_applications:
  - Early detection of neurodegenerative diseases
  - Personalized aging trajectory prediction
  - Clinical trial patient stratification
  - Intervention monitoring and assessment
  collaboration_period: 2024-2025
taxonomy:
  geography: Sweden
  ai_approach:
  - Generative AI
  ai_technology:
  - Generative AI
  primary_focus:
  - Aging Clocks
  - Diagnostics & Preventive Health
  aging_approach:
  - Diagnostics/Age Assessment
  target_biology:
  - Neurodegenerative
  - General Aging/Longevity
  ai_architecture: []
  ai_specialization: []
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality: []
organizations:
  -
    name: KTH Royal Institute of Technology
    role: primary
    org_type: institution
    legal_name: Kungliga Tekniska högskolan
    website: "https://www.kth.se/en"
    status: operational
    role_description: Primary development institution
    contribution_description: Primary development institution providing generative model development, machine learning expertise, computational resources, and project leadership
  -
    name: Karolinska Institutet
    role: collaborator
    org_type: institution
    legal_name: Karolinska Institutet
    website: "https://ki.se/en"
    status: operational
    role_description: Research Collaboration Partner
    contribution_description: Clinical and neuroimaging expertise, brain aging research, neurodegenerative disease expertise, and clinical validation
products:
  -
    name: BrainPath
    type: research_methodology
    status: Published
    development_stage: Research / Preclinical
links:
  -
    url: "https://github.com/Immortal-ai-2025"
    type: reference
    title: AI Longevity 2025 Case Studies
  -
    url: "https://ki.se/en/nvs/research"
    type: website
    title: Karolinska Institutet Brain Aging Research
  -
    url: "https://www.kth.se/en/cbh/forskning/medicinsk-bildbehandling"
    type: website
    title: KTH Medical Imaging Research
  -
    url: "https://www.vr.se/"
    type: website
    title: Swedish Research Council (Vetenskapsrådet)
  -
    url: "https://www.nature.com/subjects/brain-aging"
    type: reference
    title: Brain Aging and Neurodegenerative Diseases
  -
    url: "https://www.miccai.org/"
    type: reference
    title: MICCAI Conference - Medical Image Computing
  -
    url: "https://adni.loni.usc.edu/data-samples/data-use-agreement/"
    type: reference
    title: ADNI Data Usage Guidelines
  -
    url: "https://www.nature.com/articles/s41593-019-0448-4"
    type: article
    title: "Brain Age Prediction: A Review"
  -
    url: "https://arxiv.org/abs/2511.08847"
    type: research_publication
    title: "Data-driven spatiotemporal modeling reveals personalized trajectories of cortical atrophy in Alzheimer's disease"
  -
    url: "https://arxiv.org/abs/2502.21049"
    type: research_publication
    title: Synthesizing Individualized Aging Brains in Health and Disease with Generative Models and Parallel Transport
  -
    url: "https://adni.loni.usc.edu/"
    type: reference
    title: "Alzheimer's Disease Neuroimaging Initiative (ADNI)"
---

# BrainPath

## Description

Generative framework for predicting individualized brain aging trajectories from MRI scans using parallel transport algorithm to adapt population-level aging trajectories to individual cases

## Mission

To develop a generative framework capable of predicting individualized brain aging trajectories from a single baseline MRI scan, enabling personalized mapping of brain aging for precision medicine applications.

## Project Information

**Collaboration Period**: 2024-2025

## Scientific Background

```yaml
limitations:
  - Requires high-quality baseline MRI scans - may not work well with low-quality or artifact-ridden images
  - Validation primarily on ADNI and NACC datasets - generalizability to diverse populations needs further validation
  - Focuses on structural changes - does not incorporate functional (fMRI) or molecular (PET) imaging
  - Computational requirements may limit accessibility
  - Clinical validation and regulatory pathways remain to be established
future_directions:
  - Integration with functional imaging (fMRI) and molecular imaging (PET) for more comprehensive aging assessment
  - Validation on more diverse populations and datasets
  - "Extension to other neurodegenerative diseases beyond Alzheimer's"
  - Development of clinical tools and regulatory approval pathways
  - Integration with genetic and lifestyle factors for more comprehensive risk assessment
  - Real-time clinical implementation and validation
problem_statement: Traditional aging biomarkers require longitudinal data collection over years. Single-timepoint assessment of biological age and future disease risk is limited. Current methods cannot predict personalized aging trajectories from a single baseline scan. This creates a major bottleneck in aging research and clinical practice, as longitudinal studies are expensive, time-consuming, and may miss critical early intervention windows.
solution_approach: BrainPath uses generative models and parallel transport to learn population-level aging dynamics and adapt them to individual subjects. This enables prediction of future brain states from a single baseline MRI scan. The approach combines the power of population-level knowledge with geometric methods to personalize predictions.
biological_relevance: "Brain aging is a complex process involving structural and functional changes. Early detection of accelerated aging or neurodegenerative patterns can enable timely interventions. The framework identifies subtle patterns in single MRI scans that predict future aging trajectories. This is particularly relevant for neurodegenerative diseases like Alzheimer's, where early intervention is critical but current detection methods require longitudinal monitoring."
technical_innovation: "The framework combines 3D generative models with parallel transport algorithms to create subject-specific aging trajectories. Key innovations include: (1) Age calibration loss ensuring generated images match expected age progression, (2) Swap learning strategy improving generalization across age ranges, (3) Age perceptual loss maintaining anatomical accuracy, and (4) Parallel transport algorithm enabling geometric adaptation of population trajectories to individuals."
```

## Lessons Learned

### Achievements

- Successfully developed a framework for predicting personalized brain aging trajectories from single baseline scans
- Demonstrated superior performance compared to existing clinical and neuroimaging benchmarks
- Enabled early detection capabilities that could accelerate clinical trial timelines
- Reduced need for expensive longitudinal imaging studies

### Challenges

- Requires large-scale population data for training the generative model
- Validation on diverse populations needed to ensure generalizability
- Clinical translation requires regulatory approval if used as medical device
- Computational requirements for 3D generative models may limit accessibility

### Impact on Field

BrainPath Framework represents a significant advance in personalized brain aging prediction. By enabling trajectory prediction from single timepoints, it addresses a major bottleneck in aging biomarker research. The framework could accelerate clinical trials by identifying high-risk individuals earlier and enable more personalized interventions. However, as a research tool, clinical validation and regulatory pathways remain to be established.

## Organizations

### KTH Royal Institute of Technology
**Legal Name**: Kungliga Tekniska högskolan
**Role in Project**: primary
**Role Description**: Primary development institution
**Contribution**: Primary development institution providing generative model development, machine learning expertise, computational resources, and project leadership
**Organization Type**: institution
**Status**: operational
**Website**: https://www.kth.se/en
**Description**: Technical university in Stockholm, Sweden, specializing in engineering and technology research
**Focus**: Engineering sciences, biotechnology, health technology, medical imaging, machine learning

### Karolinska Institutet
**Role in Project**: collaborator
**Role Description**: Research Collaboration Partner
**Contribution**: Clinical and neuroimaging expertise, brain aging research, neurodegenerative disease expertise, and clinical validation
**Organization Type**: institution
**Status**: operational
**Website**: https://ki.se/en
**Description**: Medical university in Stockholm, Sweden, specializing in medical and clinical research
**Focus**: Brain aging, neurodegenerative diseases, neuroimaging, clinical validation

## Locations

### Stockholm, Sweden
**Type**: institution
**City**: Stockholm
**Country**: Sweden
**Organizations**: Karolinska Institutet, KTH Royal Institute of Technology

## Products

### BrainPath
**Type**: research_methodology
**Status**: Published
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: BrainPath framework - primary research methodology and product of this case
**Description**: Generative framework for predicting individualized brain aging trajectories from MRI scans using parallel transport algorithm to adapt population-level aging trajectories to individual cases
**Mechanism of Action**: A generative framework that uses parallel transport to adapt population-level aging trajectories to individual cases. The model learns longitudinal brain aging dynamics from population data and can generate subject-specific brain aging trajectories from a single baseline MRI scan.
**Target**: Individual brain aging trajectories
**Technical Details**:
```yaml
input: Single baseline MRI scan
output: Predicted MRI scans at future timepoints, personalized aging trajectories
datasets_used:
  -
    name: "Alzheimer's Disease Neuroimaging Initiative (ADNI)"
    website: "https://adni.loni.usc.edu/"
    modalities:
    - MRI
    - PET
    participants: 1,891+ participants
framework_type: 3D Generative Model
key_components:
  - Age calibration loss - ensures generated images match expected age progression
  - Swap learning strategy - improves model generalization
  - Age perceptual loss - maintains anatomical accuracy during aging simulation
  - Parallel transport algorithm - adapts population trajectories to individual subjects
model_architecture:
  type: 3D Generative Model
  input_dimensions: 3D MRI volumes (typically 256x256x256 or similar resolution)
  base_architecture: Likely VAE or GAN based architecture for 3D medical image generation
  output_dimensions: 3D MRI volumes at predicted future timepoints
performance_metrics:
  mse: Lower than baseline methods
  psnr: Higher than baseline methods
  ssim: Superior to baseline methods
  brain_age_prediction: Outperforms existing models
```

## Key People

### Neel Dey
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: KTH Royal Institute of Technology, School of Engineering Sciences in Chemistry, Biotechnology and Health
**Participation Period**: 2024-2025
**Contribution**: Researcher contributing to deep learning and computational neuroscience aspects
**Expertise**: Deep learning, computational neuroscience
**Biography**: Researcher at KTH Royal Institute of Technology, contributing to deep learning and computational neuroscience aspects

### Yuqi Zheng
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: KTH Royal Institute of Technology, School of Engineering Sciences in Chemistry, Biotechnology and Health
**Participation Period**: 2024-2025
**Contribution**: Researcher contributing to medical image processing and brain imaging
**Expertise**: Medical image processing, brain imaging
**Biography**: Researcher at KTH Royal Institute of Technology, contributing to medical image processing and brain imaging

### Jingru Fu
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, First Author
**Affiliations**: KTH Royal Institute of Technology, School of Engineering Sciences in Chemistry, Biotechnology and Health
**Participation Period**: 2024-2025
**Responsibilities**:
- Primary method development
- BrainPath framework implementation
- Data analysis and validation
- Manuscript preparation
**Contribution**: Lead researcher and first author of BrainPath publication
**Expertise**: Generative models, medical image analysis, machine learning, 3D generative models
**Biography**: Lead researcher and first author of BrainPath publication. Researcher in medical imaging and machine learning at KTH Royal Institute of Technology.

### Daniel Ferreira
**Title**: Researcher / Professor
**Participation Type**: pi
**Role in Project**: Co-Principal Investigator
**Affiliations**: Karolinska Institutet, Department of Neurobiology, Care Sciences and Society
**Participation Period**: 2024-2025
**Responsibilities**:
- Clinical and neuroimaging expertise
- Brain aging research guidance
- Scientific oversight
- Clinical validation
**Contribution**: Co-principal investigator providing clinical and neuroimaging expertise
**Expertise**: Brain aging, Alzheimer's disease, neuroimaging, neurodegenerative diseases
**Biography**: Researcher in brain aging and neurodegenerative diseases at Karolinska Institutet. Co-principal investigator providing clinical and neuroimaging expertise.

### Rodrigo Moreno
**Title**: Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator, Corresponding Author
**Affiliations**: KTH Royal Institute of Technology, School of Engineering Sciences in Chemistry, Biotechnology and Health
**Participation Period**: 2024-2025
**Responsibilities**:
- Overall project leadership
- Methodology development
- Publication lead and scientific oversight
- Grant management
**Contribution**: Principal Investigator and corresponding author of BrainPath publication
**Expertise**: Medical image analysis, machine learning, brain imaging, generative models
**Biography**: Professor in medical imaging and machine learning at KTH Royal Institute of Technology. Principal Investigator and corresponding author of BrainPath publication.

## Links

### [AI Longevity 2025 Case Studies](https://github.com/Immortal-ai-2025)
**Type**: reference
**Relevance**: secondary
**Category**: reference
**Relationship Description**: AI Longevity 2025 case study reference
**Publisher**: GitHub
**Publication Date**: 2025-01-01
**Description**: Reference to BrainPath Framework in AI Longevity 2025 case studies (arXiv 2508.16667)

### [Karolinska Institutet Brain Aging Research](https://ki.se/en/nvs/research)
**Type**: website
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: Karolinska brain aging research
**Description**: Brain aging and neurodegenerative disease research at Karolinska Institutet

### [KTH Medical Imaging Research](https://www.kth.se/en/cbh/forskning/medicinsk-bildbehandling)
**Type**: website
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: KTH medical imaging research
**Description**: Medical imaging research at KTH Royal Institute of Technology

### [Swedish Research Council (Vetenskapsrådet)](https://www.vr.se/)
**Type**: website
**Relevance**: secondary
**Category**: source
**Relationship Description**: Likely funding source
**Description**: Primary Swedish research funding agency, likely source of funding for KTH and Karolinska research

### [Brain Aging and Neurodegenerative Diseases](https://www.nature.com/subjects/brain-aging)
**Type**: reference
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: Brain aging research topic
**Description**: Research on brain aging mechanisms and neurodegenerative diseases

### [MICCAI Conference - Medical Image Computing](https://www.miccai.org/)
**Type**: reference
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: Medical image computing conference
**Description**: Premier conference for medical image computing where BrainPath may be presented

### [ADNI Data Usage Guidelines](https://adni.loni.usc.edu/data-samples/data-use-agreement/)
**Type**: reference
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: ADNI data usage guidelines
**Description**: Official ADNI dataset usage guidelines and data access information

### [Brain Age Prediction: A Review](https://www.nature.com/articles/s41593-019-0448-4)
**Type**: article
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Brain age prediction methods review
**Description**: Comprehensive review of brain age prediction methods and applications

### [Data-driven spatiotemporal modeling reveals personalized trajectories of cortical atrophy in Alzheimer's disease](https://arxiv.org/abs/2511.08847)
**Type**: research_publication
**Relevance**: secondary
**Category**: reference
**Relationship Description**: Related work on personalized brain aging trajectories
**Publisher**: arXiv
**Publication Date**: 2025-11-12
**Authors**: Chunyan Li, Yutong Mao, Xiao Liu, Wenrui Hao
**Description**: Related work on personalized brain aging trajectories using graph-based dynamic models

### [Synthesizing Individualized Aging Brains in Health and Disease with Generative Models and Parallel Transport](https://arxiv.org/abs/2502.21049)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: Main publication describing BrainPath framework
**Publisher**: arXiv
**Publication Date**: 2025-02-28
**Authors**: Jingru Fu, Yuqi Zheng, Neel Dey, Daniel Ferreira, Rodrigo Moreno
**Description**: Original preprint describing the BrainPath framework for generating individualized brain aging trajectories

### [Alzheimer's Disease Neuroimaging Initiative (ADNI)](https://adni.loni.usc.edu/)
**Type**: reference
**Relevance**: primary
**Category**: source
**Relationship Description**: Primary data source (ADNI dataset)
**Publisher**: ADNI
**Publication Date**: 2004-01-01
**Description**: Large-scale longitudinal study providing neuroimaging, biomarker, and clinical data used in training Unlearn's AD DTG model

## Financials

### grant
**Source**: Alzheimer's Disease Neuroimaging Initiative (ADNI)
**Funding Type**: Data Access
**Description**: Access to ADNI dataset for research purposes
**Note**: ADNI is funded by NIH with $60M+ in funding since 2004. Provides data access but not direct funding to this project.
**Details**:
```yaml
dataset: Longitudinal neuroimaging data
funding_organization: National Institutes of Health (NIH)
```

### grant
**Amount**: Not disclosed
**Source**: Karolinska Institutet
**Funding Type**: Institutional Support
**Description**: Research infrastructure and support from Karolinska Institutet
**Details**:
```yaml
contributions:
  - Research infrastructure
  - Faculty support (Daniel Ferreira)
  - Clinical research resources
  - Neuroimaging facilities
```

### grant
**Amount**: Not disclosed
**Source**: KTH Royal Institute of Technology
**Funding Type**: Institutional Support
**Description**: Research infrastructure and support from KTH
**Details**:
```yaml
contributions:
  - Research infrastructure
  - Faculty support (Rodrigo Moreno)
  - Research staff support (Jingru Fu, Yuqi Zheng, Neel Dey)
  - Computational resources
  - Laboratory facilities
```

### grant
**Amount**: Not publicly disclosed
**Source**: Swedish Research Council (Vetenskapsrådet)
**Funding Type**: Research Grant
**Description**: Likely source of funding for Swedish research institutions
**Note**: Swedish Research Council commonly funds research at KTH Royal Institute of Technology and Karolinska Institutet. Specific grant information not publicly available.

## Events

### Research project initiation
**Date**: 2024-01-01
**Type**: foundation
**Description**: Development of BrainPath framework begins

### Preprint publication
**Date**: 2025-02-28
**Type**: publication
**Description**: BrainPath framework preprint published on arXiv (2502.21049)
**Details**:
```yaml
title: Synthesizing Individualized Aging Brains in Health and Disease with Generative Models and Parallel Transport
arxiv_id: 2502.21049
```

### Case study reference
**Date**: 2025-08-01
**Type**: publication
**Description**: Referenced in AI Longevity 2025 case studies
**Details**:
```yaml
note: "Referenced in August 2025 (arXiv 2508.16667 - note: exact paper could not be verified)"
publication: AI Longevity 2025 case studies
```

## Partnerships

### research
**Date**: 2024-01-01
**Description**: Collaboration between engineering and medical research institutions
**Details**:
```yaml
type: Inter-institutional Collaboration
period: 2024-2025
status: active
partner: KTH Royal Institute of Technology - Karolinska Institutet
institutions:
  - KTH Royal Institute of Technology (engineering/computational expertise)
  - Karolinska Institutet (medical/clinical expertise)
```

### research
**Date**: 2024-01-01
**Description**: Access to longitudinal neuroimaging data for model development and validation
**Details**:
```yaml
type: Data Collaboration
status: active
partner: "Alzheimer's Disease Neuroimaging Initiative (ADNI)"
website: "https://adni.loni.usc.edu/"
```
