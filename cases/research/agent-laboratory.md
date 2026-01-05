---
id: agent-laboratory
slug: agent-laboratory
entity_type: research
status: published
data_completeness: exceptional
last_researched: 2025-01-20
research_category: collaboration
researcher: AI Assistant
version: 2.0
name: "Agent Laboratory: Using LLM Agents as Research Assistants"
description: An autonomous LLM-based framework capable of completing the entire research process from initial conception to final results. The system accepts a human-provided research idea and progresses through three stages—literature review, experimentation, and report writing—to produce comprehensive research outputs, including a code repository and a research report, while enabling users to provide feedback and guidance at each stage. Agent Laboratory achieves an 84% cost reduction compared to previous autonomous research methods (The AI Scientist costing ~$15 vs Agent Laboratory at $2.33 with gpt-4o), with generated ML code achieving state-of-the-art performance on MLE-Bench challenges, earning more medals than MLAB, OpenHands, and AIDE.
mission: To accelerate scientific discovery, reduce research costs, and improve research quality by enabling researchers to allocate more effort toward creative ideation rather than low-level coding and writing, ultimately accelerating scientific discovery.
entity_data:
  name: Agent Laboratory
  status: published
  objectives:
    - Complete entire research process autonomously from conception to results
    - Generate comprehensive research outputs including code repository and research report
    - Enable human feedback and guidance at each research stage
    - Reduce research costs compared to previous autonomous methods
    - Improve research quality through human-AI collaboration
  start_date: 2024
  publication_date: 2025-01-08
  completion_date: 2025-06-17
  methodology:
    type: Autonomous LLM-based Research Framework
    framework: Three-stage research pipeline
    integration_level: Fully autonomous with human feedback integration
    key_innovation: Complete research process automation with human-in-the-loop feedback
    stages:
      - Literature Review Stage
      - Experimentation Stage
      - Report Writing Stage
    human_feedback: Users can provide feedback and guidance at each stage
  results:
    best_performing_model: o1-preview generates best research outcomes
    code_performance: Generated machine learning code achieves state-of-the-art performance compared to existing methods
    human_impact: Human involvement providing feedback at each stage significantly improves overall quality of research
    cost_reduction: 84% decrease in research expenses compared to previous autonomous research methods ($2.33 USD vs ~$15 USD for The AI Scientist)
    outputs: Comprehensive research outputs including code repository and research report
    human_evaluation_autonomous:
      usefulness:
        gpt_4o: 4.0/5
        o1_mini: 4.3/5
        o1_preview: 4.4/5
      report_quality:
        gpt_4o: 3.0/5
        o1_mini: 3.2/5
        o1_preview: 3.4/5
      experimental_quality:
        gpt_4o: 2.6/5
        o1_mini: 3.2/5
        o1_preview: 2.9/5
    neurips_scores_autonomous:
      overall:
        gpt_4o: 3.5/10
        o1_mini: 3.8/10
        o1_preview: 4.0/10
      quality:
        gpt_4o: 1.8/4
        o1_mini: 2.3/4
        o1_preview: 2.1/4
      clarity:
        gpt_4o: 2.6/4
        o1_mini: 2.1/4
        o1_preview: 2.5/4
      soundness:
        gpt_4o: 1.7/4
        o1_mini: 1.8/4
        o1_preview: 2.2/4
      contribution:
        average: 2.1/4
    copilot_evaluation:
      utility: 3.5/5
      continuation: 3.75/5
      satisfaction: 3.63/5
      usability: 4.0/5
      custom_topics:
        utility: 3.75/5
        continuation: 4.0/5
        satisfaction: 3.75/5
        usability: 3.75/5
      preselected_topics:
        utility: 3.25/5
        continuation: 3.5/5
        satisfaction: 3.5/5
        usability: 4.25/5
    copilot_vs_autonomous:
      self_evaluation_overall: 4.13/10 vs 3.8/10 autonomous (+0.33)
      external_evaluation_overall: 4.38/10 vs 3.8/10 autonomous (+0.58)
      quality_improvement: +0.75
      soundness_improvement: +0.48
      clarity_improvement: +0.23
      presentation_improvement: +0.33
    mle_bench_performance:
      medals_earned: 4 (2 gold, 1 silver, 1 bronze)
      comparison_mlab: 0 medals
      comparison_openhands_gpt4o: 2 medals (2 gold)
      comparison_aide_o1preview: 2 medals (1 gold, 1 bronze)
      above_median_human: 6 out of 10 benchmarks
      submission_rate: 100% (all challenges submitted within 2 hours)
    automated_vs_human_review_gap:
      automated_overall: 6.1/10
      human_overall: 3.8/10
      discrepancy: -2.3 points
      clarity_gap: automated 3.6/4 vs human 2.4/4
      note: "Automated reviews significantly overestimate quality, demonstrating need for human feedback"
  collaboration_period:
    start: 2024
    publication_date: 2025-01-08
    status: published
  arxiv_versions:
    v1: 2025-01-08
    v2: 2025-06-17 (final version)
  runtime_statistics:
    gpt_4o:
      total_time: 1165.4 seconds (19.4 minutes)
      total_cost: $2.33 USD
      success_rate: 94.3%
      literature_review: 92.9s, $0.12, 60% success
      plan_formulation: 23.3s, $0.03, 100% success
      data_preparation: 55.4s, $0.09, 100% success
      running_experiments: 417.8s, $0.42, 100% success
      results_interpretation: 3.5s, $0.04, 100% success
      report_writing: 572.5s, $1.73, 100% success
      report_refinement: 0.0s, $0.00, 100% success
    o1_mini:
      total_time: 3616.8 seconds (60.3 minutes)
      total_cost: $7.51 USD
      success_rate: 92.8%
      literature_review: 56.8s, $0.16, 70% success
      plan_formulation: 35.5s, $0.04, 100% success
      data_preparation: 309.7s, $3.03, 80% success
      running_experiments: 2082.5s, $1.59, 100% success
      results_interpretation: 304.6s, $0.11, 100% success
      report_writing: 827.7s, $2.58, 100% success
      report_refinement: 0.0s, $0.00, 100% success
    o1_preview:
      total_time: 6201.3 seconds (103.4 minutes)
      total_cost: $13.10 USD
      success_rate: 95.7%
      literature_review: 97.8s, $0.29, 80% success
      plan_formulation: 33.1s, $0.04, 100% success
      data_preparation: 167.9s, $0.30, 90% success
      running_experiments: 4036.2s, $2.89, 100% success
      results_interpretation: 11.9s, $0.00, 100% success
      report_writing: 1854.2s, $9.58, 100% success
      report_refinement: 0.2s, $0.00, 100% success
    comparison_with_ai_scientist: 6.4x cost reduction (Agent Laboratory $2.33 vs AI Scientist ~$15 with gpt-4o)
    hardware: 2023 MacBook Pro with Apple M3 Max processor and 36 GB memory
  author_contributions:
    methodology:
      - Samuel Schmidgall (AMD, Johns Hopkins University)
      - Yusheng Su (AMD)
      - Ze Wang (AMD)
      - Ximeng Sun (AMD)
      - Jialian Wu (AMD)
      - Xiaodong Yu (AMD)
      - Jiang Liu (AMD)
      - Michael Moor (ETH Zurich)
      - Zicheng Liu (AMD)
      - Emad Barsoum (AMD)
  corresponding_author:
    name: Samuel Schmidgall
    email: sschmi46@jhu.edu
    affiliations:
      - AMD
      - Johns Hopkins University
