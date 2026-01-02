---
id: trialmatchai
slug: trialmatchai
entity_type: research
status: operational
data_completeness: high
last_researched: 2025-01-27
research_category: collaboration
researcher: AI Assistant
version: 3.1
name: TrialMatchAI
description: End-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data, including structured records and unstructured physician notes. The system aims to accelerate patient recruitment in clinical trials, particularly for aging populations with multimorbidity, and improve diversity and stratification in trial enrollment.
mission: To develop an end-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data, including structured records and unstructured physician notes. The system aims to accelerate patient recruitment in clinical trials, particularly for aging populations with multimorbidity, and improve diversity and stratification in trial enrollment.
entity_data:
  results:
  performance_summary: State-of-the-art performance confirmed on both synthetic and real clinical datasets, with particularly strong results in biomarker-driven cases
  real_world_validation:
  metric: Percentage of patients with at least one relevant trial in top-20 recommendations
  result: 92%
  dataset: Real oncology patient data
  description: 92% of oncology patients had at least one relevant trial found in the top-20 recommendations
  criterion_level_accuracy:
  metric: Criterion-level eligibility classification accuracy
  result: >90%
  datasets: Synthetic and real clinical datasets
  description: Over 90% accuracy in criterion-level eligibility classification, especially in biomarker-driven cases
  objectives: To develop an end-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data
  start_date: 2025
  methodology: Retrieval-Augmented Generation (RAG) with Large Language Models
  publication_date: 2025-05-13
  collaboration_period: 2025-ongoing
taxonomy:
  geography: France
  ai_approach: []
  ai_technology:
  - LLMs
  - RAG
  primary_focus:
  - Clinical Trials Optimization
  aging_approach: []
  target_biology:
  - Cancer/Oncology
  - General Aging/Longevity
  ai_architecture:
  - LLMs
  ai_specialization:
  - RAG
  development_stage: Operational
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality: []
organizations:
  -
    name: European Clinical Research Infrastructure Network (ECRIN)
    role: collaborator
    org_type: institution
    legal_name: European Clinical Research Infrastructure Network
    website: "https://ecrin.org/"
    status: operational
    role_description: Research Collaboration Partner
    contribution_description: Clinical trial infrastructure, Oncology and clinical trials expertise
  -
    name: Netherlands Cancer Institute
    role: collaborator
    org_type: institution
    legal_name: Netherlands Cancer Institute
    website: "https://www.nki.nl/"
    status: operational
    role_description: Research Collaboration Partner
    contribution_description: Cancer research expertise, Oncology and clinical research, Pathology and precision medicine, Clinical trial data
  -
    name: Centre de Bioinformatique de Bordeaux (CBiB)
    role: primary
    org_type: research_center
    legal_name: Centre de Bioinformatique de Bordeaux
    website: "https://www.bordeaux-bioinformatics.fr"
    status: operational
    role_description: Primary development institution and project host
    contribution_description: Project leadership (Macha Nikolski), Research infrastructure, Bioinformatics expertise, Development resources
  -
    name: Université de Bordeaux
    role: institution
    org_type: institution
    legal_name: Université de Bordeaux
    website: "https://www.u-bordeaux.fr/"
    status: operational
    role_description: Parent institution and project host
    contribution_description: Project leadership, Bioinformatics, Clinical research
  -
    name: Institut de Biochimie et Génétique Cellulaires
    role: collaborator
    org_type: institution
    legal_name: Institut de Biochimie et Génétique Cellulaires
    status: operational
    role_description: Research Collaboration Partner
    contribution_description: Computational biology, Bioinformatics
  -
    name: Oslo University Hospital
    role: collaborator
    org_type: institution
    legal_name: Oslo University Hospital
    website: "https://oslo-universitetssykehus.no/"
    status: operational
    role_description: Research Collaboration Partner
    contribution_description: Clinical informatics expertise, Clinical data analysis, Genomics and bioinformatics, Clinical validation
  -
    name: University of Oslo
    role: collaborator
    org_type: institution
    legal_name: University of Oslo
    website: "https://www.uio.no/"
    status: operational
    role_description: Affiliated institution
    contribution_description: Genomics, Bioinformatics
products:
  -
    name: TrialMatchAI
    type: ai_model
    status: Research/Development
    development_stage: Research / Preclinical
