---
id: deepscence-duke-senescence
slug: deepscence-duke-senescence
entity_type: research
status: published
data_completeness: very_high
last_researched: 2025-12-23
research_category: academic_institution
researcher: AI Assistant
version: 3.1
name: DeepScence - Single-Cell and Spatial Senescence Detection
description: DeepScence is a deep learning framework designed to identify senescent cells in single-cell and spatial transcriptomics data. The method utilizes deep neural networks trained on integrated senescence gene sets (CoreScence) to accurately call senescent cells across various experimental platforms and tissue types. This enables cross-platform, cross-tissue accuracy in senescence detection, which is critical for advancing senolytic therapies and understanding the role of senescent cells in aging and disease.
mission: To develop an AI-based method for accurately identifying senescent cells in single-cell and spatial transcriptomics data, enabling precise detection across different platforms and tissues to advance senolytic research and therapeutic development.
entity_data:
  name: DeepScence
  status: published
  mission: To develop an AI-based method for accurately identifying senescent cells in single-cell and spatial transcriptomics data, enabling precise detection across different platforms and tissues to advance senolytic research and therapeutic development.
  website: "https://biostat.duke.edu/news/new-duke-discovery-could-help-target-cells-drive-aging-and-disease"
  timeline:
  status: published
  preprint_date: 2025-04-23
  project_start: 2023-11
  publication_date: 2025-10-07
  full_name: DeepScence - Single-Cell and Spatial Senescence Detection
  description: DeepScence is a deep learning framework designed to identify senescent cells in single-cell and spatial transcriptomics data. The method utilizes deep neural networks trained on integrated senescence gene sets (CoreScence) to accurately call senescent cells across various experimental platforms and tissue types. This enables cross-platform, cross-tissue accuracy in senescence detection, which is critical for advancing senolytic therapies and understanding the role of senescent cells in aging and disease.
  research_institution:
  name: Duke University School of Medicine
  location:
  city: Durham
  state: North Carolina
  country: USA
  department: Department of Biostatistics & Bioinformatics
taxonomy:
  geography: USA
  ai_technology:
  - Predictive ML/DL
  primary_focus:
  - Senescent Cells & Senolytics
  aging_approach:
  - Senescent Cell Elimination
  target_biology:
  - General Aging/Longevity
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: academic_institution
  therapeutic_modality: []
organizations:
  -
    name: OpenAI
    role: partner
    org_type: company
    legal_name: OpenAI, L.P.
    founded: 2015
    website: "https://www.openai.com"
    status: operational
    role_description: Funding partner
    contribution_description: "OpenAI partnered with Duke University through Deep Tech @ Duke's AI for Metascience program to explore how AI can accelerate scientific discovery. This partnership provided funding for the DeepScence project."
  -
    name: Duke University School of Medicine
    role: primary
    org_type: institution
    legal_name: Duke University
    website: "https://medschool.duke.edu/"
    status: operational
    role_description: Primary research institution
    contribution_description: Duke University School of Medicine was the primary institution where DeepScence was developed. The Department of Biostatistics & Bioinformatics provided research infrastructure, faculty support, laboratory facilities, computational resources, and administrative support. Multiple departments (Pathology, Pharmacology & Cancer Biology, Medicine) collaborated on the project.