taxonomy:
  geography: USA
  ai_approach:
    - Generative AI
  ai_technology:
    - LLMs
    - Multi-Agent AI
    - Generative AI
  primary_focus:
    - Autonomous AI Scientists
  aging_approach: []
  target_biology: []
  ai_architecture:
    - LLMs
  ai_specialization:
    - Multi-Agent AI
  development_stage: Research / Preclinical
  therapeutic_modality: []
  organization_type: research
  organization_subtype: collaboration
organizations:
  - name: AMD
    role: primary
    org_type: company
    status: operational
    legal_name: Advanced Micro Devices, Inc.
    website: "https://www.amd.com/"
    role_description: Primary research organization
    contribution_description: AMD is the primary organization that developed Agent Laboratory, with 9 out of 10 authors affiliated with AMD including corresponding author Samuel Schmidgall. AMD provided the research infrastructure and resources for developing the autonomous research framework.
    description: Global semiconductor company and technology provider
    focus: High-performance computing, processors, graphics, and AI acceleration
  - name: Johns Hopkins University
    role: collaborator
    org_type: institution
    legal_name: Johns Hopkins University
    status: active
    website: "https://www.jhu.edu/"
    role_description: Academic collaborating institution
    contribution_description: Johns Hopkins University provided academic collaboration and research expertise through Samuel Schmidgall's affiliation. Contributed to the theoretical foundations and evaluation methodologies.
    description: Private research university in Baltimore, Maryland
    focus: Research, medical education, computer science, and engineering
  - name: ETH Zurich
    role: collaborator
    org_type: institution
    legal_name: Swiss Federal Institute of Technology Zurich
    status: active
    website: "https://ethz.ch/"
    role_description: International academic collaborator
    contribution_description: ETH Zurich contributed through Michael Moor's expertise in machine learning and AI systems for scientific applications.
    description: Public research university in Zurich, Switzerland, one of the leading universities for technology and natural sciences
    focus: Engineering, mathematics, natural sciences, computer science
products:
  - name: Agent Laboratory Framework
    type: platform
    status: published
    development_stage: Research / Preclinical
    description: Autonomous LLM-based framework for complete research process automation. Accepts human-provided research ideas and progresses through literature review, experimentation, and report writing stages to produce comprehensive research outputs. Framework is compute-flexible, allowing various levels of compute allocation based on user's access to resources (CPU, GPU, memory) and model inference budget.
    capabilities:
      - Autonomous literature review with arXiv API integration
      - Automated experimentation via mle-solver
      - Research report generation via paper-solver
      - Code repository generation
      - Human feedback integration at each stage (co-pilot mode)
      - Support for multiple LLM models (gpt-4o, o1-mini, o1-preview)
      - Autonomous and co-pilot operating modes
      - Specialized agents (PhD, Postdoc, ML Engineer, Professor roles)
      - Compute-flexible architecture
    components:
      - name: PhD Agent
        role: Literature review, plan formulation, results interpretation
        description: Acts as PhD student collecting papers, discussing plans, and interpreting results
      - name: Postdoc Agent
        role: Plan validation, results guidance
        description: Directs PhD student through dialogue to refine plans and interpretations
      - name: ML Engineer Agent
        role: Data preparation, code generation
        description: Writes and executes Python code for data preparation under PhD guidance
      - name: Professor Agent
        role: Scoring and evaluation
        description: Expert reward model assessing code quality and report quality
      - name: mle-solver
        role: Automated experimentation
        description: Specialized module for generating, testing, and refining ML code autonomously
      - name: paper-solver
        role: Report generation
        description: Specialized module for iteratively generating and refining research reports
    technical_details:
      ai_methods: LLM-based multi-agent system with specialized agents
      architecture: Three-stage pipeline (literature review, experimentation, report writing) with human feedback integration
      performance_metrics: 84% cost reduction, SOTA ML code performance, 4 medals on MLE-Bench
      llm_models: gpt-4o (fastest, cheapest), o1-mini (highest experimental quality), o1-preview (best overall, most useful)
      temperature_settings:
        agent_temperature: 0.8
        score_generation: 0.6
        code_repair: 0.8
        initial_code: 1.0
        solver: 1.0
        initial_paper: 0.8
      hyperparameters:
        literature_review:
          number_of_summaries: 5
          full_text_decay_steps: 3
        running_experiments:
          mle_solver_steps: 3
          code_repair_attempts: 2
          maximum_top_codes: 2
          error_history_length: 5
          code_history_length: 2
          experiment_timeout: 600s
        data_preparation:
          experiment_timeout: 120s
        report_writing:
          paper_solver_steps: 5
          maximum_top_papers: 1
          paper_history_length: 10
          number_of_reviewers: 1
        report_refinement:
          number_of_reviewers: 3
  - name: mle-solver
    type: ai_model
    status: operational
    development_stage: Operational
    description: Specialized module designed to generate, test, and refine machine learning code autonomously. Uses iterative tree-search approach with LLM-based scoring to optimize experimental code. Achieved superior performance on MLE-Bench compared to MLAB, OpenHands, and AIDE.
    capabilities:
      - Autonomous code generation from research plans
      - Iterative code refinement through EDIT and REPLACE operations
      - Automatic compilation checking and error repair
      - LLM-based program scoring (0-1 scale)
      - Self-reflection on errors and successes
      - Performance stabilization through top program sampling
      - Batch parallelization for code modifications
    technical_details:
      workflow:
        - Command Execution (REPLACE and EDIT operations)
        - Code Execution (compilation checking and error repair)
        - Program Scoring (LLM reward model 0-1 scale)
        - Self-Reflection (learning from errors and successes)
        - Performance Stabilization (top program sampling, batch parallelization)
      repair_attempts: 3 (Nrep=3)
      scoring_function: LLM reward model evaluates alignment with research plan
      tree_search: Similar to reasoning tree search but traversing program space
      comparison_to_aide: Similar solution space search but for general research vs Kaggle-specific
      error_prevention:
        - Detects and removes exit() commands
        - Prevents subprocess.run() system commands
        - Validates code compilation before acceptance
      performance:
        medals_earned: 4 (2 gold, 1 silver, 1 bronze)
        submission_rate: 100% (all challenges within 2 hours)
        above_median_human: 6/10 benchmarks
  - name: paper-solver
    type: ai_model
    status: operational
    development_stage: Operational
    description: Specialized module for iteratively generating and refining academic research reports. Creates LaTeX-formatted papers following standard academic structure with automated review-based improvement. Uses adapted NeurIPS automated review system from The AI Scientist.
    capabilities:
      - Initial report scaffold generation (8 standard sections)
      - arXiv literature search during writing
      - Iterative report editing with LaTeX compilation
      - Automated peer review using LLM-based NeurIPS reviewers
      - EDIT and REPLACE operations for precise modifications
    technical_details:
      workflow:
        - Initial Report Scaffold (8 sections structure)
        - arXiv Research (optional literature search per section)
        - Report Editing (iterative EDIT command refinement)
        - Paper Review (LLM-based NeurIPS reviewers)
      paper_structure:
        - Abstract
        - Introduction
        - Background
        - Related Work
        - Methods
        - Experimental Setup
        - Results
        - Discussion
      review_system: Adapted from The AI Scientist (Lu et al. 2024)
      review_metrics: Quality, Significance, Clarity, Soundness, Presentation, Contribution, Overall (1-10), Confidence
      review_accuracy: 65% automated vs 66% human on ICLR 2022 papers
      latex_compilation: Automatic checking after each edit
      target_length: 8 pages or 4000 words
      note: Not meant to replace human paper writing, but provide readable summary of research accomplished
