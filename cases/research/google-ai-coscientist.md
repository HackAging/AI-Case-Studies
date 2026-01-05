---
id: google-ai-coscientist
slug: google-ai-coscientist
entity_type: research
status: published
data_completeness: high
last_researched: 2025-02-18
research_category: collaboration
researcher: AI Assistant
version: 1.0
name: Google AI Co-Scientist
description: "A multi-agent AI system built on Gemini 2.0 designed to augment scientific discovery by generating novel research hypotheses and proposals. The AI co-scientist employs a 'generate, debate, and evolve' approach inspired by the scientific method, with specialized agents working together to create, refine, and improve research hypotheses through tournament-based evolution. The system is designed for scientist-in-the-loop collaboration, allowing domain experts to specify research goals in natural language and guide the exploration process. It has been validated in three biomedical areas: drug repurposing for acute myeloid leukemia (AML), novel epigenetic target discovery for liver fibrosis, and mechanistic explanations for bacterial evolution and antimicrobial resistance. The system demonstrates the potential to accelerate scientific discovery by combining broad knowledge synthesis with deep domain expertise."
mission: To augment scientific discovery by helping researchers generate novel, original research hypotheses and proposals that build upon prior evidence and align with scientist-provided research objectives, accelerating the pace of scientific breakthroughs through AI-human collaboration.
entity_data:
  name: Google AI Co-Scientist
  status: published
  objectives:
    - Develop a multi-agent AI system to help uncover new, original knowledge
    - Formulate demonstrably novel research hypotheses and proposals
    - Build upon prior evidence aligned to scientist-provided research objectives
    - Accelerate scientific discovery through AI-human collaboration
    - Validate system in biomedical research areas (drug repurposing, target discovery, mechanistic understanding)
  start_date: 2024
  publication_date: 2025-02-18
  methodology: "Multi-agent system with generate-debate-evolve approach, tournament evolution process, test-time compute scaling, asynchronous task execution framework"
  results: "Validated in three areas: (1) Drug repurposing - proposed AML candidates showing tumor inhibition in vitro at clinically applicable concentrations; (2) Novel target discovery - identified epigenetic targets for liver fibrosis validated by anti-fibrotic activity and liver cell regeneration in human hepatic organoids; (3) Bacterial evolution - recapitulated unpublished experimental results via parallel in silico discovery of novel gene transfer mechanism"
  collaboration_period:
    start: 2024
    publication_date: 2025-02-18
    status: active
  author_contributions:
    conceptualization:
      - Juraj Gottweis
      - Wei-Hung Weng
      - Alexander Daryin
      - Tao Tu
      - Vivek Natarajan
      - Alan Karthikesalingam
    methodology:
      - Juraj Gottweis
      - Wei-Hung Weng
      - Alexander Daryin
      - Tao Tu
      - Petar Sirkovic
      - Artiom Myaskovsky
      - Felix Weissenberger
    investigation:
      - Anil Palepu
      - Dan Popovici
      - Jacob Blum
      - Fan Zhang
      - Katherine Chou
      - Eeshit Dhaval Vaishnav
      - Byron Lee
      - Tiago R D Costa
      - José R Penadés
      - Gary Peltz
      - Vikram Dhillon
    supervision:
      - Avinatan Hassidim
      - Burak Gokturk
      - Amin Vahdat
      - Pushmeet Kohli
      - Yossi Matias
      - Andrew Carroll
      - Kavita Kulkarni
      - Nenad Tomasev
      - Yunhan Xu
      - Annalisa Pawlosky
      - Alan Karthikesalingam
      - Vivek Natarajan
    writing_original_draft:
      - Juraj Gottweis
      - Wei-Hung Weng
      - Alexander Daryin
      - Tao Tu
    writing_review_editing:
      - All authors
taxonomy:
  geography: USA
  ai_approach:
    - Generative AI
  ai_technology:
    - Generative AI
    - LLMs
    - Multi-Agent AI
  ai_architecture:
    - LLMs
    - Multi-Agent AI
  ai_specialization:
    - Multi-Agent AI
  primary_focus:
    - Autonomous AI Scientists
    - AI-Driven Drug Discovery
  aging_approach:
    - Target Discovery
    - Drug Repurposing
  target_biology:
    - General Aging/Longevity
    - Cancer/Oncology
    - Fibrosis
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality: []
organizations:
  - name: Google Cloud AI Research
    role: primary
    org_type: research_center
    website: "https://cloud.google.com/ai"
    status: active
    role_description: Primary research organization developing the AI co-scientist system
    contribution_description: Development of multi-agent AI system architecture, specialized agents, and core research framework
  - name: Google Research
    role: primary
    org_type: research_center
    website: "https://research.google/"
    status: active
    role_description: Primary research organization contributing to AI co-scientist development
    contribution_description: Research contributions to hypothesis generation, validation methodologies, and biomedical applications
  - name: Google DeepMind
    role: primary
    org_type: research_center
    website: "https://deepmind.google/"
    status: active
    role_description: Primary research organization providing Gemini 2.0 foundation model
    contribution_description: Development of Gemini 2.0 foundation model and integration with co-scientist system
  - name: Houston Methodist
    role: collaborator
    org_type: institution
    website: "https://www.houstonmethodist.org/"
    status: active
    role_description: Collaborating medical institution
    contribution_description: Biomedical research expertise and validation support
  - name: Sequome
    role: collaborator
    org_type: company
    status: active
    role_description: Collaborating biotechnology company
    contribution_description: Research collaboration and validation support
  - name: Fleming Initiative and Imperial College London
    role: collaborator
    org_type: institution
    website: "https://www.imperial.ac.uk/"
    status: active
    role_description: Collaborating research institution
    contribution_description: Research collaboration, particularly in bacterial evolution and antimicrobial resistance studies
  - name: Stanford University
    role: collaborator
    org_type: institution
    website: "https://www.stanford.edu/"
    status: active
    role_description: Collaborating research institution
    contribution_description: Research collaboration and validation support
