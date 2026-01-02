---
id: nyu-nmp-senescence
slug: nyu-nmp-senescence
entity_type: research
status: operational
data_completeness: very_high
last_researched: 2025-01-27
research_category: academic_institution
researcher: AI Assistant
version: 3.2
name: Nuclear Morphometric Pipeline (NMP) for Senescent Cell Detection
description: NMP is an in silico, machine learning-based platform developed to rapidly and accurately identify senescent cells (SnCs) for diagnostic and therapeutic applications across various disease contexts. The pipeline utilizes unsupervised machine learning algorithms to detect and quantify nuclear morphologies (size, circularity, foci, and DAPI intensity) in tissues known to contain senescent cells. These morphologies are dimensionally reduced and scored to produce a novel Senescence Score that can identify senescent cells with high accuracy.
entity_data:
  results:
  cost: Less than $100 for reagents (DAPI and PBS) per sample, assuming availability of microscopes and computer workstations
  speed: Senescence scores can be generated within 24 hours from sample imaging to score readout
  accuracy: More accurate than traditional biomarker-based approaches (e.g., SA-β-galactosidase staining). The method demonstrates high accuracy in identifying senescent cells based on conserved nuclear morphometric features.
  validation: Demonstrated 10-fold increase in senescent chondrocytes in aged mouse cartilage with osteoarthritis compared to young healthy tissues. Successfully validated on skeletal muscle and cartilage tissues from mice, showing ability to identify senescent cells in regenerating skeletal muscle and arthritic joint cartilage.
  reproducibility: Consistent performance across different tissue types (skeletal muscle, cartilage) and cell types due to nuclear morphometric-based analysis that is conserved across biological contexts
  tissue_validation: Validated on multiple tissue types including skeletal muscle and cartilage, demonstrating versatility and broad applicability
  comparison_with_baseline: The computational approach is simpler to use, more reproducible, and more accurate than traditional biomarker-based methods such as SA-β-galactosidase staining
  objectives:
  - Diagnostic identification of senescent cells
  - Therapeutic targeting of senescent cells
  - Assessment of senolytic drug efficiency
  - Biomarker for biological organ age
  - Cell-specific druggable mechanism identification
  methodology: "The NMP uses unsupervised machine learning algorithms to analyze nuclear morphologies in skeletal muscle and cartilage tissues. The pipeline follows a multi-step process: (1) High-resolution imaging of tissue samples stained with DAPI (4',6-diamidino-2-phenylindole), (2) Automated nuclear segmentation and feature extraction, (3) Quantification of key morphometric features including nuclear size (area), circularity, presence of dense foci, and DAPI staining intensity, (4) Dimensionality reduction of morphometric features using unsupervised machine learning, (5) Generation of a Senescence Score through scoring algorithms that integrate the reduced-dimensional features. The method analyzes specific nuclear morphological changes characteristic of senescent cells: increased nuclear size, appearance of dense foci, decreased circularity, and reduced DAPI staining intensity. These features are conserved across cell types, tissue contexts, and mechanisms of senescence induction, making the approach robust and reproducible."
  publication_date: 2025-07-07
  collaboration_period: 2020-present
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
  development_stage: published
  organization_type: research
  organization_subtype: academic_institution
  therapeutic_modality: []
organizations:
  -
    name: NYU Langone Health
    role: primary
    org_type: institution
    legal_name: NYU Langone Hospitals
    founded: 1841
    website: "https://nyulangone.org"
    status: operational
  -
    name: NYU Tandon School of Engineering
    role: collaborator
    org_type: institution
    status: operational
products:
  -
    name: Nuclear Morphometric Pipeline (NMP)
    type: platform
    status: Proof-of-concept completed
    development_stage: Research / Preclinical