links:
  - url: "https://arxiv.org/abs/2501.04227"
    type: research_publication
    title: "Agent Laboratory: Using LLM Agents as Research Assistants"
    relevance: primary
    category: publication
    description: Main arXiv preprint describing the Agent Laboratory framework, methodology, architecture, experimental results, and comprehensive evaluation including human studies
    publisher: arXiv
    publication_date: 2025-01-08
    authors:
      - Samuel Schmidgall
      - Yusheng Su
      - Ze Wang
      - Ximeng Sun
      - Jialian Wu
      - Xiaodong Yu
      - Jiang Liu
      - Michael Moor
      - Zicheng Liu
      - Emad Barsoum
    metadata:
      arxiv_id: "2501.04227"
      doi: "10.48550/arXiv.2501.04227"
      version: v2 (revised 2025-06-17)
      subjects:
        - Human-Computer Interaction (cs.HC)
        - Artificial Intelligence (cs.AI)
        - Computation and Language (cs.CL)
        - Machine Learning (cs.LG)
      pages: 83 pages
      abstract_excerpt: "Historically, scientific discovery has been a lengthy and costly process, demanding substantial time and resources from initial conception to final results. To accelerate scientific discovery, reduce research costs, and improve research quality, we introduce Agent Laboratory, an autonomous LLM-based framework capable of completing the entire research process."
  - url: "https://AgentLaboratory.github.io"
    type: website
    title: Agent Laboratory - Official Project Website
    relevance: primary
    category: source
    description: Official project website for Agent Laboratory with documentation, examples, and resources
  - url: "https://github.com/SamuelSchmidgall/AgentLaboratory"
    type: github
    title: Agent Laboratory - GitHub Repository
    relevance: primary
    category: source
    description: Official open-source GitHub repository containing Agent Laboratory implementation, code, documentation, and examples. Includes mle-solver and paper-solver implementations.
    metadata:
      repository: SamuelSchmidgall/AgentLaboratory
      license: Open source
      features:
        - Complete Agent Laboratory framework
        - mle-solver implementation
        - paper-solver implementation
        - Example research projects
        - Configuration files
        - Documentation and tutorials
---

# Agent Laboratory: Using LLM Agents as Research Assistants

## Description

Agent Laboratory is an autonomous LLM-based framework capable of completing the entire research process from initial conception to final results. Historically, scientific discovery has been a lengthy and costly process, demanding substantial time and resources from initial conception to final results. To accelerate scientific discovery, reduce research costs, and improve research quality, Agent Laboratory accepts a human-provided research idea and progresses through three distinct stages—literature review, experimentation, and report writing—to produce comprehensive research outputs, including a code repository and a research report.

Unlike previous approaches where agents participate in their own research ideation independent of human input (e.g., ResearchAgent, The AI Scientist), Agent Laboratory is designed to assist human scientists in executing their own research ideas using language agents. The framework enables users to provide feedback and guidance at each stage, creating a human-in-the-loop collaboration that significantly improves the overall quality of research. This approach allows researchers to allocate more effort toward creative ideation and experiment design rather than low-level coding and writing, ultimately accelerating scientific discovery.

**Key Innovation**: Agent Laboratory is compute-flexible, where various levels of compute can be allocated based on the individual's access to compute resources (e.g., CPU, GPU, memory) and model inference budget. The framework can operate in two modes: (1) **autonomous mode** where the system completes all stages without human intervention, and (2) **co-pilot mode** where humans provide feedback and guidance at the end of each research stage.

**Cost Efficiency**: Agent Laboratory achieves an **84% cost reduction** compared to previous autonomous research methods (The AI Scientist). With gpt-4o backend, Agent Laboratory costs only **$2.33 USD per paper** compared to ~$15 USD for The AI Scientist (6.4x reduction), while with o1-preview costing $13.10 USD, still significantly more cost-effective than alternatives.

**Performance**: The generated machine learning code achieves **state-of-the-art performance** compared to existing methods. On MLE-Bench (10 ML challenges), mle-solver earned **4 medals** (2 gold, 1 silver, 1 bronze) compared to MLAB (0 medals), OpenHands with gpt-4o (2 medals), and AIDE with o1-preview (2 medals). Agent Laboratory achieved **above-median human performance** on 6 out of 10 benchmarks with **100% submission rate** (all challenges completed within 2 hours).

**Human Evaluation**: Human evaluators rated papers across experimental quality, report quality, and usefulness. Results showed that o1-preview was rated as most useful (4.4/5), o1-mini achieved highest experimental quality (3.2/5), while gpt-4o consistently scored lower across all metrics. **Co-pilot mode** with human feedback achieved higher scores than autonomous mode (+0.58 overall improvement), demonstrating the value of human-AI collaboration.

**Automated vs Human Reviews**: A significant finding revealed that automated reviewers (based on NeurIPS criteria) gave average scores of 6.1/10, while human reviewers gave 3.8/10 (-2.3 points), demonstrating that **automated reviews significantly overestimate quality** and highlighting the importance of human feedback for accurate research assessment.

## Mission

To accelerate scientific discovery, reduce research costs, and improve research quality by enabling researchers to allocate more effort toward creative ideation rather than low-level coding and writing, ultimately accelerating scientific discovery.

## Project Information

**Start Date**: 2024  
**Publication Date**: 2025-01-08 (v1), 2025-06-17 (v2)  
**Status**: Published on arXiv

## AI Methods