products:
  - name: AI Co-Scientist System
    type: platform
    status: published
    development_stage: Research / Preclinical
    description: "Multi-agent AI system for autonomous scientific discovery built on Gemini 2.0. The system includes specialized agents for hypothesis generation, reflection, ranking, evolution, proximity evaluation, and meta-review. It employs a generate-debate-evolve approach with tournament-based evolution for continuous improvement."
    capabilities:
      - Natural language research goal specification
      - Literature search and synthesis
      - Novel hypothesis generation
      - Hypothesis debate and ranking
      - Tournament-based evolution
      - Research proposal generation
      - Tool integration (web search, AlphaFold, specialized AI models)
      - Scientist-in-the-loop collaboration
    technical_details:
      ai_methods: "Multi-agent system, generate-debate-evolve approach, tournament evolution, test-time compute scaling, asynchronous task execution"
      architecture: "Multi-agent architecture with specialized agents: Generation, Reflection, Ranking, Evolution, Proximity, Meta-review"
      training_data: "Built on Gemini 2.0 foundation model with access to scientific literature and databases"
      performance_metrics: "Continued benefits of test-time compute on hypothesis quality, validated in three biomedical areas"
      validation: "External validation through in vitro experiments and organoid studies"
  - name: Generation Agent
    type: ai_model
    status: published
    description: Specialized agent responsible for generating novel research hypotheses
  - name: Reflection Agent
    type: ai_model
    status: published
    description: Specialized agent for self-critique and reflection on generated hypotheses
  - name: Ranking Agent
    type: ai_model
    status: published
    description: Specialized agent for comparing and ranking hypotheses through simulated scientific debate
  - name: Evolution Agent
    type: ai_model
    status: published
    description: Specialized agent for evolving and improving hypotheses through tournament process
  - name: Proximity Agent
    type: ai_model
    status: published
    description: Specialized agent for evaluating relatedness and proximity of hypotheses
  - name: Meta-review Agent
    type: ai_model
    status: published
    description: Specialized agent providing high-level analysis and meta-review of hypotheses
people:
  - name: Juraj Gottweis
    title: PhD
    person_type: researcher
    role: Co-first Author, Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Co-first author, conceptualization, methodology, writing
  - name: Wei-Hung Weng
    title: PhD
    person_type: researcher
    role: Co-first Author, Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Co-first author, conceptualization, methodology, writing
  - name: Alexander Daryin
    title: PhD
    person_type: researcher
    role: Co-first Author, Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Co-first author, conceptualization, methodology, writing
  - name: Tao Tu
    title: PhD
    person_type: researcher
    role: Co-first Author, Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Co-first author, conceptualization, methodology, writing
  - name: Vivek Natarajan
    title: PhD
    person_type: pi
    role: Corresponding Author, Principal Investigator
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Corresponding author, supervision, conceptualization
    email: natviv@google.com
  - name: Alan Karthikesalingam
    title: PhD
    person_type: pi
    role: Corresponding Author, Principal Investigator
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Corresponding author, supervision, conceptualization
    email: alankarthi@google.com
  - name: Annalisa Pawlosky
    title: PhD
    person_type: pi
    role: Corresponding Author, Principal Investigator
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Corresponding author, supervision
    email: apawlosky@google.com
  - name: Anil Palepu
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Investigation
  - name: Petar Sirkovic
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Methodology
  - name: Artiom Myaskovsky
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Methodology
  - name: Felix Weissenberger
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Methodology
  - name: Keran Rong
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Research contributions
  - name: Ryutaro Tanno
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Research contributions
  - name: Khaled Saab
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Research contributions
  - name: Dan Popovici
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Investigation
  - name: Jacob Blum
    person_type: researcher
    role: Researcher
    affiliations:
      - Stanford University
    organization_id: stanford-university
    contribution_description: Investigation
  - name: Fan Zhang
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Investigation
  - name: Katherine Chou
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Investigation
  - name: Avinatan Hassidim
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Supervision
  - name: Burak Gokturk
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Supervision
  - name: Amin Vahdat
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Cloud AI Research
    organization_id: google-cloud-ai-research
    contribution_description: Supervision
  - name: Pushmeet Kohli
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Supervision
  - name: Yossi Matias
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Supervision
  - name: Andrew Carroll
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Supervision
  - name: Kavita Kulkarni
    person_type: researcher
    role: Researcher
    affiliations:
      - Google Research
    organization_id: google-research
    contribution_description: Supervision
  - name: Nenad Tomasev
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Supervision
  - name: Vikram Dhillon
    person_type: researcher
    role: Researcher
    affiliations:
      - Houston Methodist
    organization_id: houston-methodist
    contribution_description: Investigation
  - name: Eeshit Dhaval Vaishnav
    person_type: researcher
    role: Researcher
    affiliations:
      - Sequome
    organization_id: sequome
    contribution_description: Investigation
  - name: Byron Lee
    person_type: researcher
    role: Researcher
    affiliations:
      - Sequome
    organization_id: sequome
    contribution_description: Investigation
  - name: Tiago R D Costa
    person_type: researcher
    role: Researcher
    affiliations:
      - Fleming Initiative and Imperial College London
    organization_id: fleming-imperial
    contribution_description: Investigation
  - name: José R Penadés
    person_type: researcher
    role: Researcher
    affiliations:
      - Fleming Initiative and Imperial College London
    organization_id: fleming-imperial
    contribution_description: Investigation
  - name: Gary Peltz
    person_type: researcher
    role: Researcher
    affiliations:
      - Stanford University
    organization_id: stanford-university
    contribution_description: Investigation
  - name: Yunhan Xu
    person_type: researcher
    role: Researcher
    affiliations:
      - Google DeepMind
    organization_id: google-deepmind
    contribution_description: Supervision
links:
  - url: "https://storage.googleapis.com/coscientist_paper/ai_coscientist.pdf"
    type: research_publication
    title: "Towards an AI co-scientist"
    description: "Primary research paper describing the AI co-scientist multi-agent system built on Gemini 2.0"
    authors:
      - Juraj Gottweis
      - Wei-Hung Weng
      - Alexander Daryin
      - Tao Tu
      - Anil Palepu
      - Petar Sirkovic
      - Artiom Myaskovsky
      - Felix Weissenberger
      - Keran Rong
      - Ryutaro Tanno
      - Khaled Saab
      - Dan Popovici
      - Jacob Blum
      - Fan Zhang
      - Katherine Chou
      - Avinatan Hassidim
      - Burak Gokturk
      - Amin Vahdat
      - Pushmeet Kohli
      - Yossi Matias
      - Andrew Carroll
      - Kavita Kulkarni
      - Nenad Tomasev
      - Vikram Dhillon
      - Eeshit Dhaval Vaishnav
      - Byron Lee
      - Tiago R D Costa
      - José R Penadés
      - Gary Peltz
      - Yunhan Xu
      - Annalisa Pawlosky
      - Alan Karthikesalingam
      - Vivek Natarajan
    publisher: Google Research
    publication_date: 2025-02-18
    relevance: primary
    category: publication
  - url: "https://deepmind.google/"
    type: website
    title: "Google DeepMind"
    description: "Google DeepMind website - developer of Gemini 2.0 foundation model"
    relevance: secondary
    category: source
  - url: "https://research.google/"
    type: website
    title: "Google Research"
    description: "Google Research website"
    relevance: secondary
    category: source
  - url: "https://cloud.google.com/ai"
    type: website
    title: "Google Cloud AI"
    description: "Google Cloud AI Research website"
    relevance: secondary
    category: source
---

# Google AI Co-Scientist

## Description