links:
  -
    url: "https://scholars.duke.edu/person/Andrew.Nixon"
    type: profile
    title: Andrew B. Nixon - Duke Scholars Profile
  -
    url: "https://scholars.duke.edu/person/Xiao-Fan.Wang"
    type: profile
    title: Xiao-Fan Wang - Duke Scholars Profile
  -
    url: "https://scholars.duke.edu/person/Carolyn.Glass"
    type: profile
    title: Carolyn Glass - Duke Scholars Profile
  -
    url: "https://deeptech.duke.edu/"
    type: website
    title: Deep Tech @ Duke University
  -
    url: "https://biostat.duke.edu/"
    type: website
    title: Duke Department of Biostatistics & Bioinformatics
  -
    url: "https://scholars.duke.edu/person/Zhicheng.Ji/publications"
    type: profile
    title: Zhicheng Ji - Publications
  -
    url: "https://pubmed.ncbi.nlm.nih.gov/38045252/"
    type: database
    title: DeepScence - PubMed Entry
  -
    url: "https://scholars.duke.edu/publication/1665707"
    type: database
    title: DeepScence Publication - Duke Scholars
  -
    url: "https://zji90.github.io/"
    type: website
    title: Zhicheng Ji Lab Website
  -
    url: "https://scholars.duke.edu/person/Zhicheng.Ji"
    type: profile
    title: Zhicheng Ji - Duke Scholars Profile
  -
    url: "https://github.com/anthony-qu/DeepScence"
    type: code_repository
    title: DeepScence GitHub Repository
  -
    url: "https://deeptech.duke.edu/news/deep-tech-duke-funds-four-ai-metascience-projects-through-openai-partnership/"
    type: press_release
    title: Deep Tech @ Duke Funds Four AI for Metascience Projects Through OpenAI Partnership
  -
    url: "https://biostat.duke.edu/news/new-duke-discovery-could-help-target-cells-drive-aging-and-disease"
    type: press_release
    title: A New Duke Discovery Could Help Target the Cells That Drive Aging and Disease
  -
    url: "https://www.biorxiv.org/content/10.1101/2023.11.21.568150v1"
    type: preprint
    title: Single-cell and spatial detection of senescent cells using DeepScence (preprint)
  -
    url: "https://www.sciencedirect.com/science/article/pii/S2666979X25002915"
    type: research_publication
    title: Single-cell and spatial detection of senescent cells using DeepScence
---

# DeepScence - Single-Cell and Spatial Senescence Detection

## Description

DeepScence is a deep learning framework designed to identify senescent cells in single-cell and spatial transcriptomics data. The method utilizes deep neural networks trained on integrated senescence gene sets (CoreScence) to accurately call senescent cells across various experimental platforms and tissue types. This enables cross-platform, cross-tissue accuracy in senescence detection, which is critical for advancing senolytic therapies and understanding the role of senescent cells in aging and disease.

## Mission

To develop an AI-based method for accurately identifying senescent cells in single-cell and spatial transcriptomics data, enabling precise detection across different platforms and tissues to advance senolytic research and therapeutic development.

## Project Information


## Scientific Background

```yaml
innovation:
  core_innovation: "DeepScence combines two key innovations: (1) CoreScence - a curated gene set representing consensus senescence markers, and (2) an autoencoder-based deep neural network that transforms genetic signals into both continuous scores and binary classifications"
  practical_impact: The cross-platform and cross-tissue accuracy of DeepScence enables researchers to use the method across different experimental setups with confidence
  technical_advancement: The use of autoencoder architecture enables the model to learn compressed representations of senescence patterns while providing both continuous and binary outputs
existing_methods:
  comparison: DeepScence addresses these limitations by integrating multiple senescence gene sets and using deep learning to achieve cross-platform, cross-tissue accuracy
  limitations:
  - Existing methods for senescence detection are often platform-specific
  - Lack cross-tissue and cross-platform accuracy
  - Cannot accurately identify senescent cells at single-cell and spatial resolution
  - Often rely on single gene sets that may not capture the full heterogeneity of senescence
problem_statement: Cellular senescence is a heterogeneous and rare cellular state. Traditional methods cannot accurately identify senescent cells at single-cell and spatial resolution, which undermines senolytic development. Mislabeling of senescent cells creates significant challenges for research and therapeutic development.
historical_context:
  senescence_research: Research into cellular senescence has accelerated in recent years due to its role in aging and age-related diseases
  measurement_bottleneck: The lack of accurate, cross-platform methods for senescence detection has been a critical bottleneck in advancing senolytic research
  senolytic_therapeutics: The development of senolytic drugs (drugs that eliminate senescent cells) requires accurate identification of senescent cells to target them effectively
biological_justification:
  gene_set_integration: By integrating multiple published senescence gene sets into CoreScence, DeepScence captures the consensus markers of senescence while accounting for heterogeneity
  deep_learning_advantage: Deep learning allows the model to learn complex patterns in gene expression that may not be captured by simple threshold-based methods
  senescence_heterogeneity: Cellular senescence is not a uniform state but rather a heterogeneous condition with different subtypes and markers depending on cell type, tissue context, and senescence trigger
```

## Lessons Learned

### Achievements

- Successfully developed deep neural network approach for senescence detection
- Achieved cross-platform and cross-tissue accuracy
- Published in high-impact journal (Cell Genomics)
- Integrated multiple senescence gene sets into CoreScence foundation
- Enabled precise single-cell and spatial resolution detection

### Challenges

- Senescence is heterogeneous and rare, making accurate identification challenging
- Traditional methods cannot accurately identify senescent cells at single-cell and spatial resolution
- Mislabeling of senescent cells undermines senolytic development
- Need for cross-platform and cross-tissue validation