- LLM-based Multi-Agent System with Specialized Roles (PhD, Postdoc, ML Engineer, Professor agents)
- Autonomous Literature Review with arXiv API Integration
- Automated Experimentation via mle-solver (tree-search code generation and optimization)
- Research Report Generation via paper-solver (LaTeX generation with NeurIPS-style review)
- Human-in-the-Loop Feedback Integration (Co-pilot Mode)
- Multi-LLM Model Support (gpt-4o, o1-mini, o1-preview)
- LLM Reward Models for Code and Paper Scoring
- Self-Reflection and Iterative Improvement
- Automated Code Compilation and Error Repair
- Tree-Search Optimization for Program Space
- Batch Parallelization for Code Modifications
- Automated Peer Review System (NeurIPS Guidelines)

## System Architecture

```yaml
type: Autonomous LLM-based Research Framework with Multi-Agent Collaboration
core_innovation: Complete research process automation with human feedback integration and specialized agent roles
agent_roles:
  PhD_Agent:
    role: Primary research agent
    responsibilities:
      - Literature review using arXiv API
      - Research plan formulation (with Postdoc)
      - Results interpretation (with Postdoc)
      - Report refinement decisions
    temperature: 0.8
    commands: SUMMARY, FULL_TEXT, ADD_PAPER, DIALOGUE, SUBMIT_CODE, INTERPRETATION
  Postdoc_Agent:
    role: Supervisory research agent
    responsibilities:
      - Guide PhD in plan formulation
      - Direct PhD in results interpretation
      - Validate research direction
    commands: DIALOGUE, PLAN, INTERPRETATION
  ML_Engineer_Agent:
    role: Code implementation agent
    responsibilities:
      - Data preparation code writing
      - HuggingFace dataset search and integration
      - Python code execution and debugging
    commands: python, DIALOGUE, SEARCH_HF
  Professor_Agent:
    role: Evaluation and scoring agent
    responsibilities:
      - Score code quality (mle-solver)
      - Score paper quality (paper-solver)
      - Provide reward signals for optimization
    temperature: 0.6
stages:
  Literature_Review:
    agent: PhD_Agent
    description: Automated literature review and synthesis using arXiv API
    process:
      - 1. Query arXiv with research topic
      - 2. Retrieve top 20 paper summaries (SUMMARY command)
      - 3. Get full text for relevant papers (FULL_TEXT command)
      - 4. Add selected papers to curated review (ADD_PAPER command)
      - 5. Iterate until N papers added (N=5 in experiments)
    output: Curated literature review with paper summaries
    tools: arXiv API (summary, full text, add paper)
    success_rate: 60-80% (struggled with instruction-following)
  Plan_Formulation:
    agents: PhD_Agent, Postdoc_Agent
    description: Collaborative research plan development through dialogue
    process:
      - 1. PhD and Postdoc discuss experimental approach
      - 2. Specify ML models to implement
      - 3. Identify datasets to use
      - 4. Detail experimental steps
      - 5. Reach consensus and submit plan (PLAN command)
    output: Detailed research plan with experimental specifications
    success_rate: 100% across all models
  Data_Preparation:
    agents: PhD_Agent, ML_Engineer_Agent
    description: Code development for data preparation
    process:
      - 1. ML Engineer searches HuggingFace datasets (SEARCH_HF)
      - 2. PhD directs ML Engineer through dialogue
      - 3. ML Engineer writes Python code
      - 4. Code execution with compiler checking
      - 5. Submit when finalized (SUBMIT_CODE)
    output: Data preparation code with HuggingFace integration
    timeout: 120 seconds
    success_rate: 80-100% depending on model
  Running_Experiments:
    agent: ML_Engineer_Agent (via mle-solver)
    description: Autonomous ML code generation and optimization
    process:
      - 1. mle-solver generates initial code (REPLACE)
      - 2. Iterative refinement (EDIT command)
      - 3. Code compilation checking
      - 4. LLM-based program scoring (0-1 scale)
      - 5. Self-reflection on results
      - 6. Performance stabilization (top program sampling)
    mle_solver_steps: 3
    code_repair_attempts: 2
    maximum_top_codes: 2
    timeout: 600 seconds
    output: Experimental code repository with results
    success_rate: 100% across all models
  Results_Interpretation:
    agents: PhD_Agent, Postdoc_Agent
    description: Collaborative interpretation of experimental results
    process:
      - 1. PhD and Postdoc discuss experimental outcomes
      - 2. Analyze code and results
      - 3. Integrate literature review findings
      - 4. Formulate interpretation for paper
      - 5. Submit interpretation (INTERPRETATION command)
    output: Research interpretation with metrics and significance
    success_rate: 100% across all models
  Report_Writing:
    agents: PhD_Agent, Professor_Agent (via paper-solver)
    description: Automated LaTeX report generation with review-based refinement
    process:
      - 1. paper-solver creates initial scaffold (8 sections)
      - 2. Generate section content with arXiv research
      - 3. Iterative editing (EDIT command)
      - 4. LaTeX compilation checking
      - 5. Automated NeurIPS-style review (Professor_Agent)
    paper_solver_steps: 5
    number_of_reviewers: 1 (refinement: 3)
    target_length: 8 pages or 4000 words
    output: Complete LaTeX research report
    success_rate: 100% across all models
  Report_Refinement:
    agent: PhD_Agent
    description: Review-based paper improvement decision
    process:
      - 1. Generate 3 reviewer assessments (NeurIPS criteria)
      - 2. PhD decides: finalize or revise
      - 3. If revise: return to earlier stages for improvement
    output: Final decision on paper completion
    success_rate: 100% across all models
workflow:
  - 1. Receive research idea and notes from human user
  - 2. Literature Review Stage (PhD explores arXiv)
  - 3. Optional: Human feedback checkpoint (co-pilot mode)
  - 4. Plan Formulation (PhD + Postdoc collaboration)
  - 5. Optional: Human feedback checkpoint (co-pilot mode)
  - 6. Data Preparation (ML Engineer + PhD)
  - 7. Optional: Human feedback checkpoint (co-pilot mode)
  - 8. Running Experiments (mle-solver autonomous optimization)
  - 9. Optional: Human feedback checkpoint (co-pilot mode)
  - 10. Results Interpretation (PhD + Postdoc)
  - 11. Optional: Human feedback checkpoint (co-pilot mode)
  - 12. Report Writing (paper-solver with automated review)
  - 13. Optional: Human feedback checkpoint (co-pilot mode)
  - 14. Report Refinement (PhD decision: finalize or iterate)
  - 15. Generate final outputs: code repository and research report PDF
operating_modes:
  autonomous_mode:
    description: No human involvement except initial research idea
    process: Sequential stage progression without checkpoints
    cost: Lowest ($2.33 with gpt-4o)
    quality: Lower than co-pilot (3.8/10 average human score)
  copilot_mode:
    description: Human feedback checkpoint at end of each stage
    process: Human reviews stage output and provides feedback/guidance
    human_actions:
      - Review stage output
      - Decide to proceed or repeat stage
      - Provide high-level notes for improvement
    cost: Higher due to potential stage repetition
    quality: Higher than autonomous (4.38/10 average human score, +0.58)
    user_ratings:
      utility: 3.5/5
      continuation: 3.75/5
      satisfaction: 3.63/5
      usability: 4.0/5
human_feedback:
  integration: Users can provide feedback at checkpoints after each stage
  impact: Significantly improves overall research quality (+0.58 overall score)
  mechanism: Feedback loop allows guidance, refinement, and stage repetition
  examples:
    - Request specific paper inclusion in literature review
    - Suggest desired technique in experiments
    - Guide experimental design choices
llm_models:
  gpt_4o:
    speed: Fastest (1165.4s total, 3.2x faster than o1-mini)
    cost: Cheapest ($2.33 per paper)
    quality: Lowest (experimental 2.6/5, report 3.0/5, usefulness 4.0/5)
    success_rate: 94.3%
    best_for: Cost-constrained research, rapid prototyping
  o1_mini:
    speed: Medium (3616.8s total)
    cost: Medium ($7.51 per paper)
    quality: Highest experimental quality (3.2/5), medium report (3.2/5), high usefulness (4.3/5)
    success_rate: 92.8%
    best_for: Experimental code quality focus
  o1_preview:
    speed: Slowest (6201.3s total, 5.3x slower than gpt-4o)
    cost: Highest ($13.10 per paper, but still 1.15x cheaper than The AI Scientist)
    quality: Best overall (experimental 2.9/5, report 3.4/5, usefulness 4.4/5)
    success_rate: 95.7%
    best_for: Highest quality research outputs, most useful results
compute_flexibility:
  description: Framework adapts to user's compute resources and budget
  options:
    - Low compute: gpt-4o backend, autonomous mode
    - Medium compute: o1-mini backend, co-pilot mode
    - High compute: o1-preview backend, co-pilot mode with multiple iterations
  allocation: Users can adjust based on CPU, GPU, memory, and inference budget
```