A multi-agent AI system built on Gemini 2.0 designed to augment scientific discovery by generating novel research hypotheses and proposals. The AI co-scientist employs a "generate, debate, and evolve" approach inspired by the scientific method, with specialized agents working together to create, refine, and improve research hypotheses through tournament-based evolution. The system is designed for scientist-in-the-loop collaboration, allowing domain experts to specify research goals in natural language and guide the exploration process. It has been validated in three biomedical areas: drug repurposing for acute myeloid leukemia (AML), novel epigenetic target discovery for liver fibrosis, and mechanistic explanations for bacterial evolution and antimicrobial resistance. The system demonstrates the potential to accelerate scientific discovery by combining broad knowledge synthesis with deep domain expertise.

## Mission

To augment scientific discovery by helping researchers generate novel, original research hypotheses and proposals that build upon prior evidence and align with scientist-provided research objectives, accelerating the pace of scientific breakthroughs through AI-human collaboration.

## Project Information

**Start Date**: 2024  
**Publication Date**: 2025-02-18  
**Status**: Published

## Objectives

- Develop a multi-agent AI system to help uncover new, original knowledge
- Formulate demonstrably novel research hypotheses and proposals
- Build upon prior evidence aligned to scientist-provided research objectives
- Accelerate scientific discovery through AI-human collaboration
- Validate system in biomedical research areas (drug repurposing, target discovery, mechanistic understanding)

## AI Methods

- Multi-agent system architecture
- Generate-debate-evolve approach
- Tournament-based evolution process
- Test-time compute scaling
- Asynchronous task execution framework
- Specialized agent coordination (Generation, Reflection, Ranking, Evolution, Proximity, Meta-review)
- Tool integration (web search, AlphaFold, specialized AI models)
- Scientist-in-the-loop collaboration paradigm

## System Architecture

```yaml
type: Multi-agent AI System
foundation_model: Gemini 2.0
components:
  - Generation Agent: Generates novel research hypotheses
  - Reflection Agent: Self-critique and reflection on hypotheses
  - Ranking Agent: Compares and ranks hypotheses through simulated scientific debate
  - Evolution Agent: Evolves and improves hypotheses through tournament process
  - Proximity Agent: Evaluates relatedness and proximity of hypotheses
  - Meta-review Agent: Provides high-level analysis and meta-review
workflow:
  - 1. Research goal specification (natural language)
  - 2. Literature search and synthesis
  - 3. Hypothesis generation (Generation Agent)
  - 4. Hypothesis reflection and critique (Reflection Agent)
  - 5. Hypothesis comparison and ranking (Ranking Agent via scientific debate)
  - 6. Tournament-based evolution (Evolution Agent)
  - 7. Proximity evaluation (Proximity Agent)
  - 8. Meta-review and synthesis (Meta-review Agent)
  - 9. Iterative improvement through test-time compute scaling
  - 10. Final hypothesis and research proposal generation
key_features:
  asynchronous_execution: Asynchronous task execution framework for flexible compute scaling
  tournament_evolution: Tournament evolution process for self-improving hypothesis generation
  test_time_compute: Significant scaling of test-time compute for iterative reasoning and improvement
  tool_integration: Integration with web search, AlphaFold, and specialized AI models
  scientist_in_loop: Scientist-in-the-loop collaborative paradigm
```

## Technical Workflow

```yaml
workflow:
  step_1:
    name: Research Goal Specification
    description: Scientists specify research goals in natural language, including desirable attributes and constraints
  step_2:
    name: Literature Search and Synthesis
    description: System searches and reasons over relevant literature to summarize and synthesize prior work
  step_3:
    name: Hypothesis Generation
    description: Generation Agent creates novel research hypotheses building on prior evidence
  step_4:
    name: Reflection and Critique
    description: Reflection Agent provides self-critique and identifies potential issues
  step_5:
    name: Scientific Debate
    description: Ranking Agent simulates scientific debate to compare and rank competing hypotheses
  step_6:
    name: Tournament Evolution
    description: Evolution Agent improves hypotheses through tournament-based evolution process
  step_7:
    name: Proximity Evaluation
    description: Proximity Agent evaluates relatedness and proximity of hypotheses
  step_8:
    name: Meta-Review
    description: Meta-review Agent provides high-level analysis and synthesis
  step_9:
    name: Iterative Improvement
    description: System uses test-time compute scaling to iteratively reason, evolve, and improve outputs
  step_10:
    name: Research Proposal Generation
    description: Final hypothesis and experimental protocol generation with citations and reasoning
framework: Generate, debate, and evolve approach inspired by scientific method
compute_scaling: Significant scaling of test-time compute paradigm for iterative improvement
```

## Scientific Background