### Impact on Field

DeepScence addresses a critical measurement bottleneck in senescence research. By providing accurate, cross-platform, cross-tissue detection of senescent cells at single-cell and spatial resolution, it enables targeted senolytic trials and advances the field of senolytic therapeutics. The method unlocks senolytics and pro-youth remodeling at scale by providing the precise measurement capabilities needed for effective senolytic development.

## Organizations

### OpenAI
**Legal Name**: OpenAI, L.P.
**Role in Project**: partner
**Role Description**: Funding partner
**Contribution**: OpenAI partnered with Duke University through Deep Tech @ Duke's AI for Metascience program to explore how AI can accelerate scientific discovery. This partnership provided funding for the DeepScence project.
**Organization Type**: company
**Status**: operational
**Founded**: 2015
**Website**: https://www.openai.com
**Description**: AI research company specializing in large language models and AI applications for life sciences
**Focus**: Artificial Intelligence, Large Language Models, Life Sciences Research

### Duke University School of Medicine
**Legal Name**: Duke University
**Role in Project**: primary
**Role Description**: Primary research institution
**Contribution**: Duke University School of Medicine was the primary institution where DeepScence was developed. The Department of Biostatistics & Bioinformatics provided research infrastructure, faculty support, laboratory facilities, computational resources, and administrative support. Multiple departments (Pathology, Pharmacology & Cancer Biology, Medicine) collaborated on the project.
**Organization Type**: institution
**Status**: operational
**Website**: https://medschool.duke.edu/
**Description**: Duke University School of Medicine is a leading institution dedicated to advancing medical knowledge and improving human health through research, education, and patient care. The Department of Biostatistics & Bioinformatics was the primary department for the DeepScence project.
**Focus**: Medical research, education, and patient care

## Locations

### OpenAI Headquarters
**Type**: headquarters
**Address**: 3180 18th Street, San Francisco, California
**City**: San Francisco
**State/Region**: California
**Country**: USA
**Organizations**: OpenAI

### Duke University School of Medicine
**Type**: institution
**Address**: Duke University School of Medicine, 10 Searle Drive, Durham, NC 27710, USA
**City**: Durham
**State/Region**: North Carolina
**Country**: USA
**Organizations**: Duke University School of Medicine

## Key People

### Zhicheng Ji
**Title**: Assistant Professor
**Participation Type**: pi
**Role in Project**: Principal Investigator
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Principal Investigator leading overall project leadership, research direction, methodology development, publication, grant management, and lab coordination
**Expertise**: Single-cell genomics, Computational biology, Deep learning, Transcriptomics
**Biography**: Assistant Professor of Biostatistics & Bioinformatics at Duke University, leading research in single-cell genomics and computational biology. Principal Investigator of the DeepScence project. Lab website: https://zji90.github.io/
**Profile**: https://scholars.duke.edu/person/Zhicheng.Ji
**Email**: zhicheng.ji@duke.edu

### Andrew B. Nixon
**Title**: Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Medicine, Duke University
**Contribution**: Professor of Medicine providing clinical expertise for applications of senescence detection in clinical settings
**Expertise**: Medicine, Clinical applications, Senescence detection
**Biography**: Professor of Medicine providing clinical expertise for applications of senescence detection in clinical settings
**Profile**: https://scholars.duke.edu/person/Andrew.Nixon
**Email**: andrew.nixon@duke.edu

### Xiao-Fan Wang
**Title**: Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Pharmacology & Cancer Biology, Duke University
**Contribution**: Professor of Pharmacology & Cancer Biology providing expertise in cancer-related senescence research
**Expertise**: Pharmacology, Cancer Biology, Senescence research
**Biography**: Professor of Pharmacology & Cancer Biology providing expertise in cancer-related senescence research
**Profile**: https://scholars.duke.edu/person/Xiao-Fan.Wang
**Email**: xiaofan.wang@duke.edu

### Carolyn Glass
**Title**: Associate Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Pathology, Duke University
**Contribution**: Associate Professor of Pathology providing clinical and pathological expertise for senescence research applications
**Expertise**: Pathology, Clinical expertise, Senescence research
**Biography**: Associate Professor of Pathology providing clinical and pathological expertise for senescence research applications
**Profile**: https://scholars.duke.edu/person/Carolyn.Glass
**Email**: carolyn.glass@duke.edu