## Technical Workflow

```yaml
initialization_phase:
  input:
    - research_idea: Human-provided research idea or hypothesis
  process:
    - Agent Laboratory analyzes research idea
    - Prepares for three-stage research process
    - Initializes appropriate agents for each stage
literature_review_stage:
  description: First stage of research process
  process:
    - step: 1. Literature Search
      description: Search relevant scientific literature
      output: Collection of relevant papers and sources
    - step: 2. Literature Synthesis
      description: Synthesize findings from literature
      output: Literature review summary
    - step: 3. Human Feedback (Optional)
      description: User reviews and provides feedback
      impact: Allows refinement and guidance
  output: Comprehensive literature review
experimentation_stage:
  description: Second stage of research process
  process:
    - step: 1. Experiment Design
      description: Design experiments based on research objectives
      output: Experimental protocol
    - step: 2. Code Generation
      description: Generate code for experiments
      output: Executable code repository
    - step: 3. Experiment Execution
      description: Execute experiments
      output: Experimental results
    - step: 4. Human Feedback (Optional)
      description: User reviews experimental design and results
      impact: Allows refinement and correction
  output: Experimental results and code repository
report_writing_stage:
  description: Third and final stage of research process
  process:
    - step: 1. Results Synthesis
      description: Synthesize findings from all stages
      output: Integrated research findings
    - step: 2. Report Generation
      description: Generate comprehensive research report
      output: Complete research report
    - step: 3. Human Feedback (Optional)
      description: User reviews and refines final report
      impact: Ensures quality and accuracy
  output: Final research report with code references
final_outputs:
  - code_repository: Complete code repository for experiments
  - research_report: Comprehensive research report
  - traceability: All findings linked to code and literature
```

## Scientific Background

```yaml
autonomous_research_systems:
  challenge: Scientific discovery is lengthy and costly
  problem: Traditional research requires substantial time and resources
  solution: Autonomous LLM-based frameworks can automate research process
  description: Autonomous research systems aim to automate scientific discovery from conception to results
human_ai_collaboration:
  importance: Human feedback significantly improves research quality
  mechanism: Human-in-the-loop feedback at each stage
  benefit: Combines human creativity with AI automation
  description: Effective human-AI collaboration enables better research outcomes than fully autonomous systems
llm_based_research:
  approach: Use LLMs as research assistants
  advantage: Can handle literature review, code generation, and report writing
  limitation: Requires human oversight and feedback for quality
  description: LLM-based systems can automate various aspects of research process
cost_reduction:
  achievement: 84% decrease in research expenses
  comparison: Compared to previous autonomous research methods
  significance: Makes research more accessible and efficient
  description: Autonomous research systems can significantly reduce research costs
```

## Performance Metrics

```yaml
model_performance:
  best_model: o1-preview generates best research outcomes
  evaluation: Tested with various state-of-the-art LLMs
  finding: o1-preview outperforms other models
code_quality:
  achievement: Generated ML code achieves state-of-the-art performance
  comparison: Compared to existing methods
  significance: Demonstrates capability to generate high-quality research code
human_impact:
  finding: Human involvement significantly improves overall research quality
  mechanism: Feedback at each stage enables refinement
  significance: Demonstrates value of human-AI collaboration
cost_efficiency:
  reduction: 84% decrease in research expenses
  comparison: Compared to previous autonomous research methods
  significance: Makes research more accessible and cost-effective
research_outputs:
  code_repository: Complete code repository generated
  research_report: Comprehensive research report generated
  traceability: All findings linked to code and literature sources
```

## MLE-Bench Performance

Agent Laboratory's mle-solver was evaluated on 10 challenges from MLE-Bench (all low-complexity challenges focusing on text and tabular data):

```yaml
overall_performance:
  medals_earned: 4 total (2 gold, 1 silver, 1 bronze)
  above_median_human: 6 out of 10 benchmarks
  submission_rate: 100% (all challenges completed within 2 hours)
  consistency: Higher scoring consistency than other solvers
comparison_with_other_solvers:
  MLAB_gpt4o:
    medals: 0
    above_median: 0 out of 10
    note: Baseline method from MLAgentBench
  OpenHands_gpt4o:
    medals: 2 (2 gold)
    above_median: 2 out of 10
    note: CodeActAgent solver
  AIDE_o1preview:
    medals: 2 (1 gold, 1 bronze)
    above_median: 5 out of 10
    note: Solution Space Search approach
  mle_solver_Agent_Laboratory:
    medals: 4 (2 gold, 1 silver, 1 bronze)
    above_median: 6 out of 10
    note: Best overall performance
methodology:
  input_provided:
    - Kaggle dataset description
    - Distilled knowledge from Kaggle notebooks
    - Accessible train and dev set (80/20 split)
  scoring: Dev set evaluation (20% of training data)
  data_format: numpy arrays instead of file locations (to emulate data preparation phase)
  code_selection: Highest dev score evaluated on Kaggle test set
  time_limit: 2 hours per challenge
key_advantages:
  - Consistent submissions (100% vs variable for others)
  - Higher scoring across benchmarks
  - More medals earned
  - Better generalization to test sets
```