```yaml
scientific_discovery_challenge:
  breadth_depth_conundrum: Researchers face challenges balancing deep domain expertise with broad trans-disciplinary knowledge
  publication_volume: Rapid rise in scientific publications makes comprehensive knowledge synthesis difficult
  hypothesis_generation: Traditional hypothesis generation relies heavily on human creativity and domain expertise
  trans_disciplinary_insights: Many breakthroughs emerge from combining knowledge across disciplines
  historical_examples:
    crispr: Emmanuelle Charpentier and Jennifer Doudna combined microbiology, genetics, and molecular biology (2020 Nobel Prize Chemistry)
    neural_networks: Geoffrey Hinton and John Hopfield combined physics and neuroscience (2024 Nobel Prize Physics)
ai_augmentation:
  reasoning_capabilities: Modern AI systems capable of advanced reasoning and multimodal understanding
  agentic_behaviors: AI systems can use tools to solve complex tasks over long time horizons
  cost_trends: Inference time compute costs decreasing, making AI systems more accessible
  general_intelligence: Trends toward generally intelligent and collaborative AI systems
  foundation: Built on Gemini 2.0 with advanced reasoning, multimodal understanding, and agentic capabilities
test_time_compute_paradigm:
  concept: Allocate additional computational resources during inference for System-2 style thinking
  inspiration: AlphaGo (Monte Carlo Tree Search), Libratus (poker), modern reasoning models
  benefits: 
    - Enables slower, deliberate reasoning
    - Reduces uncertainty
    - Progresses optimally toward goals
    - Iterative improvement without retraining
  implementation: Generate, debate, and evolve approach with tournament-based evolution
  scaling: Significant scaling enables iterative reasoning, evolution, and output improvement
  no_training: System doesn't require specialized pre-training, post-training, or reinforcement learning
multi_agent_systems:
  benefits:
    - Parallel hypothesis generation
    - Specialized agent expertise
    - Collaborative refinement
    - Scalable workflows
  description: Multi-agent systems enable coordination among specialized agents for collaborative research
  supervisor_role: Manages worker task queue, assigns specialized agents, allocates resources
  asynchronous_execution: Flexible and effective computational resource utilization
  context_memory: Persistent storage for agent and system states enabling long-horizon reasoning
tournament_evolution:
  approach: Tournament-based evolution process compares and ranks hypotheses to identify best candidates
  improvement: Continuous improvement through win/loss patterns and iterative refinement
  scaling: Benefits from test-time compute scaling for enhanced hypothesis quality
  elo_system: Initial rating 1200, pairwise comparisons with multi-turn debates for top candidates
  feedback_loop: Meta-review agent enables self-improvement without backpropagation
scientist_in_loop:
  paradigm: Purpose-built for collaborative human-AI interaction
  capabilities:
    - Specify research goals in natural language
    - Inform desirable attributes and constraints
    - Directly supply own ideas and hypotheses
    - Refine system-generated hypotheses
    - Provide feedback via natural language chat
    - Guide system alignment with expertise
  goal: Augment hypothesis generation, not automate scientific process
drug_repurposing:
  challenge: Identifying new therapeutic applications for existing drugs
  complexity: Medium, data-limited
  approach: Combinatorial search through large but constrained set of drug-disease pairs
  advantages:
    - Drugs have established safety profiles
    - Reduced development time and cost
    - Readily available for testing
  limitations:
    - Requires extensive cross-domain expertise
    - Complex mammalian biological systems
    - Time-intensive computational biology analyses
  ai_contribution: AI can analyze molecular signatures, signaling pathways, drug interactions, clinical trials, literature
  validation: In vitro validation demonstrates clinical applicability
  examples: Humira (adalimumab), Keytruda (pembrolizumab) - among most successful drugs in history
  statistics: ~70% of drug approvals are for new drugs, highlighting repurposing opportunity
target_discovery:
  challenge: Discovering novel therapeutic targets for complex diseases
  complexity: High, experiment-limited
  uncertainty: Significantly greater than drug repurposing
  requirements:
    - Extensive literature review
    - Deep biological understanding
    - Sophisticated hypothesis generation
    - Complex experimental validation strategies
  process: Involves uncovering entirely new components and mechanisms within biological systems
  inefficiency: Traditional process can lead to suboptimal hypothesis selection and prioritization
  validation_cost: High costs and time associated with in vitro and in vivo experimentation
  ai_contribution: AI can propose, rank, and provide experimental protocols for novel hypotheses
  validation: Organoid models validate target efficacy and mechanism
  example: Liver fibrosis - prevalent and serious disease with limited treatment options
bacterial_evolution:
  challenge: Understanding mechanisms of antimicrobial resistance and gene transfer
  complexity: Very high, large data and computation-limited
  system_level: Involves molecular mechanisms and ecological/evolutionary pressures
  mechanisms: Conjugation, transduction, transformation
  healthcare_impact: Increasing rates of infections and deaths worldwide
  ai_contribution: AI can discover novel mechanisms through parallel in silico analysis
  validation: Recapitulation of unpublished experimental results demonstrates discovery capability
  example: cf-PICIs (capsid-forming phage-inducible chromosomal islands) transfer mechanisms
tool_integration:
  web_search: Primary tool for grounded, up-to-date hypotheses from literature
  specialized_databases: Access to domain-specific databases (e.g., FDA-approved drugs, cell receptors)
  specialized_ai_models: Integration with AlphaFold for protein structure prediction and validation
  private_repositories: Can index and search scientist-provided publication collections
  example: AlphaFold validates structural plausibility of protein sequences, reduces hallucinations
safety_considerations:
  dual_use_risks: Potential for misuse of scientific breakthroughs
  ethical_concerns: Research contradicting established norms
  safeguards:
    - Research goal safety review on input
    - Hypothesis safety review even for safe goals
    - Continuous monitoring of research directions
    - Explainability and transparency with reasoning traces
    - Comprehensive logging for auditing
    - Red teaming with 1,200 adversarial examples
    - Trusted tester program for responsible rollout
  foundation: Builds on Gemini 2.0 safety evaluations and safeguards
  human_oversight: Designed for continuous expert oversight, final decisions by scientists
```

## Validation Results

### Drug Repurposing for Acute Myeloid Leukemia (AML)

The AI co-scientist was tasked with identifying drug repurposing candidates for AML, particularly targeting the MOLM13 cell line. The system explored a constrained space of 2,300 approved drugs across 33 cancer types.

**Clinical Expert Evaluation:**
- 78 drug repurposing proposals were evaluated by 6 board-certified hematologists and oncologists
- Proposals were formatted as NIH-style Specific Aims Pages
- Expert evaluation showed high ratings across all 15 evaluation criteria
- Experts consistently rated proposals as "Strongly Agree" or "Agree" on significance, innovation, rigor, and feasibility

**Drug Candidates with Existing Preclinical Evidence:**
Five drugs were selected for in vitro validation based on their potential to modulate key molecular signaling pathways:
- **Binimetinib** (MEK1/2 inhibitor): IC50 of 7 nM in MOLM-13 cells, demonstrated efficacy at clinically applicable concentrations
- **Pacritinib** (dual JAK2/FLT3 inhibitor): Showed inhibition of cell viability
- **Cerivastatin** (statin): Demonstrated tumor inhibition activity
- Pravastatin and Dimethyl fumarate (DMF) showed minimal effect

**Novel Drug Repurposing Candidates (No Prior AML Evidence):**
Three novel candidates with no prior preclinical or clinical data for AML were tested:
- **KIRA6** (IRE1α inhibitor): 
  - KG-1 cells: IC50 of 13 nM
  - MOLM-13 cells: IC50 of 517 nM
  - HL-60 cells: IC50 of 817 nM
- Nanvuranlat and Leflunomide showed no significant effect

**Computational Validation:**
- Integration with DepMap (Cancer Dependency Map) Q2 2024 data
- High concordance between co-scientist scores and DepMap dependency scores
- Candidates required co-scientist review score ≥4 and DepMap score ≥0.99 for expert review

### Novel Target Discovery for Liver Fibrosis

The AI co-scientist was instructed to propose experimentally testable hypotheses about epigenetic alterations in myofibroblast formation in liver fibrosis.

**Validation Process:**
- System generated 15 top-ranked research hypotheses with comprehensive experimental designs
- Experts selected 3 hypotheses for validation
- Testing performed using human hepatic organoids with live cell imaging system

**Results:**
- **Three novel epigenetic modifiers** identified with supporting preclinical evidence
- **Four drugs** based on epigenetic targets showed significant effects:
  - Two drugs targeting epigenetic modifiers exhibited significant anti-fibrotic activity
  - Demonstrated liver cell regeneration in human hepatic organoids
  - Minimal cellular toxicity at effective concentrations
  - One identified drug is FDA-approved for another indication, enabling potential expedited repurposing

**Methodology:**
- Used fibrogenic agent TGF-β as inducer
- Measured myofibroblast activity via fluorescence labeling
- Statistical significance demonstrated between treatment groups (p-values reported)
- Validation detailed in separate co-timed technical report