links:
  -
    url: "https://github.com/cbib/TrialMatchAI"
    type: documentation
    title: "GitHub - cbib/TrialMatchAI: TrialMatchAI aims to seamlessly match cancer patients to clinical trials based on their unique genomic and clinical profiles using AI"
  -
    url: "https://bordeaux-bioinformatics.fr/trialmatchai-a-new-approach-to-matching-cancer-patients-with-clinical-trials-based-on-large-language-models-llms/amp/"
    type: website
    title: "TrialMatchAI: Harnessing Large Language Models (LLMs) to Match Cancer Patients with Molecularly-driven Clinical Trials – Part of the European Open Science Cloud for Cancer Project"
  -
    url: "https://arxiv.org/abs/2505.08508"
    type: research_publication
    title: "TrialMatchAI: An End-to-End AI-powered Clinical Trial Recommendation System to Streamline Patient-to-Trial Matching"
---

# TrialMatchAI

## Description

End-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data, including structured records and unstructured physician notes. The system aims to accelerate patient recruitment in clinical trials, particularly for aging populations with multimorbidity, and improve diversity and stratification in trial enrollment.

## Mission

To develop an end-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data, including structured records and unstructured physician notes. The system aims to accelerate patient recruitment in clinical trials, particularly for aging populations with multimorbidity, and improve diversity and stratification in trial enrollment.

## Project Information

**Start Date**: 2025
**Publication Date**: 2025-05-13
**Objectives**: To develop an end-to-end AI-powered clinical trial recommendation system that streamlines patient-to-trial matching by processing heterogeneous clinical data
**Methodology**: Retrieval-Augmented Generation (RAG) with Large Language Models
**Results**: [object Object]
**Collaboration Period**: 2025-ongoing

## Lessons Learned

### Achievements

- Achieved 92% of oncology patients with relevant trial in top-20 recommendations
- Demonstrated >90% accuracy in criterion-level eligibility classification
- Developed modular, privacy-preserving system suitable for clinical deployment
- Successfully integrated RAG architecture with medical Chain-of-Thought reasoning

### Challenges

- Processing heterogeneous clinical data (structured and unstructured)
- Ensuring accuracy in criterion-level eligibility assessment
- Balancing transparency and reproducibility with clinical deployment requirements
- Handling privacy concerns in clinical data processing

### Impact on Field

TrialMatchAI demonstrates the potential of LLM-based systems with RAG architecture for patient-to-trial matching, particularly addressing the bottleneck of slow recruitment in aging populations with multimorbidity. The system's criterion-level eligibility reasoning approach provides transparency and interpretability crucial for clinical adoption. The 92% success rate in finding relevant trials for oncology patients in top-20 recommendations shows significant promise for accelerating clinical trial recruitment and improving diversity/stratification.

## Organizations

### European Clinical Research Infrastructure Network (ECRIN)
**Legal Name**: European Clinical Research Infrastructure Network
**Role in Project**: collaborator
**Role Description**: Research Collaboration Partner
**Contribution**: Clinical trial infrastructure, Oncology and clinical trials expertise
**Organization Type**: institution
**Status**: operational
**Website**: https://ecrin.org/
**Description**: Research collaboration partner. European research infrastructure network.
**Focus**: Clinical trial infrastructure, oncology and clinical trials expertise

### Netherlands Cancer Institute
**Role in Project**: collaborator
**Role Description**: Research Collaboration Partner
**Contribution**: Cancer research expertise, Oncology and clinical research, Pathology and precision medicine, Clinical trial data
**Organization Type**: institution
**Status**: operational
**Website**: https://www.nki.nl/
**Description**: Research collaboration partner. Research institute in Amsterdam, Netherlands.
**Focus**: Cancer research expertise, oncology and clinical research, pathology and precision medicine

### Centre de Bioinformatique de Bordeaux (CBiB)
**Legal Name**: Centre de Bioinformatique de Bordeaux
**Role in Project**: primary
**Role Description**: Primary development institution and project host
**Contribution**: Project leadership (Macha Nikolski), Research infrastructure, Bioinformatics expertise, Development resources
**Organization Type**: research_center
**Status**: operational
**Website**: https://www.bordeaux-bioinformatics.fr
**Description**: Primary development institution and project host for TrialMatchAI. Research center at Université de Bordeaux.
**Focus**: Bioinformatics research, computational biology, AI in healthcare
**Research Focus**: Bioinformatics, Computational biology, AI in healthcare, Clinical trial matching
**Key Achievements**:
- Development of TrialMatchAI system
- 92% success rate in patient-to-trial matching
- >90% criterion-level eligibility classification accuracy
**Director**: {"name":"Macha Nikolski","title":"Principal Investigator / Project Lead","expertise":["Bioinformatics","Computational biology","AI in healthcare","Clinical trial matching"],"background":"Principal Investigator and Project Lead of TrialMatchAI. Director or senior researcher at Centre de Bioinformatique de Bordeaux, Université de Bordeaux."}

