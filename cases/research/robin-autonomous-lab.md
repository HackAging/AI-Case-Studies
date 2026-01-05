---
id: robin-autonomous-lab
slug: robin-autonomous-lab
entity_type: research
status: published
data_completeness: very_high
last_researched: 2026-01-06
research_category: collaboration
researcher: AI Assistant
version: 3.2
name: Robin - Autonomous Lab System
description: First fully autonomous scientific discovery system that can generate hypotheses, plan experiments, analyze results, and update hypotheses in a closed-loop manner. The system integrates literature search agents with data analysis agents to automate the entire scientific discovery process. Published in May 2025, Robin was later evolved into Kosmos (November 2025, arXiv:2511.02824) by the same research team from Edison Scientific and FutureHouse. Kosmos introduced structured world models, achieving 9.8x increase in code generation (42,000 vs 4,310 lines) and 8x more iterations (200 vs ~25 rollouts), enabling longer research cycles and multi-domain discoveries.
mission: To develop and demonstrate fully autonomous scientific discovery systems that can accelerate research by autonomously generating hypotheses, planning experiments, and discovering novel therapeutic strategies for age-related diseases.
entity_data:
  results:
  ai_achievement: First fully autonomous scientific discovery where entire main text hypotheses, experiments, and figures were produced by AI
  primary_discovery: Ripasudil (ROCK inhibitor) identified as novel therapeutic candidate for dry AMD
  validation_status: Mechanism validated experimentally via RNA-seq
  mechanism_discovered: ROCK inhibition upregulates ABCA1, enhancing phagocytosis in retinal cells
  objectives:
  - Develop fully autonomous scientific discovery system
  - Demonstrate AI can autonomously generate hypotheses, plan experiments, and analyze results
  - Apply system to discover novel therapeutic strategies for age-related diseases
  - Validate lab-in-the-loop framework for autonomous scientific discovery
  start_date: 2024
  methodology:
  type: Multi-agent LLM System
  framework: Lab-in-the-loop
  integration_level: Semi-autonomous - AI directs experiments, humans execute
  publication_date: 2025-05-19
  collaboration_period:
  start: 2024
  status: active
taxonomy:
  geography: USA
  ai_approach:
  - Generative AI
  ai_technology:
  - Generative AI
  - LLMs
  primary_focus:
  - Robotic Lab Automation
  - Autonomous AI Scientists
  aging_approach: []
  target_biology:
  - General Aging/Longevity
  ai_architecture:
  - LLMs
  ai_specialization: []
  development_stage: Research / Preclinical
  therapeutic_modality: []
organizations:
  -
    name: Simons Foundation
    role: collaborator
    org_type: institution
    legal_name: Simons Foundation
    status: active
    role_description: Potential funding source
    contribution_description: Research foundation that may have provided funding or support for autonomous research systems. Specific funding details not publicly disclosed.
  -
    name: FutureHouse Inc.
    role: primary
    org_type: company
    legal_name: FutureHouse Inc.
    website: "https://futurehouse.org"
    status: operational
    role_description: Primary organization
    contribution_description: Research and development company focused on developing AI systems for autonomous scientific discovery. Primary organization leading the Robin project. Multiple authors affiliated with FutureHouse.
  -
    name: Cornell University
    role: collaborator
    org_type: institution
    legal_name: Cornell University
    status: active
    role_description: Collaborating institution
    contribution_description: Rodriques Lab at Cornell University participated in the research. Provided research expertise and laboratory facilities.
  -
    name: University of Rochester
    role: collaborator
    org_type: institution
    legal_name: University of Rochester
    status: active
    role_description: Collaborating institution
    contribution_description: "Andrew D. White's lab contributed expertise in machine learning for scientific discovery. Provided machine learning and AI expertise."
products:
  - name: Robin Autonomous Lab System
    type: platform
    status: published
    development_stage: Research / Preclinical
    description: Multi-agent LLM system for autonomous scientific discovery using lab-in-the-loop framework. First system to autonomously discover validated therapeutic candidate.
    capabilities:
      - Autonomous hypothesis generation from literature
      - Experimental protocol design
      - Result analysis and interpretation
      - Iterative hypothesis refinement
      - Wet-lab experiment integration
    technical_details:
      code_generation: ~4,310 lines per run
      literature_analysis: ~1,530 papers per run
      framework: Lab-in-the-loop (AI directs, humans execute)
      validation: Experimentally validated therapeutic discovery
  - name: Ripasudil
    type: drug
    status: preclinical
    development_stage: Research / Preclinical