### Recapitulating Discovery of Bacterial Evolution Mechanism (Antimicrobial Resistance)

The AI co-scientist was challenged to explain why capsid-forming phage-inducible chromosomal islands (cf-PICIs) are readily found across diverse bacterial species - a question that researchers had spent ~10 years investigating.

**Timeline Comparison:**
- Traditional experimental pipeline: 2015-2024 (~10 years of iterative research)
- AI co-scientist: 2 days (building on decades of prior literature)

**Input Provided:**
- Single-page document with general background on phage satellites
- Two research articles: original cf-PICI discovery and computational identification technique
- No access to unpublished experimental findings

**System Output - Top-Ranked Hypothesis:**
The co-scientist independently proposed that **cf-PICIs interact with diverse phage tails to expand their host range** - precisely matching the unpublished experimental finding.

**Additional Research Directions Proposed:**
- Capsid-tail interactions (primary finding alignment)
- Integration mechanisms across bacterial genomes
- Entry mechanisms beyond traditional phage receptor recognition
- Helper phage and environmental factors in cf-PICI transfer
- Alternative transfer mechanisms (conjugation, extracellular vesicles)

**Experimental Validation:**
- Independent research study validated this hypothesis through genomic and experimental studies
- Mechanism involves cf-PICI-encoded adaptor and connector proteins mediating interactions with different phage tails
- Finding currently under peer review at established journal
- Demonstrates co-scientist's capability for parallel discovery of novel mechanisms

**Significance:**
- Demonstrates capability to generate hypotheses matching ~10 years of experimental research
- Novel solutions proposed for combating antimicrobial resistance
- Validates system's ability in complex, systems-level biological problems

## Performance Metrics

```yaml
benchmark_performance:
  gpqa_diamond:
    top_1_accuracy: 78.4%
    metric: Concordance between Elo rating and correctness
    dataset: GPQA diamond set (challenging multiple-choice questions)
    baseline_comparison: Gemini 2.0 reference responses
elo_rating_analysis:
  research_goals_analyzed: 203 distinct goals across broad scientific topics
  temporal_buckets: 10 equal-sized buckets
  metrics_tracked:
    - best_elo: Maximum individual Elo rating per bucket
    - top_10_avg: Average Elo rating of top 10 hypotheses
  trend: Consistent upward improvement from first to last bucket
  conclusion: Significant quality enhancement with test-time compute scaling
expert_curated_subset:
  goals: 15 challenging biomedical problems
  curators: 7 PhD-level experts (postdocs/faculty)
  comparison_models:
    - Gemini 2.0 Pro Experimental
    - Gemini 2.0 Flash Thinking Experimental 12-19
    - OpenAI o1
    - OpenAI o3-mini-high
    - DeepSeek R1
  result: AI co-scientist outperformed all baselines and human expert "best guess"
  saturation: No evidence of performance saturation, suggesting continued benefits
expert_evaluation:
  evaluators: 11 expert evaluations
  preference_rank: 2.36 (1 = most preferred, 4 = least preferred)
  novelty_rating: 3.64 out of 5
  impact_rating: 3.09 out of 5
  result: Co-scientist most preferred over other LLM baselines
llm_judge_evaluation:
  judges:
    - OpenAI o3-mini-2025-01-31
    - OpenAI o1-preview-2024-09-12
    - Gemini 2.0 Pro Experimental
    - Gemini 2.0 Flash Thinking Experimental 01-21
  result: Co-scientist outputs most preferred by all LLM judges
hypothesis_quality:
  metric: Continued benefits of test-time compute on hypothesis quality
  improvement: Automated evaluations show improved hypothesis quality with increased compute
  elo_improvement: Progressive increase from early to late temporal buckets
validation_success:
  drug_repurposing:
    platform: In vitro validation in AML cell lines
    binimetinib_ic50: 7 nM in MOLM-13 cells
    kira6_ic50_range: 13-817 nM across KG-1, MOLM-13, HL-60
    clinical_relevance: Concentrations clinically applicable
  target_discovery:
    platform: Human hepatic organoids
    targets_identified: 3 novel epigenetic modifiers
    drugs_tested: 4 based on AI suggestions
    successful_drugs: 2 with significant anti-fibrotic activity
    toxicity: Minimal cellular toxicity
  mechanism_discovery:
    discovery_time: 2 days (vs ~10 years traditional research)
    accuracy: Independently recapitulated unpublished findings
    validation_status: Under peer review at established journal
compute_efficiency:
  scaling: Asynchronous task execution framework enables flexible compute scaling
  test_time: Test-time compute scaling provides iterative improvement without retraining
  no_additional_training: No reinforcement learning or fine-tuning required
  model_agnostic: Compatible with different foundation models
safety_evaluation:
  adversarial_examples: 1,200 across 40 biomedical/scientific topics
  pass_rate: 100% (all adversarial goals successfully rejected)
  mechanisms:
    - Initial research goal safety review
    - Research hypothesis safety review
    - Continuous monitoring via meta-review agent
    - Comprehensive logging and explainability
```

## Lessons Learned

### Achievements

**System Development and Architecture**:
- Successfully developed multi-agent AI system for autonomous scientific discovery without requiring specialized pre-training or reinforcement learning
- Implemented asynchronous task execution framework enabling flexible compute scaling
- Created six specialized agents (Generation, Reflection, Ranking, Evolution, Proximity, Meta-review) with distinct roles
- Established tournament-based evolution process with Elo rating system (initial 1200) for self-improving hypothesis generation
- Integrated feedback loops enabling learning without backpropagation techniques

**Performance and Validation**:
- Achieved 78.4% top-1 accuracy on GPQA diamond set
- Outperformed Gemini 2.0, OpenAI o1, OpenAI o3-mini-high, DeepSeek R1, and human expert "best guess" on challenging biomedical problems
- Demonstrated continued benefits of test-time compute scaling with no evidence of performance saturation
- Validated system in three distinct biomedical areas with different complexity levels (medium to very high)
- Expert preference ranking of 2.36 (1 = best, 4 = worst), with novelty rating 3.64/5 and impact rating 3.09/5

**Drug Repurposing**:
- Generated 78 drug repurposing proposals evaluated by 6 board-certified oncologists
- Identified Binimetinib with IC50 of 7 nM in MOLM-13 cells (clinically applicable concentration)
- Discovered novel candidate KIRA6 (no prior AML evidence) with IC50 range 13-817 nM across multiple AML cell lines
- Demonstrated high concordance between AI scores and DepMap dependency scores

**Target Discovery**:
- Identified 3 novel epigenetic targets for liver fibrosis
- 2 of 4 tested drugs showed significant anti-fibrotic activity in human hepatic organoids
- One identified drug is FDA-approved for another indication, enabling potential expedited repurposing
- Minimal cellular toxicity at effective concentrations