### Université de Bordeaux
**Role in Project**: institution
**Role Description**: Parent institution and project host
**Contribution**: Project leadership, Bioinformatics, Clinical research
**Organization Type**: institution
**Status**: operational
**Website**: https://www.u-bordeaux.fr/
**Description**: Research university in Bordeaux, France. Parent institution of Centre de Bioinformatique de Bordeaux (CBiB).
**Focus**: Higher education and research

### Institut de Biochimie et Génétique Cellulaires
**Role in Project**: collaborator
**Role Description**: Research Collaboration Partner
**Contribution**: Computational biology, Bioinformatics
**Organization Type**: institution
**Status**: operational
**Description**: Research collaboration partner. Research institute in France.
**Focus**: Computational biology, bioinformatics

### Oslo University Hospital
**Role in Project**: collaborator
**Role Description**: Research Collaboration Partner
**Contribution**: Clinical informatics expertise, Clinical data analysis, Genomics and bioinformatics, Clinical validation
**Organization Type**: institution
**Status**: operational
**Website**: https://oslo-universitetssykehus.no/
**Description**: Research collaboration partner. Hospital and research institution in Oslo, Norway.
**Focus**: Clinical informatics expertise, clinical data analysis, genomics and bioinformatics

### University of Oslo
**Role in Project**: collaborator
**Role Description**: Affiliated institution
**Contribution**: Genomics, Bioinformatics
**Organization Type**: institution
**Status**: operational
**Website**: https://www.uio.no/
**Description**: University in Oslo, Norway. Affiliated institution for one researcher (Eivind Hovig).
**Focus**: Research and higher education

## Locations

### Amsterdam, Netherlands
**Type**: institution
**City**: Amsterdam
**Country**: Netherlands
**Organizations**: Netherlands Cancer Institute

### Oslo, Norway
**Type**: institution
**City**: Oslo
**Country**: Norway
**Organizations**: Oslo University Hospital, University of Oslo

### Europe
**Type**: institution
**Country**: Europe
**Organizations**: European Clinical Research Infrastructure Network (ECRIN)

### Bordeaux, France
**Type**: headquarters
**City**: Bordeaux
**State/Region**: Nouvelle-Aquitaine
**Country**: France
**Organizations**: Centre de Bioinformatique de Bordeaux (CBiB), Université de Bordeaux

### France
**Type**: institution
**Country**: France
**Organizations**: Institut de Biochimie et Génétique Cellulaires

## Products

### TrialMatchAI
**Type**: ai_model
**Status**: Research/Development
**Development Stage**: Research / Preclinical
**Role in Project**: primary
**Relationship Description**: Main AI system developed in this research project
**Description**: End-to-end AI-powered clinical trial recommendation system using Large Language Models (LLMs) within a Retrieval-Augmented Generation (RAG) architecture. The system processes heterogeneous clinical data (structured records and unstructured physician notes) to match patients with relevant clinical trials through: (1) Biomedical entity normalization, (2) Hybrid search combining lexical and semantic similarity for relevant trial retrieval, (3) Result re-ranking, (4) Criterion-level eligibility assessment using medical Chain-of-Thought (CoT) reasoning.
**Mechanism of Action**: End-to-end AI-powered clinical trial recommendation system using Large Language Models (LLMs) within a Retrieval-Augmented Generation (RAG) architecture. The system processes heterogeneous clinical data (structured records and unstructured physician notes) to match patients with relevant clinical trials through: (1) Biomedical entity normalization, (2) Hybrid search combining lexical and semantic similarity for relevant trial retrieval, (3) Result re-ranking, (4) Criterion-level eligibility assessment using medical Chain-of-Thought (CoT) reasoning.
**Target**: Clinical trial matching process
**Pathway**: Patient-to-trial matching pipeline
**Indications**: [
  {
    "primary": "Oncology clinical trials",
    "secondary": "General clinical trial matching (with focus on aging populations with multimorbidity)"
  }
]
**Clinical Trials**:
```yaml
-
  name: Real-world validation of TrialMatchAI
  phase: Validation Study
  status: Completed
  results:
  summary: Real-world validation showed that 92% of oncology patients had at least one relevant trial found in the top-20 recommendations. Evaluation on synthetic and real clinical datasets confirmed state-of-the-art performance with over 90% accuracy in criterion-level eligibility classification, particularly in biomarker-driven cases.
  primary_result: 92%
  primary_endpoint: Percentage of oncology patients with at least one relevant trial in top-20 recommendations
  validation_datasets: Synthetic and real clinical datasets
  criterion_level_accuracy: >90% accuracy in criterion-level eligibility classification, especially in biomarker-driven cases
  indication: Oncology patient-to-trial matching
  start_date: 2025
  publications:
  -
  url: "https://arxiv.org/abs/2505.08508"
  date: 2025-05-13
  type: arXiv Publication
  title: "TrialMatchAI: An End-to-End AI-powered Clinical Trial Recommendation System to Streamline Patient-to-Trial Matching"
```
**Technical Details**:
```yaml
privacy: Privacy-preserving local deployment
deployment: Modular design supporting local deployment in clinical environments
llm_models: Fine-tuned open-source Large Language Models
modularity: Seamless replacement of LLM components as more advanced models become available
data_format: Phenopackets standardized format
architecture: Retrieval-Augmented Generation (RAG)
```