## Runtime and Cost Analysis

```yaml
comparative_analysis:
  Agent_Laboratory_gpt4o: $2.33 USD, 19.4 minutes
  Agent_Laboratory_o1mini: $7.51 USD, 60.3 minutes
  Agent_Laboratory_o1preview: $13.10 USD, 103.4 minutes
  The_AI_Scientist_gpt4o: ~$15 USD (6.4x more expensive than Agent Laboratory)
cost_breakdown_gpt4o:
  literature_review: $0.12 (92.9s)
  plan_formulation: $0.03 (23.3s)
  data_preparation: $0.09 (55.4s)
  running_experiments: $0.42 (417.8s)
  results_interpretation: $0.04 (3.5s)
  report_writing: $1.73 (572.5s)
  report_refinement: $0.00 (0.0s)
  total: $2.33 (1165.4s)
cost_breakdown_o1mini:
  literature_review: $0.16 (56.8s)
  plan_formulation: $0.04 (35.5s)
  data_preparation: $3.03 (309.7s)
  running_experiments: $1.59 (2082.5s)
  results_interpretation: $0.11 (304.6s)
  report_writing: $2.58 (827.7s)
  report_refinement: $0.00 (0.0s)
  total: $7.51 (3616.8s)
cost_breakdown_o1preview:
  literature_review: $0.29 (97.8s)
  plan_formulation: $0.04 (33.1s)
  data_preparation: $0.30 (167.9s)
  running_experiments: $2.89 (4036.2s)
  results_interpretation: $0.00 (11.9s)
  report_writing: $9.58 (1854.2s)
  report_refinement: $0.00 (0.2s)
  total: $13.10 (6201.3s)
phase_observations:
  most_expensive: Report Writing (especially with o1-preview at $9.58)
  most_time_consuming: Running Experiments (especially with o1-preview at 4036.2s)
  most_efficient: Literature Review (fast and cheap across all models)
  highest_failure_rate: Literature Review (40% failure with gpt-4o, 30% with o1-mini, 20% with o1-preview)
hardware_requirements:
  tested_on: 2023 MacBook Pro with Apple M3 Max processor, 36 GB memory
  note: No GPU required, runs on CPU
```

## Human Evaluation Results

```yaml
autonomous_mode_evaluation:
  papers_evaluated: 15 (5 research questions × 3 LLM backends)
  evaluators: 10 volunteer PhD students
  papers_per_evaluator: 3 randomly assigned
  research_questions:
    - Do language models exhibit cognitive biases?
    - Are image transformers more/less sensitive to noise than CNNs?
    - Do LMs improve accuracy on MedQA with differential diagnosis?
    - Are LMs sensitive to word order in multiple choice benchmarks?
    - Does gender role play affect LM accuracy on math questions?
  metrics:
    experimental_quality:
      gpt_4o: 2.6/5
      o1_mini: 3.2/5
      o1_preview: 2.9/5
    report_quality:
      gpt_4o: 3.0/5
      o1_mini: 3.2/5
      o1_preview: 3.4/5
    usefulness:
      gpt_4o: 4.0/5
      o1_mini: 4.3/5
      o1_preview: 4.4/5
  neurips_style_scores:
    quality:
      gpt_4o: 1.8/4
      o1_mini: 2.3/4 (best)
      o1_preview: 2.1/4
    significance: 2.2-2.5/4 (similar across models)
    clarity:
      gpt_4o: 2.6/4
      o1_mini: 2.1/4
      o1_preview: 2.5/4
    soundness:
      gpt_4o: 1.7/4
      o1_mini: 1.8/4
      o1_preview: 2.2/4 (best)
    presentation: Similar trends to soundness
    contribution: 2.1/4 average
    overall:
      gpt_4o: 3.5/10
      o1_mini: 3.8/10
      o1_preview: 4.0/10 (best)
    neurips_acceptance_threshold: 5.9/10
    gap_to_acceptance: -1.9 to -2.4 points
copilot_mode_evaluation:
  participants: Multiple researchers
  modes:
    custom_topics: Researchers chose their own research questions
    preselected_topics: Selected from 5 predefined questions
  backend: o1-mini for all phases except literature review
  tool_quality_metrics:
    utility: 3.5/5 (custom 3.75/5, preselected 3.25/5)
    continuation: 3.75/5 (custom 4.0/5, preselected 3.5/5)
    satisfaction: 3.63/5 (custom 3.75/5, preselected 3.5/5)
    usability: 4.0/5 (custom 3.75/5, preselected 4.25/5)
  paper_quality_self_evaluation:
    experimental_quality: 2.38/5
    report_quality: 3.13/5
    usefulness: 3.75/5
  neurips_style_self_evaluation:
    overall: 4.13/10 (vs 3.8/10 autonomous, +0.33)
    quality: +0.13 improvement
    clarity: +0.48 improvement
    soundness: +0.35 improvement
    presentation: +0.33 improvement
    significance: -0.3 decrease
    contribution: -0.1 decrease
  neurips_style_external_evaluation:
    overall: 4.38/10 (vs 3.8/10 autonomous, +0.58)
    quality: +0.75 improvement
    soundness: +0.48 improvement
    clarity: +0.23 improvement
    presentation: +0.33 improvement
    significance: -0.05 decrease
    contribution: +0.03 improvement
  preselected_vs_custom:
    external_evaluation_finding: Preselected topics rated slightly higher by external evaluators
    self_evaluation_finding: Custom topics rated higher by researchers themselves
    interpretation: Researchers perceive their own topics as higher quality
  feedback:
    response_rate: 75% provided optional feedback
    common_requests:
      - Improved GUI interface
      - Better inspection of intermediate results
      - More figures in paper
      - Improved literature review phase
    main_challenge: Difficulty guiding agents to execute exact vision
automated_vs_human_reviewer_discrepancy:
  automated_overall: 6.1/10
  human_overall: 3.8/10
  gap: -2.3 points
  automated_clarity: 3.6/4
  human_clarity: 2.4/4
  finding: Automated reviews significantly overestimate quality
  implication: Human feedback essential for accurate quality assessment
  note: Contrasts with Lu et al. 2024 showing high alignment on ICLR 2022 papers
```

## Limitations and Challenges

### Workflow Limitations