**Mechanism Discovery**:
- Recapitulated ~10 years of experimental research in 2 days (building on decades of prior literature)
- Independently discovered cf-PICI tail interaction mechanism matching unpublished findings
- Proposed mechanism now under peer review at established journal

**Safety and Collaboration**:
- Passed 100% of 1,200 adversarial safety tests across 40 topics
- Established scientist-in-the-loop collaborative paradigm
- Integrated specialized tools (AlphaFold, web search, databases) for enhanced validation
- Implemented comprehensive safety mechanisms: goal review, hypothesis review, continuous monitoring, logging

### Implications

**For Scientific Discovery**:
- Opens new possibilities for AI-augmented scientific discovery across disciplines
- Demonstrates value of test-time compute scaling for scientific reasoning without additional training
- Addresses breadth-depth conundrum: enables deep domain expertise with broad trans-disciplinary knowledge synthesis
- Provides framework for scalable scientific discovery workflows
- Shows potential for "raising the tide" of scientific progress, benefiting resource-constrained areas

**For AI Architecture**:
- Demonstrates effectiveness of multi-agent systems with specialized roles
- Shows value of tournament-based evolution for iterative improvement
- Validates feedback loop approach using meta-review without backpropagation
- Proves model-agnostic architecture benefits from underlying LLM improvements
- Illustrates power of inductive biases from scientific method in system design

**For Drug Discovery and Development**:
- Enables faster research progress through AI-human collaboration
- Provides evidence-based rationales for drug repurposing with mechanistic insights
- Can generate structured outputs (NIH Specific Aims Pages) facilitating regulatory submissions
- Particularly valuable for orphan drugs with existing safety data
- Supports compassionate use applications for patients with refractory diseases

**For Biomedicine**:
- Accelerates hypothesis generation for complex diseases (AML, liver fibrosis)
- Enables parallel discovery of mechanisms (antimicrobial resistance)
- Supports identification of novel therapeutic targets with experimental validation protocols
- Bridges computational prediction with experimental validation

**For Research Equity**:
- Potential to democratize access to scientific information and accelerate discovery
- Can benefit historically neglected and resource-constrained research areas
- May enable researchers with limited resources to compete with well-funded laboratories
- Risk of homogenization requires careful mitigation through design

### Challenges

**Technical Limitations**:
- Literature search limited to open-access publications (licensing/access restrictions may cause missed work)
- No access to negative results data (publication bias affects knowledge base)
- Multimodal reasoning over figures/charts not fully optimized despite frontier model capabilities
- Limited evaluation of integration with domain-specific datasets (multi-omics, knowledge graphs)
- Need for better metrics beyond Elo rating for hypothesis quality assessment
- Inherited limitations from foundation LLMs (factuality, hallucinations, biases)

**Methodological Challenges**:
- Requires careful validation of AI-generated hypotheses through expert review and experimental testing
- Need to ensure novelty and originality (not just literature synthesis)
- Distinguishing primary drivers from downstream consequences in proposed mechanisms
- Balancing AI autonomy with human oversight to prevent automation bias
- Integration with experimental validation workflows requires expert prioritization
- Scaling to more complex research domains beyond biomedical sciences
- Ensuring reproducibility and reliability of generated hypotheses across runs

**Evaluation and Validation**:
- Elo rating is auto-evaluation metric, not based on independent ground truth
- May favor certain attributes not aligned with scientist preferences
- Comprehensive systematic evaluation across diverse disciplines needed
- Need for objective, less intrinsically-favored evaluation metrics
- Small-scale expert evaluations (11 goals) require larger studies for conclusive findings
- Translation from in vitro success to clinical efficacy highly uncertain

**Safety and Ethics**:
- Dual-use risks: potential misuse for harmful research despite safeguards
- Need for evolving ethics frameworks and policy for advanced AI in science
- Adversarial robustness requires continuous testing and improvement
- Risk of homogenization of research ideas across populations
- Potential for narrowing scientific inquiry due to correlated LLM failure modes
- LLM blind spots and performance variations across research domains

**Practical Considerations**:
- Does not access entire published literature (compliance with restrictions)
- Limited awareness of recent unpublished work or ongoing research
- Requires significant computational resources for test-time compute scaling
- Need for specialized domain expertise to evaluate and prioritize hypotheses
- Integration with laboratory automation systems still experimental
- Complex experimental designs (multi-step, conditional logic) require further development

### Impact on Field

**Transformative Potential**:
The AI co-scientist demonstrates the potential to augment biomedical and scientific discovery, ushering in an era of AI-empowered scientists. By combining broad knowledge synthesis with deep domain expertise, the system addresses key challenges in modern scientific research and accelerates the pace of discovery across multiple biomedical domains.

**Paradigm Shift**:
Represents a shift from specialized AI tools toward AI as active collaborator in the complete research workflow. Not intended to automate scientific discovery, but to augment human scientists in hypothesis generation, literature synthesis, and experimental planning.

**Validation of Approach**:
End-to-end validation through wet-lab experiments in three distinct areas (varying complexity: medium, high, very high) demonstrates practical utility beyond theoretical capabilities. Results detailed in separate, co-timed technical reports for each validation area.

**Future Implications**:
- Test-time compute scaling with scientific reasoning priors enables improvement without retraining
- Model-agnostic design benefits from continued LLM advancement
- Integration of specialized AI tools (AlphaFold) demonstrates composable AI systems
- Tournament-based evolution creates reusable framework for other domains
- Scientist-in-the-loop design ensures human judgment remains central to discovery process

**Broader Context**:
System designed to help scientists "traverse and expertly reason across disciplinary domains" similar to historical breakthroughs (CRISPR, neural networks). Aims to empower scientists in creatively bridging breadth and depth, ultimately accelerating fundamental research in science and medicine while maintaining rigorous validation standards.

## Organizations

### Google Cloud AI Research
**Role in Project**: primary  
**Role Description**: Primary research organization developing the AI co-scientist system  
**Contribution**: Development of multi-agent AI system architecture, specialized agents, and core research framework  
**Organization Type**: research_center  
**Status**: active  
**Website**: https://cloud.google.com/ai  
**Description**: Google Cloud AI Research division focused on advancing AI research and applications

### Google Research
**Role in Project**: primary  
**Role Description**: Primary research organization contributing to AI co-scientist development  
**Contribution**: Research contributions to hypothesis generation, validation methodologies, and biomedical applications  
**Organization Type**: research_center  
**Status**: active  
**Website**: https://research.google/  
**Description**: Google's central research organization advancing the state of the art in AI and other fields