## Key People

### Maria Alexandra Rujano
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Université de Bordeaux
**Contribution**: Contributing to bioinformatics
**Expertise**: Bioinformatics
**Biography**: Researcher at Université de Bordeaux, contributing to bioinformatics

### Remond Fijneman
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Netherlands Cancer Institute
**Contribution**: Contributing to cancer research
**Expertise**: Cancer research
**Biography**: Researcher at Netherlands Cancer Institute, contributing to cancer research

### Rodrigo Dienstmann
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: European Clinical Research Infrastructure Network (ECRIN)
**Contribution**: Contributing to oncology and clinical trials expertise
**Expertise**: Oncology, Clinical trials
**Biography**: Researcher at ECRIN, contributing to oncology and clinical trials expertise

### Majd Abdallah
**Title**: Lead Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, First Author
**Affiliations**: Oslo University Hospital
**Responsibilities**:
- Primary method development
- System implementation
- Data analysis and validation
- Manuscript preparation
**Contribution**: Lead researcher and first author of TrialMatchAI publication
**Expertise**: Clinical informatics, AI in healthcare, Clinical trial matching
**Biography**: Lead researcher and first author of TrialMatchAI publication. Expert in clinical informatics and AI in healthcare.

### Lana Meiqari
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Université de Bordeaux
**Contribution**: Contributing to clinical research
**Expertise**: Clinical research
**Biography**: Researcher at Université de Bordeaux, contributing to clinical research

### Gerrit Meijer
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Netherlands Cancer Institute
**Contribution**: Contributing to pathology and precision medicine expertise
**Expertise**: Pathology, Precision medicine
**Biography**: Researcher at Netherlands Cancer Institute, contributing to pathology and precision medicine expertise

### Alexis Groppi
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Institut de Biochimie et Génétique Cellulaires
**Contribution**: Contributing to computational biology
**Expertise**: Computational biology
**Biography**: Researcher at Institut de Biochimie et Génétique Cellulaires, contributing to computational biology

### Slim Karkar
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Institut de Biochimie et Génétique Cellulaires
**Contribution**: Contributing to bioinformatics
**Expertise**: Bioinformatics
**Biography**: Researcher at Institut de Biochimie et Génétique Cellulaires, contributing to bioinformatics

### Macha Nikolski
**Title**: Principal Investigator / Project Lead
**Participation Type**: pi
**Role in Project**: Principal Investigator, Corresponding Author
**Affiliations**: Université de Bordeaux, Centre de Bioinformatique de Bordeaux (CBiB)
**Responsibilities**:
- Overall project leadership
- Methodology development
- Publication lead and scientific oversight
- Grant management
- Multi-institutional collaboration coordination
**Contribution**: Principal Investigator and Project Lead of TrialMatchAI
**Expertise**: Bioinformatics, Computational biology, AI in healthcare, Clinical trial matching
**Biography**: Principal Investigator and Project Lead of TrialMatchAI. Director or senior researcher at Centre de Bioinformatique de Bordeaux, Université de Bordeaux. Expert in bioinformatics and computational biology.