```yaml
self_evaluation_challenges:
  issue_1_review_quality:
    problem: LLM emulated NeurIPS reviewers may not capture true quality
    evidence: Agent Laboratory papers have lower quality figures than The AI Scientist despite higher scores
    concern: Automated reviews don't align with human judgment (-2.3 points gap)
  issue_2_llm_reliability:
    problem: LLMs show lower agreement than humans for self-evaluation
    evidence: Lu et al. 2024 showed 53.3% vs 56.1% agreement
    concern: May rely on superficial patterns rather than robust criteria
  purpose_clarification:
    note: paper-solver meant to provide readable summary, not replace human paper writing
    intended_use: Help researcher understand what was accomplished
    not_intended: Automatic paper generation for submission
automated_structure_limitations:
  fixed_paper_structure:
    constraint: Enforces standard 8-section format
    limitation: Disallows unique section organizations
    sections: Abstract, Introduction, Background, Related Work, Methods, Experimental Setup, Results, Discussion
  figure_limitations:
    constraint: Limited to 2 figures per paper
    workaround: Could incorporate all mle-solver generated figures
    future_work: Detect image files and provide paths to solver
  repository_management:
    limitation: Cannot manage repository-level code independently
    current_approach: Files provided at each step, saved by phase
    future_work: Enable flexible repository-level file modification
hallucination_issues:
  occurrence: Uncommon but present, especially in lower performing models
  model_affected: Particularly gpt-4o
  example: False claims about hyperparameters, training details not actually performed
  quoted_example: "Hyperparameter optimization played a crucial role... learning rate 0.001, batch size 32, epochs 50"
  reality: These hyperparameters were not actually used in experiments
  general_problem: LLM hallucination issue, not specific to Agent Laboratory
  mitigation_needed: Prevent misinformation propagation in automated research tools
```

### Common Failure Modes

```yaml
literature_review_failures:
  issue: Instruction-following difficulty
  behavior: Repeated SUMMARY command until max phase steps
  success_rate: 60% (gpt-4o), 70% (o1-mini), 80% (o1-preview)
  impact: Highest failure rate among all phases
token_limit_issues:
  retrieved_papers: Sometimes exceed token limit
  printed_output: Data preparation or experiment results can exceed limits
  impact: Process termination or truncation
code_quality_issues:
  zero_accuracy: Experiments sometimes obtain 0% accuracy
  persistence: Not corrected by agent before solving steps exhausted
  line_0_bias: Tendency to edit line 0 more than other lines
  impact: REPLACE command more successful than targeted EDIT
dangerous_commands:
  exit_command: mle-solver generates exit() which terminates entire process
  mitigation: Manual detection and removal required
  subprocess_run: System commands via subprocess.run() observed
  risk: Potential security concern
  safeguard_needed: Implement restrictions around system commands
arxiv_search_issues:
  problem: paper-solver struggles with relevant paper search
  behavior: Could take up to 100 tries before successful search
  mitigation: 5 try limit enforced to prevent cycles
  impact: Reduced literature integration quality
```

### Ethical Considerations

```yaml
research_quality_concerns:
  risk: Lower barriers to producing substandard or misleading outputs
  impact: Could overwhelm peer review systems
  threat: Jeopardize integrity of academic discourse
  mitigation_needed: Transparent disclosure of AI involvement
bias_amplification:
  risk: Reflect or amplify biases in datasets or algorithms
  impact: Skewed research findings
  mitigation: Transparent disclosure, bias checking
misuse_potential:
  cybersecurity_risk: Automated malware creation
  environmental_risk: Biased analyses downplaying climate risks
  general_concern: Bypassing ethical oversight
  safeguards_needed: Alignment with ethical research standards
governance:
  requirement: Robust governance mechanisms
  goal: Ensure LLM outputs align with ethical principles and societal values
  importance: Increases as platform matures
disclosure:
  importance: Critical for maintaining accountability
  requirement: Transparent disclosure of AI involvement in research outputs
```

## Lessons Learned

### Achievements

- Successfully developed autonomous framework for complete research process from conception to results
- Demonstrated that o1-preview generates best research outcomes among tested LLMs (4.4/5 usefulness, 4.0/10 NeurIPS score)
- o1-mini achieved highest experimental quality (3.2/5) demonstrating technical soundness
- Generated machine learning code achieves state-of-the-art performance on MLE-Bench (4 medals vs 0-2 for competitors)
- Achieved 84% cost reduction compared to previous autonomous research methods ($2.33 vs ~$15 with gpt-4o)
- Enabled human feedback integration at each research stage significantly improving quality (+0.58 overall improvement)
- Produced comprehensive research outputs including code repository and research report in under 2 hours
- Demonstrated feasibility of both autonomous and co-pilot modes for different use cases
- Achieved 100% submission rate on MLE-Bench challenges (vs variable for other solvers)
- Co-pilot mode rated highly for utility (3.5/5), continuation likelihood (3.75/5), and usability (4.0/5)
- Compute-flexible architecture adapts to user resources and budget constraints

### Implications

- Autonomous research systems can significantly accelerate scientific discovery while reducing costs
- Human-AI collaboration improves research quality compared to fully autonomous systems (+0.58 overall score improvement)
- LLM-based frameworks can handle complex research tasks including literature review, experimentation, and report writing
- Cost reduction makes research more accessible to broader scientific community (from $15 to $2.33)
- Framework enables researchers to allocate more effort toward creative ideation rather than low-level coding and writing
- Opens new possibilities for accelerating scientific progress through AI automation
- Different LLM backends offer trade-offs: gpt-4o for cost, o1-mini for experimental quality, o1-preview for overall usefulness
- Automated reviews significantly overestimate quality, demonstrating importance of human evaluation
- Co-pilot mode with human feedback essential for quality research, especially for significance and contribution
- Multi-agent collaboration with specialized roles effective for complex workflows

### Challenges

**Model Selection and Performance:**
- Requires appropriate LLM model selection based on priorities (cost vs quality vs speed)
- o1-preview performs best overall but costs 5.6x more than gpt-4o
- Success rates vary by phase (literature review 60-80%, other phases 80-100%)
- Automated reviews overestimate quality by 2.3 points compared to human reviews

**Quality and Validation:**
- Human feedback essential for ensuring research quality, especially significance and contribution
- Generated papers score below NeurIPS acceptance threshold (3.8-4.38 vs 5.9 required)
- System performance depends on quality of initial research idea and guidance
- Need to balance automation with human oversight
- Validation of generated code and research findings is essential
- Hallucination issues especially with lower performing models (gpt-4o)
- 0% accuracy bugs sometimes not corrected by agents

**Technical Limitations:**
- Literature review phase has highest failure rate (20-40% depending on model)
- Token limits can be reached with long papers or printed output
- Repository-level code management not yet supported
- Limited to 2 figures per paper
- Fixed 8-section paper structure
- arXiv search in paper-solver can struggle (up to 100 tries needed)

**Usability Challenges:**
- Difficulty guiding agents to execute exact research vision in co-pilot mode
- Need for better GUI and intermediate result inspection
- Instruction-following issues especially in literature review
- Security concerns with subprocess.run() system commands

**Ethical Concerns:**
- Risk of overwhelming peer review systems with substandard outputs
- Potential bias amplification in research findings
- Misuse potential (malware, biased analyses, bypassing ethics)
- Need for transparent disclosure of AI involvement
- Requires robust governance mechanisms

### Impact on Field