links:
  -
    url: "https://github.com/Future-House/robin"
    type: documentation
    title: "GitHub - Future-House/robin: Robin: A multi-agent system for automating scientific discovery"
  -
    url: "https://www.emergentmind.com/papers/2505.13400"
    type: article
    title: Emergent Mind - Robin Paper Analysis
  -
    url: "https://en.wikipedia.org/wiki/Robot_Scientist"
    type: reference
    title: "Adam and Eve: Robot Scientists"
  -
    url: "https://arxiv.org/abs/2505.13400"
    type: research_publication
    title: "Robin: A multi-agent system for automating scientific discovery"
---

# Robin - Autonomous Lab System

## Description

Robin is the first fully autonomous scientific discovery system that can generate hypotheses, plan experiments, analyze results, and update hypotheses in a closed-loop manner. The system integrates literature search agents with data analysis agents to automate the entire scientific discovery process, demonstrating the viability of AI-driven therapeutic discovery.

Using a multi-agent LLM architecture, Robin performs automated cycles of literature search and data analysis to propose evidence-based hypotheses. The system operates in a "lab-in-the-loop" framework where AI agents design experiments and analyze results, while human researchers execute the wet-lab experimental work. This semi-autonomous approach enables Robin to explore hypothesis spaces too large for manual investigation while maintaining practical feasibility through human-executed experiments.

Robin successfully identified Ripasudil, a ROCK inhibitor, as a novel therapeutic candidate for dry age-related macular degeneration (AMD)—marking the first time this drug was proposed for this indication. The discovery demonstrates AI's ability to make cross-domain connections beyond typical human cognitive capacity, linking glaucoma treatment knowledge with retinal phagocytosis mechanisms. The therapeutic mechanism was validated experimentally via RNA-seq, showing that ROCK inhibition upregulates ABCA1, enhancing phagocytic capacity in retinal cells.

The system generates an average of 4,310 lines of code and reads approximately 1,530 scientific papers per research run, achieving 3-10x speed improvement over traditional research cycles. Robin compresses the typical hypothesis-to-validation timeline from 7-30 months to 2-7 months, demonstrating substantial acceleration of scientific discovery.

### Relationship to Kosmos

**Robin (May 2025)** served as the foundation for **Kosmos (November 2025)**. The same research team from Edison Scientific (Andrew D. White, Samuel G. Rodriques) created Kosmos as an evolution of Robin, addressing its identified limitations. In the Kosmos paper (arXiv:2511.02824), the authors explicitly state: *"Robin [1], a system we previously reported, performs automated cycles of literature search and data analysis to propose evidence-based hypotheses, but has limited context sharing between its agents and is primarily tailored for therapeutics development."*

**Robin → Kosmos Evolution:**
- **Code Generation**: 4,310 → 42,000 lines (**9.8x increase**)
- **Agent Rollouts**: ~25 → 200 (**8x increase**)  
- **Research Duration**: Short cycles → 12 hours continuous
- **Context Sharing**: Limited → Structured World Model
- **Domains**: Therapeutics focus → 6 scientific domains
- **Discoveries**: 1 therapeutic → 7 discoveries (metabolomics, materials, neuroscience, genetics)
- **Accuracy**: Not reported → 79.4% validated by independent scientists

**Key Innovation in Kosmos:** Introduction of **structured world model** that coordinates all agents and enables the system to maintain coherence 8x longer without losing focus on research objectives.

**Shared Authors:** Andrew D. White, Samuel G. Rodriques, Ludovico Mitchener, Angela Yiu, Benjamin Chang, Michaela M. Hinks, Jon M. Laurent

**In Simple Terms:** Robin = first-generation autonomous AI scientist (proof-of-concept), Kosmos = next-generation system (8-10x more powerful, works across multiple scientific domains beyond just therapeutics).

## Mission

To develop and demonstrate fully autonomous scientific discovery systems that can accelerate research by autonomously generating hypotheses, planning experiments, and discovering novel therapeutic strategies for age-related diseases.

## Project Information

**Start Date**: 2024  
**Publication Date**: 2025-05-19  
**Status**: Published on arXiv

**Objectives:**
- Develop fully autonomous scientific discovery system
- Demonstrate AI can autonomously generate hypotheses, plan experiments, and analyze results
- Apply system to discover novel therapeutic strategies for age-related diseases
- Validate lab-in-the-loop framework for autonomous scientific discovery

**Methodology:**
- Type: Multi-agent LLM System
- Framework: Lab-in-the-loop
- Integration Level: Semi-autonomous (AI directs experiments, humans execute)

**Key Results:**
- AI Achievement: First fully autonomous scientific discovery where entire main text hypotheses, experiments, and figures were produced by AI
- Primary Discovery: Ripasudil (ROCK inhibitor) identified as novel therapeutic candidate for dry AMD
- Validation: Mechanism validated experimentally via RNA-seq
- Mechanism: ROCK inhibition upregulates ABCA1, enhancing phagocytosis in retinal cells