### Eivind Hovig
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Oslo
**Contribution**: Contributing to genomics and bioinformatics
**Expertise**: Genomics, Bioinformatics
**Biography**: Researcher at University of Oslo, contributing to genomics and bioinformatics

### Steve Canham
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: European Clinical Research Infrastructure Network (ECRIN)
**Contribution**: Contributing to clinical trial infrastructure expertise
**Expertise**: Clinical trial infrastructure
**Biography**: Researcher at ECRIN, contributing to clinical trial infrastructure expertise

### Johanna Galvis
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Netherlands Cancer Institute
**Contribution**: Contributing to oncology and clinical research
**Expertise**: Oncology, Clinical research
**Biography**: Researcher at Netherlands Cancer Institute, contributing to oncology and clinical research

### Sigve Nakken
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Oslo University Hospital
**Contribution**: Contributing to bioinformatics and clinical data analysis
**Expertise**: Bioinformatics, Clinical data analysis
**Biography**: Researcher at Oslo University Hospital, contributing to bioinformatics and clinical data analysis

### Mariska Bierkens
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Netherlands Cancer Institute
**Contribution**: Contributing to cancer research and clinical trials expertise
**Expertise**: Cancer research, Clinical trials
**Biography**: Researcher at Netherlands Cancer Institute, contributing to cancer research and clinical trials expertise

## Links

### [GitHub - cbib/TrialMatchAI: TrialMatchAI aims to seamlessly match cancer patients to clinical trials based on their unique genomic and clinical profiles using AI](https://github.com/cbib/TrialMatchAI)
**Type**: documentation
**Relevance**: primary
**Category**: source
**Relationship Description**: Open-source code repository for TrialMatchAI system
**Publisher**: GitHub
**Description**: Open-source code repository for TrialMatchAI system

### [TrialMatchAI: Harnessing Large Language Models (LLMs) to Match Cancer Patients with Molecularly-driven Clinical Trials – Part of the European Open Science Cloud for Cancer Project](https://bordeaux-bioinformatics.fr/trialmatchai-a-new-approach-to-matching-cancer-patients-with-clinical-trials-based-on-large-language-models-llms/amp/)
**Type**: website
**Relevance**: primary
**Category**: source
**Relationship Description**: Project website describing TrialMatchAI as part of EOSC4Cancer initiative
**Publisher**: Centre de Bioinformatique de Bordeaux
**Description**: CBiB project page describing TrialMatchAI as part of EOSC4Cancer initiative

### [TrialMatchAI: An End-to-End AI-powered Clinical Trial Recommendation System to Streamline Patient-to-Trial Matching](https://arxiv.org/abs/2505.08508)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: Main publication describing the TrialMatchAI system, methodology, and validation results
**Publisher**: arXiv
**Publication Date**: 2025-05-13
**Authors**: Majd Abdallah, Sigve Nakken, Mariska Bierkens, Johanna Galvis, Alexis Groppi, Slim Karkar, Lana Meiqari, Maria Alexandra Rujano, Steve Canham, Rodrigo Dienstmann, Remond Fijneman, Eivind Hovig, Gerrit Meijer, Macha Nikolski
**Description**: Main research paper describing TrialMatchAI system, methodology, and validation results
**Metadata**:
```yaml
doi: 10.48550/arXiv.2505.08508
arxiv_id: 2505.08508
```

## Financials

### grant
**Source**: European Clinical Research Infrastructure Network (ECRIN)
**Funding Type**: Research Infrastructure Support
**Description**: Research collaboration and support from ECRIN
**Details**:
```yaml
type: Research Infrastructure Support
contributions:
  - Clinical trial infrastructure
  - Clinical trials expertise
  - Research staff support (2 researchers)
```

### grant
**Source**: Institut de Biochimie et Génétique Cellulaires
**Funding Type**: Collaborating Institution Support
**Description**: Research collaboration and support from Institut de Biochimie et Génétique Cellulaires
**Details**:
```yaml
type: Collaborating Institution Support
contributions:
  - Computational biology expertise
  - Research staff support (2 researchers)
```

### grant
**Source**: Netherlands Cancer Institute
**Funding Type**: Collaborating Institution Support
**Description**: Research collaboration and support from Netherlands Cancer Institute
**Details**:
```yaml
type: Collaborating Institution Support
contributions:
  - Cancer research expertise
  - Clinical trial data
  - Research staff support (4 researchers)
```