### Google DeepMind
**Role in Project**: primary  
**Role Description**: Primary research organization providing Gemini 2.0 foundation model  
**Contribution**: Development of Gemini 2.0 foundation model and integration with co-scientist system  
**Organization Type**: research_center  
**Status**: active  
**Website**: https://deepmind.google/  
**Description**: Google DeepMind, leading AI research lab developing advanced AI systems including Gemini models

### Houston Methodist
**Role in Project**: collaborator  
**Role Description**: Collaborating medical institution  
**Contribution**: Biomedical research expertise and validation support  
**Organization Type**: institution  
**Status**: active  
**Website**: https://www.houstonmethodist.org/  
**Description**: Leading medical institution providing clinical and research expertise

### Sequome
**Role in Project**: collaborator  
**Role Description**: Collaborating biotechnology company  
**Contribution**: Research collaboration and validation support  
**Organization Type**: company  
**Status**: active  
**Description**: Biotechnology company collaborating on research validation

### Fleming Initiative and Imperial College London
**Role in Project**: collaborator  
**Role Description**: Collaborating research institution  
**Contribution**: Research collaboration, particularly in bacterial evolution and antimicrobial resistance studies  
**Organization Type**: institution  
**Status**: active  
**Website**: https://www.imperial.ac.uk/  
**Description**: Research collaboration between Fleming Initiative and Imperial College London, focusing on bacterial research and antimicrobial resistance

### Stanford University
**Role in Project**: collaborator  
**Role Description**: Collaborating research institution  
**Contribution**: Research collaboration and validation support  
**Organization Type**: institution  
**Status**: active  
**Website**: https://www.stanford.edu/  
**Description**: Leading research university providing research collaboration and validation support

## Products

### AI Co-Scientist System
**Type**: platform  
**Status**: published  
**Development Stage**: Research / Preclinical  
**Description**: Multi-agent AI system for autonomous scientific discovery built on Gemini 2.0. The system includes specialized agents for hypothesis generation, reflection, ranking, evolution, proximity evaluation, and meta-review. It employs a generate-debate-evolve approach with tournament-based evolution for continuous improvement.

**Capabilities**:
- Natural language research goal specification
- Literature search and synthesis
- Novel hypothesis generation
- Hypothesis debate and ranking
- Tournament-based evolution
- Research proposal generation
- Tool integration (web search, AlphaFold, specialized AI models)
- Scientist-in-the-loop collaboration

**Technical Details**:
```yaml
foundation_model: Gemini 2.0
architecture: Multi-agent architecture with specialized agents
agents:
  - Generation Agent: Generates novel research hypotheses
  - Reflection Agent: Self-critique and reflection
  - Ranking Agent: Compares and ranks hypotheses through scientific debate
  - Evolution Agent: Evolves hypotheses through tournament process
  - Proximity Agent: Evaluates relatedness of hypotheses
  - Meta-review Agent: Provides high-level analysis
workflow: Generate-debate-evolve approach with tournament evolution
compute_scaling: Test-time compute scaling for iterative improvement
tool_integration: Web search, AlphaFold, specialized AI models
```

### Specialized Agents

The AI co-scientist system includes six specialized agents, each with specific roles and methodologies:

#### 1. Generation Agent

**Primary Function**: Generate initial focus areas and novel research hypotheses

**Techniques Employed**:
- **Literature Exploration via Web Search**: Iteratively searches, retrieves, and reads research articles, grounding reasoning in prior work
- **Simulated Scientific Debates**: Self-play multi-turn conversations among experts leading to refined hypotheses
- **Iterative Assumptions Identification**: Identifies testable intermediate assumptions through conditional reasoning hops
- **Research Expansion**: Reviews existing hypotheses and meta-reviews to identify unexplored areas

**Output**: Initial hypothesis pool with categorization and core idea summaries for rapid scientist comprehension

#### 2. Reflection Agent

**Primary Function**: Critical peer review of hypotheses for correctness, quality, and novelty

**Review Types**:
- **Initial Review**: Quick assessment without external tools to filter obviously flawed hypotheses
- **Full Review**: Comprehensive review leveraging web search and literature to evaluate:
  - Correctness and quality of reasoning
  - Novelty assessment based on existing literature
  - Supporting and contradicting evidence
- **Deep Verification Review**: 
  - Decomposes hypothesis into constituent assumptions
  - Breaks assumptions into fundamental sub-assumptions
  - Independently evaluates each for correctness
  - Identifies invalidating elements with detailed reasoning
- **Observation Review**: Explores whether hypothesis explains long-tail observations from experimental results
- **Simulation Review**: Step-wise simulation of mechanism of action or proposed experiments to identify failure scenarios
- **Recurrent/Tournament Review**: Adapts reviews based on growing system knowledge and tournament results

**Integration**: Can incorporate reviews from expert scientists for enhanced guidance

#### 3. Ranking Agent

**Primary Function**: Automatic evaluation and ranking using Elo-based tournament

**Tournament Methodology**:
- **Elo Rating System**: Initial rating of 1200 for new hypotheses
- **Pairwise Comparisons**: 
  - Top-ranked hypotheses: Multi-turn scientific debates
  - Lower-ranked hypotheses: Single-turn comparisons
- **Optimization Strategies**:
  - Prioritizes similar hypotheses (via Proximity agent graph)
  - New and top-ranking hypotheses prioritized for matches
  - Successful hypotheses quickly achieve favorable rankings
- **Scientific Debate Process**: Simulates panel discussions evaluating novelty, correctness, testability
- **Decision Output**: Clear determination of superior hypothesis with supporting rationale

**Purpose**: Communicates ordered list of hypotheses to scientists, guides computational resource allocation

#### 4. Evolution Agent

**Primary Function**: Continuous refinement and improvement of existing hypotheses

**Improvement Approaches**:
- **Enhancement through Grounding**: Identifies weaknesses, retrieves articles, fills reasoning gaps
- **Coherence and Feasibility**: Addresses issues with invalid assumptions, improves practicality
- **Inspiration from Existing Hypotheses**: Creates new hypotheses inspired by top-ranked candidates
- **Combination**: Merges best aspects of multiple top-ranking hypotheses
- **Simplification**: Makes hypotheses easier to verify and test
- **Out-of-box Thinking**: Explores divergent ideas moving away from current hypothesis subset

**Strategy**: Generates new hypotheses rather than modifying existing ones to protect top-ranked quality; new hypotheses must compete in tournament

#### 5. Proximity Agent

**Primary Function**: Calculate similarity and build proximity graph of hypotheses

**Capabilities**:
- Computes hypothesis similarity relative to research goal
- Builds proximity graph for hypothesis organization
- Enables clustering of similar ideas
- Facilitates de-duplication
- Supports efficient exploration of hypothesis landscape
- Assists Ranking agent in organizing tournament matches
- Helps scientists quickly identify related concepts

**Impact**: Showcases diverse range of ideas, enables rapid exploration of interest areas

#### 6. Meta-review Agent