links:
  -
    url: "https://med.nyu.edu/faculty/michael-wosczyna"
    type: other
    title: Michael N. Wosczyna - Faculty Profile
  -
    url: "https://nyulangone.org/news/ai-assisted-technique-can-measure-track-aging-cells"
    type: press_release
    title: AI-Assisted Technique Can Measure & Track Aging Cells
  -
    url: "https://www.labmedica.com/pathology/articles/294805766/ai-assisted-technique-tracks-cells-damaged-from-injury-aging-and-disease.html"
    type: news_article
    title: AI-Assisted Technique Tracks Cells Damaged from Injury, Aging and Disease
  -
    url: "https://www.nature.com/nature-index/article/10.1038/s41467-025-60975-z"
    type: research_publication
    title: Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age - Nature Index
  -
    url: "https://pubmed.ncbi.nlm.nih.gov/40624008/"
    type: research_publication
    title: Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age - PubMed
  -
    url: "https://www.labmedica.com/technology/articles/294805780/ai-assisted-technique-tracks-cells-damaged-from-injury-aging-and-disease.html"
    type: news_article
    title: AI-Assisted Technique Tracks Cells Damaged from Injury, Aging and Disease - LabMedica Technology
  -
    url: "https://license.tov.med.nyu.edu/product/in-silico-machine-learning-based-platform-to-identify-disease-causing-senescent-cells"
    type: other
    title: In Silico, Machine Learning-Based Platform to Identify Disease-Causing Senescent Cells
  -
    url: "https://www.industryintel.com/news/nyu-langone-health-develops-ai-assisted-technique-to-measure-aging-cells-in-tissues-system-analyzes-nuclear-changes-to-track-senescent-cell-progression-in-disease-and-repair-171720887016"
    type: news_article
    title: NYU Langone Health Develops AI-Assisted Technique to Measure Aging Cells
  -
    url: "https://www.nature.com/articles/s41467-025-60975-z"
    type: research_publication
    title: Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age
  -
    url: "https://www.genengnews.com/topics/artificial-intelligence/ai-approach-tracks-cell-senescence-using-nuclear-morphology/"
    type: news_article
    title: AI Approach Tracks Cell Senescence Using Nuclear Morphology
---

# Nuclear Morphometric Pipeline (NMP) for Senescent Cell Detection

## Description

NMP is an in silico, machine learning-based platform developed to rapidly and accurately identify senescent cells (SnCs) for diagnostic and therapeutic applications across various disease contexts. The pipeline utilizes unsupervised machine learning algorithms to detect and quantify nuclear morphologies (size, circularity, foci, and DAPI intensity) in tissues known to contain senescent cells. These morphologies are dimensionally reduced and scored to produce a novel Senescence Score that can identify senescent cells with high accuracy.

## Project Information