### Jichun Xie
**Title**: Associate Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Associate Professor providing expertise in biostatistics and bioinformatics
**Expertise**: Biostatistics, Bioinformatics
**Biography**: Associate Professor providing expertise in biostatistics and bioinformatics
**Profile**: https://scholars.duke.edu/person/Jichun.Xie

### Cliburn Chan
**Title**: Associate Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Associate Professor providing expertise in biostatistics and computational methods
**Expertise**: Biostatistics, Computational methods
**Biography**: Associate Professor providing expertise in biostatistics and computational methods
**Profile**: https://scholars.duke.edu/person/Cliburn.Chan

### Liangcai Gu
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Researcher contributing to computational analysis and validation
**Biography**: Researcher contributing to computational analysis and validation

### Runze Dong
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Researcher contributing to method development and validation
**Biography**: Researcher contributing to method development and validation

### Beijie Ji
**Title**: PhD Student
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: PhD student contributing to DeepScence development and validation
**Biography**: PhD student contributing to DeepScence development and validation

### Yilong Qu
**Title**: Researcher
**Participation Type**: researcher
**Role in Project**: Lead Researcher, First Author
**Affiliations**: Duke University School of Medicine, Department of Biostatistics & Bioinformatics, Duke University
**Contribution**: Lead researcher and first author responsible for primary method development, code implementation, data analysis, validation, and manuscript preparation
**Biography**: First author of DeepScence publication. Lead researcher responsible for method development and implementation. Primary contributions: method development, code implementation, data analysis and validation, manuscript preparation. GitHub repository: https://github.com/anthony-qu/DeepScence

## Links

### [Andrew B. Nixon - Duke Scholars Profile](https://scholars.duke.edu/person/Andrew.Nixon)
**Type**: profile
**Relevance**: secondary
**Category**: profile
**Relationship Description**: Academic profile of co-author Andrew B. Nixon
**Publisher**: Duke University
**Description**: Academic profile of co-author Andrew B. Nixon

### [Xiao-Fan Wang - Duke Scholars Profile](https://scholars.duke.edu/person/Xiao-Fan.Wang)
**Type**: profile
**Relevance**: secondary
**Category**: profile
**Relationship Description**: Academic profile of co-author Xiao-Fan Wang
**Publisher**: Duke University
**Description**: Academic profile of co-author Xiao-Fan Wang

### [Carolyn Glass - Duke Scholars Profile](https://scholars.duke.edu/person/Carolyn.Glass)
**Type**: profile
**Relevance**: secondary
**Category**: profile
**Relationship Description**: Academic profile of co-author Carolyn Glass
**Publisher**: Duke University
**Description**: Academic profile of co-author Carolyn Glass

### [Deep Tech @ Duke University](https://deeptech.duke.edu/)
**Type**: website
**Relevance**: secondary
**Category**: website
**Relationship Description**: Deep Tech @ Duke initiative supporting multidisciplinary research
**Publisher**: Duke University
**Description**: Deep Tech @ Duke initiative supporting multidisciplinary research

### [Duke Department of Biostatistics & Bioinformatics](https://biostat.duke.edu/)
**Type**: website
**Relevance**: secondary
**Category**: website
**Relationship Description**: Official website of the Department of Biostatistics & Bioinformatics at Duke
**Publisher**: Duke University
**Description**: Official website of the Department of Biostatistics & Bioinformatics at Duke

### [Zhicheng Ji - Publications](https://scholars.duke.edu/person/Zhicheng.Ji/publications)
**Type**: profile
**Relevance**: secondary
**Category**: profile
**Relationship Description**: List of publications by Principal Investigator Zhicheng Ji
**Publisher**: Duke University
**Description**: List of publications by Principal Investigator Zhicheng Ji

### [DeepScence - PubMed Entry](https://pubmed.ncbi.nlm.nih.gov/38045252/)
**Type**: database
**Relevance**: secondary
**Category**: database
**Relationship Description**: PubMed database entry for the DeepScence publication
**Publisher**: PubMed
**Publication Date**: 2025-10-07
**Description**: PubMed database entry for the DeepScence publication in Cell Genomics

### [DeepScence Publication - Duke Scholars](https://scholars.duke.edu/publication/1665707)
**Type**: database
**Relevance**: secondary
**Category**: database
**Relationship Description**: Duke Scholars database entry for the DeepScence publication
**Publisher**: Duke University
**Description**: Duke Scholars database entry for the DeepScence publication