Agent Laboratory demonstrates the feasibility of autonomous LLM-based research frameworks that can complete the entire research process from conception to results in under 2 hours at significantly reduced cost ($2.33 vs $15). The 84% cost reduction, state-of-the-art code performance on MLE-Bench, and the ability to integrate human feedback at each stage opens new pathways for accelerating scientific discovery. 

The framework enables researchers to focus on creative ideation while automating routine tasks of literature review, coding, and report writing, potentially transforming how scientific research is conducted. The co-pilot mode demonstrates that human-AI collaboration produces higher quality research than fully autonomous systems, with external evaluators rating co-pilot papers 0.58 points higher than autonomous papers.

However, the significant gap between automated reviews (6.1/10) and human reviews (3.8/10) demonstrates that human evaluation remains essential for accurate quality assessment. Papers generated by Agent Laboratory still fall short of conference acceptance thresholds (3.8-4.38 vs 5.9 for NeurIPS), particularly in significance and contribution metrics, indicating that while the tool accelerates the research process, human refinement and creative input remain crucial for producing conference-quality research.

Agent Laboratory represents a step toward human-centered research workflows that leverage LLMs as assistants rather than replacements, enabling researchers to explore more ideas simultaneously and investigate concepts that might otherwise remain unexplored due to resource constraints.

## Organizations

### Research Collaboration
**Role in Project**: primary  
**Role Description**: Multi-institutional research collaboration  
**Contribution**: Development of Agent Laboratory framework through collaborative research effort involving multiple institutions and researchers  
**Organization Type**: research_center  
**Status**: active  
**Description**: Multi-institutional research collaboration for developing autonomous AI research systems

## Key People

### Samuel Schmidgall
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: First Author, Corresponding Author  
**Affiliations**: AMD, Johns Hopkins University  
**Email**: sschmi46@jhu.edu  
**Contribution**: Lead development of Agent Laboratory framework, overall system design, methodology, experimental design, paper writing  
**Expertise**: AI research, LLM systems, autonomous research systems, multi-agent frameworks  
**Biography**: Researcher at AMD and PhD student at Johns Hopkins University, leading the Agent Laboratory project

### Yusheng Su
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, system implementation, experimental evaluation  
**Expertise**: AI research, LLM systems, autonomous agents  
**Biography**: Researcher at AMD working on autonomous research systems

### Ze Wang
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, agent design, code implementation  
**Expertise**: AI research, machine learning, software engineering  
**Biography**: Researcher at AMD contributing to Agent Laboratory development

### Ximeng Sun
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, experimental design  
**Expertise**: AI research, autonomous systems, experimental methodology  
**Biography**: Researcher at AMD working on autonomous research agents

### Jialian Wu
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, research automation components  
**Expertise**: AI research, research automation, workflow optimization  
**Biography**: Researcher at AMD specializing in research automation

### Xiaodong Yu
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, LLM integration  
**Expertise**: AI research, LLM applications, natural language processing  
**Biography**: Researcher at AMD working on LLM-based applications

### Jiang Liu
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, system architecture  
**Expertise**: AI research, autonomous systems, system design  
**Biography**: Researcher at AMD contributing to system architecture

### Michael Moor
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: ETH Zurich  
**Contribution**: Development of Agent Laboratory framework, academic collaboration, methodology validation  
**Expertise**: AI research, machine learning, AI for scientific discovery  
**Biography**: Researcher at ETH Zurich providing international academic collaboration on AI for science

### Zicheng Liu
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, technical implementation  
**Expertise**: AI research, computer vision, autonomous systems, deep learning  
**Biography**: Researcher at AMD with expertise in computer vision and AI systems

### Emad Barsoum
**Title**: Researcher  
**Participation Type**: researcher  
**Role in Project**: Co-author  
**Affiliations**: AMD  
**Contribution**: Development of Agent Laboratory framework, project oversight  
**Expertise**: AI research, autonomous research systems, machine learning applications  
**Biography**: Researcher at AMD working on autonomous AI systems

## Products

### Agent Laboratory Framework
**Type**: platform  
**Status**: published  
**Development Stage**: Research / Preclinical  
**Role in Project**: primary  
**Description**: Autonomous LLM-based framework for complete research process automation. The system accepts human-provided research ideas and progresses through three stages (literature review, experimentation, and report writing) to produce comprehensive research outputs.  
**Capabilities**:
- Autonomous literature review and synthesis
- Automated experiment design and execution
- Research report generation with code references
- Human feedback integration at each stage
- Support for multiple LLM models (best performance with o1-preview)
- Code repository generation
- Complete research workflow automation

**Technical Details**:
```yaml
ai_methods: LLM-based multi-agent system
architecture: Three-stage pipeline (literature review, experimentation, report writing)
llm_models: Tested with various state-of-the-art LLMs, o1-preview performs best
performance_metrics:
  cost_reduction: 84% decrease compared to previous autonomous methods
  code_quality: State-of-the-art performance
  human_impact: Significant quality improvement with human feedback
workflow:
  - Literature Review Stage
  - Experimentation Stage
  - Report Writing Stage
  - Human feedback integration at each stage
outputs:
  - Code repository
  - Research report
  - Complete traceability to code and literature
```

## Links

### [Agent Laboratory: Using LLM Agents as Research Assistants](https://arxiv.org/abs/2501.04227)
**Type**: research_publication  
**Relevance**: primary  
**Category**: publication  
**Description**: Main arXiv preprint describing the Agent Laboratory framework, methodology, architecture, and evaluation results  
**Publisher**: arXiv  
**Publication Date**: 2025-01-08 (v1), 2025-06-17 (v2)  
**Authors**: Samuel Schmidgall, Yusheng Su, Ze Wang, Ximeng Sun, Jialian Wu, Xiaodong Yu, Jiang Liu, Michael Moor, Zicheng Liu, Emad Barsoum  
**Metadata**:
```yaml
type: arXiv Preprint
venue: arXiv
arxiv_id: 2501.04227
doi: 10.48550/arXiv.2501.04227
version: v2 (revised 2025-06-17)
subjects: Human-Computer Interaction (cs.HC), Artificial Intelligence (cs.AI), Computation and Language (cs.CL), Machine Learning (cs.LG)
```

## Events

### Agent Laboratory arXiv Publication (v1)
**Date**: 2025-01-08  
**Type**: publication  
**Description**: Initial publication of Agent Laboratory paper on arXiv (v1)  
**Details**:
```yaml
type: arXiv Preprint
venue: arXiv
arxiv_id: 2501.04227
version: v1
significance: First comprehensive documentation of the Agent Laboratory framework
```

### Agent Laboratory Paper Revision (v2)
**Date**: 2025-06-17  
**Type**: publication  
**Description**: Revised version (v2) of Agent Laboratory paper published on arXiv  
**Details**:
```yaml
type: arXiv Preprint
venue: arXiv
arxiv_id: 2501.04227
version: v2
significance: Updated version with revisions and improvements
```