### grant
**Source**: Oslo University Hospital
**Funding Type**: Collaborating Institution Support
**Description**: Research collaboration and support from Oslo University Hospital
**Details**:
```yaml
type: Collaborating Institution Support
contributions:
  - Clinical informatics expertise
  - Clinical data access
  - Research staff support (Majd Abdallah, Sigve Nakken, Eivind Hovig)
```

### grant
**Source**: Université de Bordeaux / Centre de Bioinformatique de Bordeaux (CBiB)
**Funding Type**: Institutional Support
**Description**: Research infrastructure and support from host institution
**Details**:
```yaml
type: Institutional Support
contributions:
  - Research infrastructure
  - Faculty support (Macha Nikolski)
  - Computational resources
  - Laboratory facilities
  - Development resources
```

### grant
**Amount**: Not disclosed
**Source**: European Open Science Cloud for Cancer (EOSC4Cancer)
**Funding Type**: European Research Initiative
**Description**: Research project funded through EOSC4Cancer, a European initiative bringing together researchers and institutions across Europe to accelerate data-driven cancer research
**Note**: EOSC4Cancer is a European research infrastructure initiative. Specific grant amounts not publicly disclosed in available sources.
**Details**:
```yaml
type: European Research Initiative
initiative: EOSC4Cancer
```

## Events

### Open Source Release
**Date**: 2025-01-01
**Type**: launch
**Description**: TrialMatchAI code made available on GitHub (https://github.com/cbib/TrialMatchAI) as open-source software

### TrialMatchAI project launched
**Date**: 2025-01-01
**Type**: launch
**Description**: TrialMatchAI project launched as part of the European Open Science Cloud for Cancer (EOSC4Cancer) initiative

### Publication of TrialMatchAI paper on arXiv
**Date**: 2025-05-13
**Type**: publication
**Description**: Publication of TrialMatchAI paper on arXiv (2505.08508) describing the end-to-end AI-powered clinical trial recommendation system

## Partnerships

### research
**Date**: 2025-01-01
**Focus**: Primary development institution
**Description**: TrialMatchAI is developed at the Centre de Bioinformatique de Bordeaux (CBiB) at Université de Bordeaux, led by Macha Nikolski
**Partner Organizations**:
- Centre de Bioinformatique de Bordeaux (CBiB) (initiator)
  - Primary development institution
- Université de Bordeaux (initiator)
  - Host institution
**Details**:
```yaml
type: Host Institution
leader: Macha Nikolski
```

### research
**Date**: 2025-01-01
**Focus**: Clinical trial infrastructure
**Description**: Collaboration with ECRIN (Steve Canham, Rodrigo Dienstmann) for clinical trial infrastructure and expertise
**Partner Organizations**:
- European Clinical Research Infrastructure Network (ECRIN) (collaborator)
  - Research collaboration partner
**Details**:
```yaml
type: Research Collaboration
researchers:
  - Steve Canham
  - Rodrigo Dienstmann
```

### research
**Date**: 2025-01-01
**Focus**: Oncology research, clinical trials
**Description**: Collaboration with Netherlands Cancer Institute researchers (Mariska Bierkens, Johanna Galvis, Remond Fijneman, Gerrit Meijer) for oncology expertise and clinical trial data
**Partner Organizations**:
- Netherlands Cancer Institute (collaborator)
  - Research collaboration partner
**Details**:
```yaml
type: Research Collaboration
researchers:
  - Mariska Bierkens
  - Johanna Galvis
  - Remond Fijneman
  - Gerrit Meijer
```

### research
**Date**: 2025-01-01
**Focus**: Clinical validation, patient data
**Description**: Collaboration with Oslo University Hospital researchers (Majd Abdallah, Sigve Nakken, Eivind Hovig) for clinical validation and development
**Partner Organizations**:
- Oslo University Hospital (collaborator)
  - Research collaboration partner
**Details**:
```yaml
type: Research Collaboration
researchers:
  - Majd Abdallah
  - Sigve Nakken
  - Eivind Hovig
```

### research
**Date**: 2025-01-01
**Focus**: Cancer research infrastructure and data-driven oncology
**Description**: TrialMatchAI is part of the EOSC4Cancer initiative, bringing together researchers and institutions across Europe to accelerate data-driven cancer research
**Partner Organizations**:
- European Open Science Cloud for Cancer (EOSC4Cancer) (partner)
  - Funding initiative and research infrastructure
**Details**:
```yaml
type: Research Initiative
initiative: European Open Science Cloud for Cancer (EOSC4Cancer)
```