**Primary Function**: Enable self-improvement through feedback loop synthesis

**Key Activities**:
- **Pattern Identification**: Synthesizes insights from all reviews, identifies recurring patterns in tournament debates
- **Feedback Generation**: Provides feedback to Reflection agent for more thorough future reviews
- **Issue Prevention**: Prevents recurrence of common problems in hypothesis generation
- **Research Overview Generation**: Synthesizes top-ranked hypotheses into comprehensive research roadmap
- **Research Contacts Identification**: Suggests qualified domain experts for review and collaboration
- **Format Adaptation**: Can format outputs using constrained decoding (e.g., NIH Specific Aims Page format)

**Feedback Mechanism**: Insights appended to agent prompts in next iteration (leveraging Gemini 2.0 long-context capabilities), enabling learning without backpropagation

**Example Impact**: If 90% of reviews identify an issue (e.g., blood-brain barrier permeability), meta-review ensures 100% of future reviews address this factor

## Key People

### Juraj Gottweis
**Title**: PhD  
**Participation Type**: researcher  
**Role**: Co-first Author, Researcher  
**Affiliations**: Google Cloud AI Research  
**Contribution**: Co-first author, conceptualization, methodology, writing

### Wei-Hung Weng
**Title**: PhD  
**Participation Type**: researcher  
**Role**: Co-first Author, Researcher  
**Affiliations**: Google Research  
**Contribution**: Co-first author, conceptualization, methodology, writing

### Alexander Daryin
**Title**: PhD  
**Participation Type**: researcher  
**Role**: Co-first Author, Researcher  
**Affiliations**: Google Cloud AI Research  
**Contribution**: Co-first author, conceptualization, methodology, writing

### Tao Tu
**Title**: PhD  
**Participation Type**: researcher  
**Role**: Co-first Author, Researcher  
**Affiliations**: Google DeepMind  
**Contribution**: Co-first author, conceptualization, methodology, writing

### Vivek Natarajan
**Title**: PhD  
**Participation Type**: pi  
**Role**: Corresponding Author, Principal Investigator  
**Affiliations**: Google Research  
**Contribution**: Corresponding author, supervision, conceptualization  
**Email**: natviv@google.com

### Alan Karthikesalingam
**Title**: PhD  
**Participation Type**: pi  
**Role**: Corresponding Author, Principal Investigator  
**Affiliations**: Google Research  
**Contribution**: Corresponding author, supervision, conceptualization  
**Email**: alankarthi@google.com

### Annalisa Pawlosky
**Title**: PhD  
**Participation Type**: pi  
**Role**: Corresponding Author, Principal Investigator  
**Affiliations**: Google Cloud AI Research  
**Contribution**: Corresponding author, supervision  
**Email**: apawlosky@google.com

## Links

### [Towards an AI co-scientist](https://storage.googleapis.com/coscientist_paper/ai_coscientist.pdf)
**Type**: research_publication  
**Relevance**: primary  
**Category**: publication  
**Description**: Primary research paper describing the AI co-scientist multi-agent system built on Gemini 2.0  
**Publisher**: Google Research  
**Publication Date**: 2025-02-18  
**Authors**: Juraj Gottweis, Wei-Hung Weng, Alexander Daryin, Tao Tu, and co-authors

### [Google DeepMind](https://deepmind.google/)
**Type**: website  
**Relevance**: secondary  
**Category**: source  
**Description**: Google DeepMind website - developer of Gemini 2.0 foundation model

### [Google Research](https://research.google/)
**Type**: website  
**Relevance**: secondary  
**Category**: source  
**Description**: Google Research website

### [Google Cloud AI](https://cloud.google.com/ai)
**Type**: website  
**Relevance**: secondary  
**Category**: source  
**Description**: Google Cloud AI Research website

## Events

### Publication of AI Co-Scientist Paper
**Date**: 2025-02-18  
**Type**: publication  
**Description**: Publication of primary research paper "Towards an AI co-scientist" describing the multi-agent system built on Gemini 2.0, with end-to-end validation in three biomedical areas detailed in separate co-timed reports  
**Details**:
```yaml
title: "Towards an AI co-scientist"
venue: Google Research
publication_type: Research Paper
significance: First comprehensive documentation of multi-agent AI co-scientist system with wet-lab validation
key_contributions:
  - Multi-agent architecture with asynchronous task execution framework
  - Tournament evolution process for self-improving hypothesis generation
  - Scientist-in-the-loop collaborative workflow
  - End-to-end validation in drug repurposing, target discovery, and antimicrobial resistance
validation_areas:
  drug_repurposing:
    disease: Acute Myeloid Leukemia (AML)
    key_results: Binimetinib IC50 7 nM, KIRA6 IC50 13-817 nM
    validation: In vitro cell line experiments
  target_discovery:
    disease: Liver Fibrosis
    key_results: 3 novel epigenetic targets, 2 drugs with anti-fibrotic activity
    validation: Human hepatic organoids
  mechanism_discovery:
    topic: Bacterial evolution and antimicrobial resistance (cf-PICIs)
    key_results: Recapitulated ~10 years of research in 2 days
    validation: Independent experimental findings (under peer review)
performance_metrics:
  gpqa_accuracy: 78.4%
  expert_preference_rank: 2.36 (out of 4, lower is better)
  safety_test_pass_rate: 100% (1,200 adversarial examples)
  research_goals_analyzed: 203 distinct goals
```

### Co-timed Validation Reports
**Date**: 2025-02-18  
**Type**: publication  
**Description**: Three separate technical reports detailing experimental validation of AI co-scientist hypotheses published simultaneously with main paper  
**Details**:
```yaml
reports:
  - topic: Drug repurposing for AML
    focus: In vitro validation of repurposing candidates
    key_findings: Novel candidates with clinically applicable IC50 values
  - topic: Liver fibrosis target discovery
    focus: Epigenetic target validation in hepatic organoids
    key_findings: Anti-fibrotic activity and liver cell regeneration
  - topic: Bacterial evolution mechanism (cf-PICIs)
    focus: Parallel in silico discovery matching experimental findings
    key_findings: Capsid-tail interaction mechanism for broad host range
    status: Under peer review at established journal
```

## Partnerships

### Research Collaboration
**Date**: 2024  
**Type**: research  
**Focus**: Multi-institutional collaboration for AI co-scientist development and validation  
**Description**: Collaboration between Google Cloud AI Research, Google Research, Google DeepMind, and external partners including Houston Methodist, Sequome, Fleming Initiative/Imperial College London, and Stanford University  
**Partner Organizations**:
- Google Cloud AI Research (primary)
- Google Research (primary)
- Google DeepMind (primary)
- Houston Methodist (collaborator)
- Sequome (collaborator)
- Fleming Initiative and Imperial College London (collaborator)
- Stanford University (collaborator)