**Publication Date**: 2025-07-07
**Objectives**: Diagnostic identification of senescent cells,Therapeutic targeting of senescent cells,Assessment of senolytic drug efficiency,Biomarker for biological organ age,Cell-specific druggable mechanism identification
**Methodology**: The NMP uses unsupervised machine learning algorithms to analyze nuclear morphologies in skeletal muscle and cartilage tissues. The pipeline follows a multi-step process: (1) High-resolution imaging of tissue samples stained with DAPI (4',6-diamidino-2-phenylindole), (2) Automated nuclear segmentation and feature extraction, (3) Quantification of key morphometric features including nuclear size (area), circularity, presence of dense foci, and DAPI staining intensity, (4) Dimensionality reduction of morphometric features using unsupervised machine learning, (5) Generation of a Senescence Score through scoring algorithms that integrate the reduced-dimensional features. The method analyzes specific nuclear morphological changes characteristic of senescent cells: increased nuclear size, appearance of dense foci, decreased circularity, and reduced DAPI staining intensity. These features are conserved across cell types, tissue contexts, and mechanisms of senescence induction, making the approach robust and reproducible.
**Results**: [object Object]
**Collaboration Period**: 2020-present

## AI Methods

- Unsupervised machine learning
- Dimensionality reduction
- Nuclear morphometric analysis
- Image analysis and computer vision

## Scientific Background

```yaml
nmp_approach: "The Nuclear Morphometric Pipeline uses machine learning to analyze nuclear morphology features (size, circularity, foci, DAPI intensity) that are characteristic of senescent cells. This computational approach is simpler to use, more reproducible, and more accurate than traditional biomarker-based methods such as SA-β-galactosidase staining. The method analyzes specific nuclear morphological changes: increased nuclear size, appearance of dense foci, decreased circularity, and reduced DAPI staining intensity."
historical_context: Existing methods for detecting and analyzing senescent cells are complex to use and insufficiently accurate for real-time monitoring. NMP addresses this gap by providing a computational, morphometric-based approach that is simpler, faster, and more accurate than traditional biomarker-based methods.
senescence_mechanism: Cellular senescence is a state in which cells stop dividing and enter a state of permanent growth arrest. Senescent cells accumulate with age and secrete pro-inflammatory factors that contribute to age-related diseases. These cells play crucial roles in wound healing processes and age-related diseases such as cancer and cardiovascular disease, but over time can contribute to tissue degeneration.
morphometric_analysis: Nuclear morphometric features are conserved across cell types, tissue contexts, and mechanisms of senescence induction, making NMP a robust tool for senescent cell identification across diverse biological contexts. This conservation allows the method to be applied universally across different cell types and tissues.
biological_significance: Tracking senescent cells provides valuable insights into how tissues lose regenerative capacity over time and how these cells contribute to disease progression. NMP enables researchers to study senescent cells and test the effectiveness of therapeutic agents, such as senolytics, in various tissues and pathologies.
machine_learning_application: Unsupervised machine learning algorithms are applied to detect and quantify nuclear morphologies, which are then dimensionally reduced and scored to produce a Senescence Score that can identify senescent cells with high accuracy. The approach eliminates the need for labeled training data by using unsupervised learning to discover patterns in nuclear morphology.
comparison_with_existing_methods:
  advantages: NMP offers advantages in speed (24-hour turnaround), cost (less than $100 per sample), reproducibility, and accuracy compared to traditional methods.
  molecular_biomarkers: Unlike molecular biomarkers (p16, p21) that require specific antibodies and may vary by cell type, NMP uses conserved morphometric features that work across diverse cell types.
  sa_beta_galactosidase: Traditional SA-β-galactosidase staining is complex to use and less accurate. NMP provides a more accurate, cost-effective, and reproducible alternative.
```

## Performance Metrics

```yaml
cost: Less than $100 for reagents (DAPI and PBS) per sample, assuming availability of microscopes and computer workstations
speed: Senescence scores can be generated within 24 hours from sample imaging to score readout
accuracy: More accurate than traditional biomarker-based approaches (e.g., SA-β-galactosidase staining). The method demonstrates high accuracy in identifying senescent cells based on conserved nuclear morphometric features.
validation: Demonstrated 10-fold increase in senescent chondrocytes in aged mouse cartilage with osteoarthritis compared to young healthy tissues. Successfully validated on skeletal muscle and cartilage tissues from mice, showing ability to identify senescent cells in regenerating skeletal muscle and arthritic joint cartilage.
reproducibility: Consistent performance across different tissue types (skeletal muscle, cartilage) and cell types due to nuclear morphometric-based analysis that is conserved across biological contexts
tissue_validation: Validated on multiple tissue types including skeletal muscle and cartilage, demonstrating versatility and broad applicability
comparison_with_baseline: The computational approach is simpler to use, more reproducible, and more accurate than traditional biomarker-based methods such as SA-β-galactosidase staining
```

## Lessons Learned

### Achievements

- Successfully developed a machine learning-based pipeline for senescent cell detection
- Demonstrated that nuclear morphometric features can reliably identify senescent cells
- Showed 10-fold increase in senescent cells in aged tissues compared to young tissues
- Published high-impact research in Nature Communications
- Created a cost-effective and rapid method for senescent cell identification

### Challenges

- Need for validation in human tissues
- Integration with other biomarker tools for comprehensive senescent cell detection
- Translation from preclinical to clinical applications

### Impact on Field

The NMP represents a significant advancement in senescent cell detection methodology, providing a more accurate, cost-effective, and reproducible alternative to traditional biomarker-based approaches. This technology has the potential to accelerate research in aging and age-related diseases by enabling rapid identification and quantification of senescent cells across diverse tissue types.

## Organizations

### NYU Langone Health
**Legal Name**: NYU Langone Hospitals
**Role in Project**: primary
**Organization Type**: institution
**Status**: operational
**Founded**: 1841
**Website**: https://nyulangone.org
**Description**: NYU Langone Health is a world-class, patient-centered, integrated academic medical center, known for its excellence in clinical care, research, and education. It includes NYU Grossman School of Medicine and a network of hospitals and ambulatory care centers.
**Focus**: Medical research, education, and clinical care. AI-driven senescent cell detection and aging research.

### NYU Tandon School of Engineering
**Role in Project**: collaborator
**Organization Type**: institution
**Status**: operational
**Description**: Engineering school at New York University providing engineering expertise and computational resources for the SenoTrack AI project
**Focus**: Engineering education and research, machine learning, computational biology

## Locations

### NYU Langone Health Headquarters
**Type**: institution
**Address**: New York, NY, USA
**City**: New York
**State/Region**: New York
**Country**: USA
**Organizations**: NYU Langone Health

## Products

### Nuclear Morphometric Pipeline (NMP)
**Type**: platform
**Status**: Proof-of-concept completed
**Development Stage**: Research / Preclinical
**Description**: NMP is an in silico, machine learning-based platform developed to rapidly and accurately identify senescent cells (SnCs) for diagnostic and therapeutic applications across various disease contexts. The pipeline utilizes unsupervised machine learning algorithms to detect and quantify nuclear morphologies (size, circularity, foci, and DAPI intensity) in tissues known to contain senescent cells. These morphologies are dimensionally reduced and scored to produce a novel Senescence Score that can identify senescent cells with high accuracy.
**Capabilities**:
- Diagnostic identification of senescent cells
- Therapeutic targeting of senescent cells
- Assessment of senolytic drug efficiency
- Biomarker for biological organ age
- Cell-specific druggable mechanism identification
**Applications**:
- Diagnostic identification of senescent cells
- Therapeutic targeting of senescent cells
- Assessment of senolytic drug efficiency
- Biomarker for biological organ age
- Cell-specific druggable mechanism identification
**Technical Details**:
```yaml
advantages:
  - "Rapid and cost-effective methodology: results within 24 hours with minimal reagent costs (less than $100 per sample)"
  - Consistent and reproducible analysis across different tissue types due to nuclear morphometric-based analysis
  - High accuracy and applicability across multiple cell types (stem cells, endothelial cells, chondrocytes, muscle cells, etc.)
  - More accurate than traditional biomarker-based approaches (e.g., SA-β-galactosidase)
  - Simple to use and highly reproducible computational approach
  - Conserved morphometric features across cell types, tissue contexts, and senescence induction mechanisms
  - Applicable to various disease contexts and tissue types
indications:
  -
    primary: Age-related diseases
    specific:
    - Osteoarthritis
    - Sarcopenia
    - Neurodegenerative diseases
    - Age-related lipodystrophy
    - Cancer
    - Muscular dystrophy
    - Renal dysfunction
    - Osteoporosis
    - COPD
    - Cirrhosis
    - Cataracts
    - Atherosclerosis
    - Idiopathic pulmonary fibrosis
    - Premature aging
    - Other age-related disorders
limitations:
  - Currently validated primarily in mouse tissues; human tissue validation needed
  - Requires high-resolution imaging equipment and computational resources
  - Specific algorithm details and training parameters not fully disclosed
  - May need integration with other biomarker tools for comprehensive senescent cell detection
  - Translation from preclinical to clinical applications requires further validation
alternative_names:
  - NMP
  - Nuclear Morphometric Pipeline for Senescent Cell Detection
cell_types_applicable:
  - Stem cells
  - Fibroadipogenic progenitor cells
  - Endothelial cells
  - Skeletal muscle cells
  - Chondrocytes
  - Immune cells
  - Myoblasts
  - Adipocytes
  - Epithelial cells
```

## Key People

### Vikrant Piprode
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Fengyuan Liu
**Participation Type**: researcher
**Biography**: Researcher at NYU Langone Health

### Katerina Petroff
**Participation Type**: researcher
**Biography**: Researcher at NYU Langone Health

### Edgar Perez Carbajal
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Sahil A. Mapkar
**Title**: Doctoral Candidate
**Participation Type**: researcher
**Expertise**: Machine learning, computational biology, image analysis
**Biography**: Graduate student working on machine learning applications in biology

### Zhiru Li
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Sarah Bliss
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Anna Wilson
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Michael N. Wosczyna
**Title**: Assistant Professor
**Participation Type**: pi
**Expertise**: Muscle regeneration, senescent cell biology, aging research
**Biography**: Researcher in muscle regeneration, cellular senescence, and aging
**Profile**: https://med.nyu.edu/faculty/michael-wosczyna

### Youjin Lee
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

### Thorsten Kirsch
**Participation Type**: researcher
**Biography**: Researcher at NYU Langone Health

### Sean Murray
**Participation Type**: researcher
**Biography**: Researcher in the Wosczyna lab

## Links

### [Michael N. Wosczyna - Faculty Profile](https://med.nyu.edu/faculty/michael-wosczyna)
**Type**: other
**Description**: NYU Grossman School of Medicine faculty profile for Principal Investigator Michael N. Wosczyna

### [AI-Assisted Technique Can Measure & Track Aging Cells](https://nyulangone.org/news/ai-assisted-technique-can-measure-track-aging-cells)
**Type**: press_release
**Publication Date**: 2025-07-07
**Description**: NYU Langone Health news release announcing the development of AI-assisted technique for measuring and tracking aging cells

### [AI-Assisted Technique Tracks Cells Damaged from Injury, Aging and Disease](https://www.labmedica.com/pathology/articles/294805766/ai-assisted-technique-tracks-cells-damaged-from-injury-aging-and-disease.html)
**Type**: news_article
**Publication Date**: 2025-07-08
**Description**: LabMedica article covering the AI-assisted technique announcement

### [Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age - Nature Index](https://www.nature.com/nature-index/article/10.1038/s41467-025-60975-z)
**Type**: research_publication
**Publication Date**: 2025-07-07
**Description**: Nature Index article about the NMP publication, including information about the research team from five institutions

### [Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age - PubMed](https://pubmed.ncbi.nlm.nih.gov/40624008/)
**Type**: research_publication
**Publication Date**: 2025-07-07
**Description**: PubMed entry for the Nature Communications publication (PubMed ID: 40624008)

### [AI-Assisted Technique Tracks Cells Damaged from Injury, Aging and Disease - LabMedica Technology](https://www.labmedica.com/technology/articles/294805780/ai-assisted-technique-tracks-cells-damaged-from-injury-aging-and-disease.html)
**Type**: news_article
**Publication Date**: 2025-07-07
**Description**: LabMedica Technology article covering NMP development and applications

### [In Silico, Machine Learning-Based Platform to Identify Disease-Causing Senescent Cells](https://license.tov.med.nyu.edu/product/in-silico-machine-learning-based-platform-to-identify-disease-causing-senescent-cells)
**Type**: other
**Description**: NYU Technology Opportunities & Ventures licensing page for related NMP technology

### [NYU Langone Health Develops AI-Assisted Technique to Measure Aging Cells](https://www.industryintel.com/news/nyu-langone-health-develops-ai-assisted-technique-to-measure-aging-cells-in-tissues-system-analyzes-nuclear-changes-to-track-senescent-cell-progression-in-disease-and-repair-171720887016)
**Type**: news_article
**Publication Date**: 2025-07-07
**Description**: IndustryIntel article providing details about the NMP technology, research team, and funding (NIH grant R01AG053438)

### [Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age](https://www.nature.com/articles/s41467-025-60975-z)
**Type**: research_publication
**Publisher**: Nature Communications
**Publication Date**: 2025-07-07
**Authors**: Sahil A. Mapkar, Sarah Bliss, Edgar Perez Carbajal, Sean Murray, Zhiru Li, Anna Wilson, Vikrant Piprode, Youjin Lee, Thorsten Kirsch, Katerina Petroff, Fengyuan Liu, Michael N. Wosczyna
**Description**: Primary research publication in Nature Communications describing the AI-assisted technique for senescent cell detection and tracking. This publication is closely related to SenoTrack AI methodology.
**Metadata**:
```yaml
doi: 10.1038/s41467-025-60975-z
type: Research Article
journal: Nature Communications
```

### [AI Approach Tracks Cell Senescence Using Nuclear Morphology](https://www.genengnews.com/topics/artificial-intelligence/ai-approach-tracks-cell-senescence-using-nuclear-morphology/)
**Type**: news_article
**Publication Date**: 2025-07-07
**Description**: GEN News coverage of the AI-assisted senescent cell tracking technology

## Financials

### grant
**Source**: National Institutes of Health (NIH)
**Funding Type**: Research Project Grant (R01)
**Description**: NIH research grant R01AG053438 supporting the NMP project
**Details**:
```yaml
agency: National Institute on Aging (NIA)
period: Ongoing
grant_type: Research Project Grant (R01)
grant_number: R01AG053438
funding_structure:
  primary_sources:
  -
  agency: National Institute on Aging (NIA)
  source: National Institutes of Health (NIH)
  grant_number: R01AG053438
  institutional_support:
  -
  institution: Department of Orthopedic Surgery, NYU Langone Health
  -
  institution: NYU Langone Health
  -
  institution: NYU Tandon School of Engineering
```

## Events

### Published in Nature Communications
**Date**: 2025-07-07
**Type**: publication
**Description**: NMP research published in Nature Communications journal
**Details**:
```yaml
doi: 10.1038/s41467-025-60975-z
title: Nuclear morphometrics coupled with machine learning identifies dynamic states of senescence across age
journal: Nature Communications
```

## Partnerships

### research
**Focus**: Machine learning applications in biology and senescent cell detection
**Description**: Collaboration between NYU Langone Health and NYU Tandon School of Engineering on NMP development
**Details**:
```yaml
type: Research Collaboration
period: 2020-present
status: Ongoing
partners:
  - NYU Langone Health
  - NYU Tandon School of Engineering
```