### [Zhicheng Ji Lab Website](https://zji90.github.io/)
**Type**: website
**Relevance**: secondary
**Category**: website
**Relationship Description**: Laboratory website of Zhicheng Ji at Duke University
**Publisher**: Duke University
**Description**: Laboratory website of Zhicheng Ji at Duke University

### [Zhicheng Ji - Duke Scholars Profile](https://scholars.duke.edu/person/Zhicheng.Ji)
**Type**: profile
**Relevance**: secondary
**Category**: profile
**Relationship Description**: Academic profile of Principal Investigator Zhicheng Ji
**Publisher**: Duke University
**Description**: Academic profile of Principal Investigator Zhicheng Ji

### [DeepScence GitHub Repository](https://github.com/anthony-qu/DeepScence)
**Type**: code_repository
**Relevance**: primary
**Category**: code
**Relationship Description**: Open-source implementation of DeepScence on GitHub
**Publisher**: GitHub
**Description**: Open-source implementation of DeepScence on GitHub, allowing researchers to use the tool

### [Deep Tech @ Duke Funds Four AI for Metascience Projects Through OpenAI Partnership](https://deeptech.duke.edu/news/deep-tech-duke-funds-four-ai-metascience-projects-through-openai-partnership/)
**Type**: press_release
**Relevance**: primary
**Category**: news
**Relationship Description**: Announcement of funding for DeepScence project through OpenAI partnership
**Publisher**: Deep Tech @ Duke
**Publication Date**: 2025-07-09
**Description**: Announcement of funding for DeepScence project through OpenAI partnership

### [A New Duke Discovery Could Help Target the Cells That Drive Aging and Disease](https://biostat.duke.edu/news/new-duke-discovery-could-help-target-cells-drive-aging-and-disease)
**Type**: press_release
**Relevance**: primary
**Category**: news
**Relationship Description**: Duke University press release announcing the DeepScence discovery
**Publisher**: Duke University
**Publication Date**: 2025-10-17
**Description**: Duke University press release announcing the DeepScence discovery

### [Single-cell and spatial detection of senescent cells using DeepScence (preprint)](https://www.biorxiv.org/content/10.1101/2023.11.21.568150v1)
**Type**: preprint
**Relevance**: primary
**Category**: publication
**Relationship Description**: Preprint version published on bioRxiv
**Publisher**: bioRxiv
**Publication Date**: 2025-04-23
**Description**: Preprint version published on bioRxiv before peer review in Cell Genomics. DOI: 10.1101/2023.11.21.568150

### [Single-cell and spatial detection of senescent cells using DeepScence](https://www.sciencedirect.com/science/article/pii/S2666979X25002915)
**Type**: research_publication
**Relevance**: primary
**Category**: publication
**Relationship Description**: Main peer-reviewed publication in Cell Genomics
**Publisher**: Cell Genomics
**Publication Date**: 2025-10-07
**Description**: Main publication in Cell Genomics describing the DeepScence method. DOI: 10.1016/j.xgen.2025.101035. Duke Scholars: https://scholars.duke.edu/publication/1665707

## Financials

### partnership_deal
**Amount**: Not disclosed USD
**Funding Date**: 2025-07-09
**Period**: 2025-ongoing
**Source**: Deep Tech @ Duke University / OpenAI
**Funding Type**: Partnership Grant
**Description**: Funding provided through the Artificial Intelligence (AI) for Metascience research program, a partnership between Duke University and OpenAI to explore how AI can accelerate scientific discovery
**Details**:
```yaml
note: Specific grant amount not publicly disclosed. OpenAI partnership details may be confidential.
partner: OpenAI
program: AI for Metascience Research Program
announcement_date: 2025-07-09
institutional_support:
  department:
  name: Department of Biostatistics & Bioinformatics
  contributions:
  - Faculty appointment
  - Research infrastructure
  - Computational resources
  - Student support
  duke_university:
  contributions:
  - Research infrastructure
  - Faculty support
  - Laboratory facilities
  - Computational resources
  - Administrative support
  - Student support
```

## Partnerships

### research
**Date**: 2025-07-09
**Focus**: AI for Metascience, accelerating scientific discovery
**Description**: Partnership through Deep Tech @ Duke's AI for Metascience program to explore how AI can accelerate scientific discovery
**Partner Organizations**:
- OpenAI (partner)
**Details**:
```yaml
status: ongoing
program: AI for Metascience Research Program
funding_provided: true
partner_organization: OpenAI
funding_amount_disclosed: false
```