**Collaboration Period:**
- Start: 2024
- Status: Active

## AI Methods

- **Multi-agent LLM System**: Coordinates multiple AI agents for different research tasks
- **Literature Search Agent**: Searches and synthesizes scientific literature (~1,530 papers per run)
- **Data Analysis Agent**: Executes statistical analyses and generates visualizations (~4,310 lines of code per run)
- **Hypothesis Generation**: Automated generation of evidence-based hypotheses from literature
- **Experimental Planning**: AI-driven design of wet-lab experimental protocols
- **Result Interpretation**: Automated analysis of experimental results
- **Iterative Refinement**: Closed-loop hypothesis-experiment-analysis cycles

## Data Types

- **Scientific Literature**: Research papers, reviews, clinical studies
- **Experimental Data**: RNA-seq data from validation experiments
- **Biological Data**: Gene expression, protein interactions, pathway data
- **Clinical Data**: Disease phenotypes, therapeutic outcomes
- **Experimental Protocols**: Detailed methods for wet-lab execution

## Platforms and Technologies

- **Programming**: Python 3.12+
- **LLM Integration**: LiteLLM for multi-model support
- **API**: FutureHouse API for agent coordination
- **Analysis Tools**: Statistical analysis packages, bioinformatics tools
- **Data Processing**: RNA-seq analysis pipelines
- **Version Control**: GitHub (https://github.com/Future-House/robin)

## System Architecture

```yaml
type: Multi-agent LLM System
framework: Lab-in-the-loop
integration_level: Semi-autonomous (AI directs experiments, humans execute wet-lab work)
components:
  - Literature Search Agent:
      description: Searches and synthesizes scientific literature
      capabilities:
        - Search scientific databases
        - Read and analyze papers
        - Extract relevant information
        - Synthesize literature findings
      average_performance: ~1,530 papers per run
  - Data Analysis Agent:
      description: Performs statistical analysis and data processing
      capabilities:
        - Execute code for data analysis
        - Generate statistical models
        - Test hypotheses
        - Process datasets
      average_performance: ~4,310 lines of code per run
  - Hypothesis Generation System:
      description: Generates scientific hypotheses from literature and data
      capabilities:
        - Cross-domain hypothesis generation
        - Evidence-based hypothesis formulation
        - Iterative hypothesis refinement
  - Experimental Planning System:
      description: Plans wet-lab experiments to test hypotheses
      capabilities:
        - Design experimental protocols
        - Specify materials and methods
        - Plan validation experiments
  - Result Interpretation System:
      description: Analyzes experimental results and updates hypotheses
      capabilities:
        - Interpret experimental outcomes
        - Update hypotheses based on results
        - Plan next experimental steps
key_innovation: Integration of literature search with data analysis for automated hypothesis-experiment cycles
context_sharing: Limited context sharing between agents (addressed in later Kosmos system)
primary_focus: Therapeutics development for age-related diseases
```

## Technical Workflow

```yaml
lab_in_the_loop_process:
  description: AI system directs wet-lab experiments iteratively, creating a closed-loop discovery process
  integration_level: Semi-autonomous - AI directs experiments, humans execute
  human_role: Execute wet-lab experiments designed by AI
  ai_role: Generate hypotheses, plan experiments, analyze results
detailed_workflow:
  step_1_hypothesis_generation:
    description: AI generates hypothesis from literature
    process:
      - Literature search agent reviews scientific literature
      - Identifies knowledge gaps and opportunities
      - Generates testable hypotheses
    output: Evidence-based hypothesis
  step_2_experimental_planning:
    description: AI plans experiment to test hypothesis
    process:
      - Design experimental protocol
      - Specify materials, methods, conditions
      - Plan data collection strategy
    output: Detailed experimental protocol
  step_3_human_execution:
    description: Human researchers execute experiment
    process:
      - Follow AI-generated protocol
      - Perform wet-lab experiments
      - Collect experimental data
    output: Experimental data (e.g., RNA-seq data)
  step_4_data_analysis:
    description: AI analyzes experimental results
    process:
      - Data analysis agent processes experimental data
      - Statistical analysis and visualization
      - Interpretation of results
    output: Analysis results and interpretation
  step_5_hypothesis_update:
    description: AI updates hypothesis and plans next experiment
    process:
      - Evaluate if hypothesis supported or refuted
      - Refine hypothesis based on results
      - Generate next experimental questions
    output: Updated hypothesis and next experiment plan
  step_6_iteration:
    description: Repeat until validation
    process: Cycle continues until hypothesis fully validated
    outcome: Validated therapeutic candidate (Ripasudil for dry AMD)
performance:
  code_generation: ~4,310 lines per run
  literature_analysis: ~1,530 papers per run
  iteration_speed: 3-10x faster than manual research
  discovery_timeline: 2-7 months (vs. 7-30 months traditional)
```

## Scientific Background

```yaml
biological_context:
  dry_amd:
  pathology: Characterized by RPE dysfunction, drusen accumulation, and geographic atrophy
  prevalence: Leading cause of blindness in developed countries, affecting millions
  unmet_need: Urgent need for effective dry AMD treatments
  current_treatments: Limited - no approved treatments for dry AMD, only for wet AMD
  abca1_biology:
  function: Critical lipid efflux pump maintaining cholesterol homeostasis
  retinal_importance: Essential for RPE function and photoreceptor health
  therapeutic_target: ABCA1 upregulation could restore RPE function in dry AMD
  disease_association: ABCA1 mutations cause Tangier disease with retinal abnormalities
  rock_inhibitors:
  mechanism: ROCK inhibitors reduce intraocular pressure by affecting trabecular meshwork
  existing_use: Ripasudil approved for glaucoma treatment in Japan
  safety_profile: Established safety profile from glaucoma use could accelerate dry AMD development
  novel_application: Robin identified new application for retinal phagocytosis enhancement
autonomous_lab_systems_history:
  description: Historical context of autonomous laboratory systems
  early_systems:
  -
  name: Adam Robot Scientist
  year: 2009
  limitation: Required significant human programming and was limited to yeast genetics
  description: First autonomous robot scientist that could generate hypotheses and conduct experiments
  -
  name: Eve Robot Scientist
  year: 2015
  limitation: Still required extensive human oversight and programming
  description: Successor to Adam, focused on drug discovery
  paradigm_shift: Transition from rule-based systems to LLM-powered autonomous discovery
  robin_advancement: Robin represents next generation - fully autonomous hypothesis generation using LLMs, not requiring pre-programmed knowledge
```

## Performance Metrics

```yaml
computational_performance:
  code_generation: Average 4,310 lines of code per run
  literature_analysis: Average 1,530 papers read per run
  agent_rollouts: Multiple agent iterations per research cycle
search_space: Can explore hypothesis space too large for manual exploration (ROCK inhibitors × retinal biology × aging pathways)
speed_improvement: 3-10x faster per iteration
literature_integration: Can integrate thousands of literature sources with experimental design beyond human cognitive capacity
hypothesis_to_validation_cycle: 2-7 months (vs. 7-30 months traditional)
discovery_success:
  therapeutic_candidate: Ripasudil identified for dry AMD
  validation: Mechanism validated via RNA-seq
  clinical_relevance: Potential treatment for major age-related disease
```

## Lessons Learned

### Achievements

- Successfully demonstrated fully autonomous scientific discovery from hypothesis to validation
- Proved AI can make cross-domain connections beyond human cognitive capacity
- Established lab-in-the-loop framework as viable approach
- Identified novel therapeutic candidate for major age-related disease
- Validated mechanism through experimental RNA-seq analysis

### Challenges

**AI-Human Integration:**
- Integration of AI agents with wet-lab experimental execution requires careful coordination
- Ensuring experimental protocols are feasible, safe, and executable by human researchers
- Balancing AI autonomy with necessary human oversight for safety and quality control
- Time delays between AI planning and human execution of experiments

**Technical Challenges:**
- Limited context sharing between agents (compared to later systems with structured world models)
- Scaling to more complex experimental systems beyond single therapeutic discovery
- Managing coherence across multiple research cycles
- Computational resource requirements for long-running agent processes

**Domain-Specific Challenges:**
- Primarily tailored for therapeutics development
- Wet-lab validation required for all hypotheses (cannot be fully in silico)
- Access to laboratory facilities and materials needed
- Time and cost of experimental validation

**Quality Control:**
- Ensuring AI-generated hypotheses are scientifically valid
- Verifying experimental protocols are appropriate
- Validating AI interpretations of experimental results
- Maintaining scientific rigor in autonomous discovery process

### Impact on Field

Robin represents a paradigm shift toward fully autonomous scientific discovery in biomedical research. It demonstrates that AI systems can not only assist researchers but can autonomously generate novel hypotheses, design experiments, and discover new therapeutic strategies. This has transformative implications for aging research and drug discovery, potentially compressing decades of research into years through autonomous discovery systems.

**Key Contributions to Field:**
- **First Autonomous Therapeutic Discovery**: Robin is the first AI system to autonomously discover a novel therapeutic candidate (Ripasudil for dry AMD) through closed-loop hypothesis-experiment cycles
- **Lab-in-the-Loop Framework**: Established viable framework for AI-human collaboration in experimental science
- **Cross-Domain Discovery**: Demonstrated AI's ability to make unexpected connections across different medical domains (glaucoma treatment → retinal phagocytosis)
- **Validated Mechanism**: AI-discovered mechanism validated experimentally, proving reliability of autonomous discovery
- **Acceleration of Research**: 3-10x speed improvement demonstrates practical value for research acceleration

**Broader Implications:**
- Opens pathway for AI-driven drug repurposing at scale
- Demonstrates feasibility of autonomous systems in wet-lab science
- Provides template for future autonomous research systems
- Shows potential for AI to discover connections beyond human cognitive capacity
- Establishes proof-of-concept for autonomous therapeutic discovery in aging research

**Limitations Identified:**
- Limited context sharing between agents (addressed in subsequent systems)
- Primary focus on therapeutics (later systems expanded to multiple domains)
- Requires human execution of experiments (semi-autonomous rather than fully autonomous)

Robin's success demonstrated the viability of autonomous AI scientists and laid groundwork for next-generation systems with improved context management and broader scientific applicability.

## Evolution to Kosmos (November 2025)

**Robin** (May 2025) was evolved into **Kosmos** (November 2025, arXiv:2511.02824) by the same research team from Edison Scientific and FutureHouse:

```yaml
timeline:
  robin_publication: May 2025 (arXiv:2505.13400)
  kosmos_publication: November 2025 (arXiv:2511.02824)
  time_between: 6 months
same_research_team:
  organization: Edison Scientific Inc. and FutureHouse Inc.
  shared_leaders:
    - Andrew D. White (co-supervisor in both systems)
    - Samuel G. Rodriques (PI Robin → co-supervisor Kosmos)
  shared_core_developers:
    - Ludovico Mitchener (co-author Robin → co-first author + co-supervisor Kosmos)
    - Angela Yiu (co-author Robin → co-first author Kosmos)
    - Benjamin Chang (co-author Robin → co-first author Kosmos)
    - Michaela M. Hinks (co-author Robin → co-supervisor Kosmos)
    - Jon M. Laurent (co-author in both)
robin_limitations:
  context_sharing: Limited context sharing between agents
  domain_focus: Primarily tailored for therapeutics development
  iteration_limit: Could not maintain coherence beyond ~25 rollouts
  research_duration: Shorter research cycles
kosmos_improvements:
  structured_world_model: Enables information sharing between all agents
  code_generation: 9.8x increase (42,000 vs 4,310 lines per run)
  iterations: 8x more rollouts (200 vs ~25)
  duration: Up to 12 hours continuous operation (vs shorter cycles)
  domains: Multi-domain capability (6 domains demonstrated vs therapeutics focus)
  coherence: Maintains goal pursuit over 200 rollouts without losing coherence
  traceability: All statements cited to code or primary literature
  discoveries: 7 validated discoveries across metabolomics, materials science, connectomics, genetics, proteomics, transcriptomics
  accuracy: 79.4% validated by independent scientists
kosmos_key_innovation:
  structured_world_model:
    description: Shared information structure that consolidates findings from all agents
    benefit: Enables every cycle to build on all previous findings
    result: Can explore many research avenues simultaneously while maintaining coherence
    comparison: Robin had limited context sharing, Kosmos has systematic context management
relationship:
  robin: Proof-of-concept for autonomous scientific discovery with lab-in-the-loop
  kosmos: Next-generation system scaling Robin's approach to longer cycles and multiple domains
  evolution: Kosmos built on Robin's success, addressing identified limitations
quote_from_kosmos_paper: "Robin [1], a system we previously reported, performs automated cycles of literature search and data analysis to propose evidence-based hypotheses, but has limited context sharing between its agents and is primarily tailored for therapeutics development."
```

**Conclusion:** Robin proved the viability of autonomous AI scientists. Kosmos scaled this approach 8-10x by adding structured world model for managing multiple agents across extended research cycles.

## Organizations

### Simons Foundation
**Role in Project**: collaborator
**Role Description**: Potential funding source
**Contribution**: Research foundation that may have provided funding or support for autonomous research systems. Specific funding details not publicly disclosed.
**Organization Type**: institution
**Status**: active
**Description**: Research foundation that may have provided funding or support

### FutureHouse Inc.
**Role in Project**: primary
**Role Description**: Primary organization
**Contribution**: Research and development company focused on developing AI systems for autonomous scientific discovery. Primary organization leading the Robin project. Majority of authors affiliated with FutureHouse including first author Ali Essam Ghareeb and PI Samuel G. Rodriques.
**Organization Type**: company
**Status**: operational
**Website**: https://futurehouse.org
**Description**: Research and development company focused on developing AI systems for autonomous scientific discovery. Located in San Francisco, CA.
**Focus**: AI systems for autonomous scientific discovery, autonomous laboratory systems

### Cornell University
**Role in Project**: collaborator
**Role Description**: Collaborating institution
**Contribution**: Rodriques Lab at Cornell University participated in the research. Provided research expertise and laboratory facilities.
**Organization Type**: institution
**Status**: active
**Description**: Rodriques Lab at Cornell University participated in the research

### University of Rochester
**Role in Project**: collaborator
**Role Description**: Collaborating institution
**Contribution**: Andrew D. White's lab contributed expertise in machine learning for scientific discovery. Provided machine learning and AI expertise.
**Organization Type**: institution
**Status**: active
**Description**: Andrew D. White's lab contributed expertise in machine learning for scientific discovery

## Locations

### FutureHouse Inc. Headquarters
**Type**: headquarters
**City**: San Francisco
**State/Region**: California
**Country**: USA
**Organizations**: FutureHouse Inc.
**Description**: Primary location for Robin project development and autonomous research systems

### University of Rochester Main Campus
**Type**: institution
**City**: Rochester
**State/Region**: New York
**Country**: USA
**Organizations**: University of Rochester
**Description**: Collaborating institution providing machine learning expertise

### Cornell University Main Campus
**Type**: institution
**City**: Ithaca
**State/Region**: New York
**Country**: USA
**Organizations**: Cornell University
**Description**: Collaborating institution providing research expertise and laboratory facilities

## Products

### Ripasudil (ROCK Inhibitor for Dry AMD)
**Type**: drug
**Status**: preclinical
**Development Stage**: Research / Preclinical
**Role in Project**: discovery
**Relationship Description**: Ripasudil (ROCK inhibitor) discovered by Robin AI system as potential therapeutic candidate for dry AMD through autonomous hypothesis generation and experimental validation. First time Ripasudil was proposed for dry AMD treatment. Discovery demonstrates AI's ability to make cross-domain connections beyond human cognitive capacity.
**Description**: ROCK (Rho-kinase) inhibitor autonomously identified by Robin AI system as novel therapeutic candidate for dry age-related macular degeneration (dAMD). Robin made unexpected cross-domain connection between glaucoma treatment (where Ripasudil is approved in Japan) and retinal phagocytosis mechanisms in AMD. Discovery validated experimentally via RNA-seq showing mechanism: ROCK inhibition → ABCA1 upregulation → Enhanced phagocytosis in retinal pigment epithelium cells.
**Mechanism of Action**: ROCK inhibition → ABCA1 upregulation → Enhanced phagocytosis in retinal cells
**Target**: Rho-kinase (ROCK), key regulator of cytoskeletal dynamics
**Pathway**: ROCK inhibitor → ABCA1 lipid efflux pump upregulation → Increased phagocytic capacity → Improved RPE function
**Indications**:
```yaml
primary_indication:
  disease: Dry Age-related Macular Degeneration (dAMD)
  status: preclinical
  prevalence: Leading cause of blindness in developed countries, affecting millions
  pathology: Characterized by RPE dysfunction, drusen accumulation, geographic atrophy
  current_treatments: Limited - no approved treatments for dry AMD (only for wet AMD)
  unmet_need: Urgent need for effective dry AMD treatments
  robin_discovery: First proposal of Ripasudil for dry AMD indication
```
**Clinical Relevance**:
```yaml
existing_approval: Ripasudil approved for glaucoma treatment in Japan
safety_profile: Established safety profile from glaucoma use
development_advantage: Known safety could accelerate development for dry AMD
novel_mechanism: New application for retinal phagocytosis enhancement (not just IOP reduction)
cross_domain_insight: Links glaucoma pharmacology with retinal disease biology
```
**Technical Details**:
```yaml
significance: First time Ripasudil was proposed for dry AMD treatment. Discovery demonstrates AI's ability to make cross-domain connections beyond human cognitive capacity.
discovery_method: AI-autonomous discovery via Robin system
validation_status: Mechanism validated experimentally via RNA-seq
validation_results: Confirmed ROCK inhibition upregulates ABCA1
detailed_mechanism:
  step_1: Ripasudil inhibits Rho-kinase (ROCK), key regulator of cytoskeletal dynamics
  step_2: ROCK inhibition leads to upregulation of ABCA1 (ATP-binding cassette sub-family A member 1)
  step_3: Enhanced ABCA1 function improves phagocytic capacity of RPE cells
  step_4: Improved phagocytosis reduces drusen accumulation and RPE dysfunction
biological_rationale:
  abca1_importance: ABCA1 mutations cause Tangier disease with retinal abnormalities, highlighting its critical role in retinal health
  dry_amd_pathology: Dry AMD characterized by RPE dysfunction, drusen accumulation, impaired phagocytosis
  therapeutic_strategy: Enhancing RPE phagocytic capacity could slow or reverse disease progression
  literature_support: Robin integrated literature on ROCK inhibitors, ABCA1 biology, and AMD pathology
discovery_process:
  literature_search: Thousands of papers analyzed on ROCK inhibitors, retinal biology, AMD
  hypothesis_generation: AI proposed ROCK inhibition could enhance retinal phagocytosis
  experimental_design: RNA-seq experiment designed to validate mechanism
  result_validation: Confirmed ABCA1 upregulation via experimental data
```

## Key People

### Ali Essam Ghareeb
**Participation Type**: researcher
**Role in Project**: First Author
**Affiliations**: Future House
**Contribution**: First author of Robin paper. Led the research on autonomous lab system development and application to dry AMD therapeutic discovery.
**Expertise**: Autonomous laboratory systems, therapeutic discovery, multi-agent AI systems
**Biography**: Researcher at Future House, first author focusing on autonomous scientific discovery systems

### Samuel G. Rodriques
**Participation Type**: pi
**Role in Project**: Principal Investigator / Corresponding Author
**Affiliations**: Future House, Cornell University
**Contribution**: Principal Investigator and Corresponding Author. Overall project leadership, scientific direction, development of autonomous laboratory systems framework, multi-institutional collaboration coordination.
**Expertise**: Autonomous laboratory systems, scientific discovery automation, neurotechnology
**Biography**: Research scientist at Future House and Cornell University, expert in autonomous laboratory systems and scientific discovery automation

### Andrew D. White
**Title**: Professor
**Participation Type**: researcher
**Role in Project**: Co-author, Senior Researcher
**Affiliations**: University of Rochester
**Contribution**: Professor of Chemical Engineering. Contributed machine learning and AI expertise for autonomous scientific discovery. Senior advisor on AI methods and system architecture.
**Expertise**: Machine learning for scientific discovery, Chemical Engineering, AI for drug discovery
**Biography**: Professor of Chemical Engineering at University of Rochester, expert in applying machine learning to scientific discovery

### Ludovico Mitchener
**Participation Type**: researcher
**Role in Project**: Co-author, Core Developer
**Affiliations**: Future House
**Contribution**: Core developer of Robin system. Contributed to system architecture, multi-agent coordination, and autonomous hypothesis generation.
**Expertise**: AI systems, autonomous scientific discovery, Multi-agent systems
**Biography**: Researcher at Future House specializing in autonomous AI scientists

### Angela Yiu
**Participation Type**: researcher
**Role in Project**: Co-author, Core Developer
**Affiliations**: Future House
**Contribution**: Core developer of Robin system. Contributed to system development and research coordination.
**Expertise**: AI systems, autonomous scientific discovery
**Biography**: Researcher at Future House working on autonomous AI scientists

### Benjamin Chang
**Participation Type**: researcher
**Role in Project**: Co-author, Core Developer
**Affiliations**: Future House
**Contribution**: Core developer of Robin system. Contributed to system architecture and performance evaluation.
**Expertise**: AI systems, system evaluation, autonomous research
**Biography**: Researcher at Future House developing autonomous research systems

### Michaela M. Hinks
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Future House
**Contribution**: Contributed to Robin system development and scientific evaluation of discovery outputs.
**Expertise**: Scientific evaluation, AI systems for research
**Biography**: Researcher at Future House focusing on AI-driven scientific discovery

### Jon M. Laurent
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Future House
**Contribution**: Contributed to software development and system architecture of Robin.
**Expertise**: Software engineering, computational biology
**Biography**: Researcher at Future House, software engineer for autonomous research systems

### Caralyn J. Szostkiewicz
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Future House
**Contribution**: Contributed to Robin system development and research execution.
**Expertise**: Autonomous research systems
**Biography**: Researcher at Future House

### Muhammed T. Razzak
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: Future House
**Contribution**: Contributed to Robin system development and research execution.
**Expertise**: Autonomous research systems, AI agents
**Biography**: Researcher at Future House

### Andrew D. White
**Title**: Professor
**Participation Type**: researcher
**Role in Project**: Co-author
**Affiliations**: University of Rochester
**Contribution**: Professor of Chemical Engineering, expert in machine learning for scientific discovery. Contributed machine learning and AI expertise.
**Expertise**: Machine learning for scientific discovery, Chemical Engineering
**Biography**: Professor of Chemical Engineering, expert in machine learning for scientific discovery

### Samuel G. Rodriques
**Participation Type**: pi
**Role in Project**: Principal Investigator / Corresponding Author
**Affiliations**: Future House, Cornell University
**Contribution**: Principal Investigator, Corresponding Author, Project Leader. Overall project leadership, scientific direction, publication lead, multi-institutional collaboration coordination, grant management.
**Expertise**: Autonomous laboratory systems, scientific discovery automation
**Biography**: Research scientist working on autonomous laboratory systems and scientific discovery automation

### Ali Essam Ghareeb
**Participation Type**: researcher
**Role in Project**: First Author
**Affiliations**: Future House

## Links

### [GitHub - Future-House/robin: Robin: A multi-agent system for automating scientific discovery](https://github.com/Future-House/robin)
**Type**: documentation
**Relevance**: primary
**Category**: source
**Relationship Description**: Open-source repository containing the Robin system code and documentation
**Description**: Open-source repository containing the Robin system code and documentation
**Metadata**:
```yaml
type: Code Repository
license: Apache-2.0
```

### [Emergent Mind - Robin Paper Analysis](https://www.emergentmind.com/papers/2505.13400)
**Type**: article
**Relevance**: secondary
**Category**: related
**Relationship Description**: Analysis and discussion of the Robin paper on Emergent Mind
**Description**: Analysis and discussion of the Robin paper on Emergent Mind

### [Adam and Eve: Robot Scientists](https://en.wikipedia.org/wiki/Robot_Scientist)
**Type**: reference
**Relevance**: tertiary
**Category**: reference
**Relationship Description**: Information about early autonomous laboratory systems
**Description**: Information about early autonomous laboratory systems

### [Robin: A multi-agent system for automating scientific discovery](https://arxiv.org/abs/2505.13400)
**Type**: research_publication
**Relevance**: primary
**Category**: source
**Relationship Description**: Main arXiv preprint describing the Robin system, methodology, and discovery of Ripasudil for dry AMD
**Publisher**: arXiv
**Publication Date**: 2025-05-19
**Authors**: Ali Essam Ghareeb, Benjamin Chang, Ludovico Mitchener, Angela Yiu, Caralyn J. Szostkiewicz, Jon M. Laurent, Muhammed T. Razzak, Andrew D. White, Michaela M. Hinks, Samuel G. Rodriques
**Description**: Main arXiv preprint describing the Robin system, methodology, and discovery of Ripasudil for dry AMD
**Metadata**:
```yaml
doi: 10.48550/arXiv.2505.13400
type: Preprint
venue: arXiv
arxiv_id: 2505.13400
```

### [Kosmos: An AI Scientist for Autonomous Discovery](https://arxiv.org/abs/2511.02824)
**Type**: research_publication
**Relevance**: secondary
**Category**: related
**Relationship Description**: Related autonomous AI scientist system from overlapping research group. References Robin as prior work and reports 9.8x increase in code generation through structured world models.
**Publisher**: arXiv
**Publication Date**: 2025-11-04
**Authors**: Ludovico Mitchener, Angela Yiu, Benjamin Chang, Andrew D. White, Samuel G. Rodriques, Michaela M. Hinks, and 30 co-authors
**Description**: Next-generation autonomous AI scientist system that addresses context sharing limitations through structured world models, enabling longer-duration research cycles and multi-domain scientific discovery
**Metadata**:
```yaml
doi: 10.48550/arXiv.2511.02824
type: arXiv Preprint
arxiv_id: 2511.02824
relationship: Related autonomous research system with overlapping authors
comparison: 9.8x increase in code generation, 8x more iterations, structured world model innovation
```

## Events

### Project start
**Date**: 2024-01-01
**Type**: foundation
**Description**: Robin project initiated

### Publication of Robin paper on arXiv
**Date**: 2025-05-19
**Type**: publication
**Description**: Main publication describing the Robin system and its application to discovering Ripasudil for dry AMD
**Details**:
```yaml
doi: 10.48550/arXiv.2505.13400
title: "Robin: A multi-agent system for automating scientific discovery"
venue: arXiv
arxiv_id: 2505.13400
```

## Partnerships

### research
**Date**: 2024-01-01
**Focus**: Research collaboration
**Description**: Andrew D. White's lab contributed expertise in machine learning for scientific discovery
**Partner Organizations**:
- University of Rochester (collaborator)
  - Research collaboration partner providing machine learning and AI expertise
**Details**:
```yaml
type: Research Collaboration
partner: University of Rochester
contribution: Machine learning and AI expertise
```

### research
**Date**: 2024-01-01
**Focus**: Research collaboration
**Description**: Rodriques Lab at Cornell University collaborated on the research
**Partner Organizations**:
- Cornell University (collaborator)
  - Research collaboration partner providing research expertise and laboratory facilities
**Details**:
```yaml
type: Research Collaboration
partner: Cornell University
contribution: Research expertise and laboratory facilities
```
