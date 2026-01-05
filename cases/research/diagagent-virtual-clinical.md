---
id: diagagent-virtual-clinical
slug: diagagent-virtual-clinical
entity_type: research
status: published
data_completeness: exceptional
last_researched: 2025-01-05
research_category: collaboration
researcher: AI Assistant
version: 2.0
name: DiagAgent - Evolving Diagnostic Agents in Virtual Clinical Environment
description: "DiagAgent is a reinforcement learning framework for training large language models (LLMs) as diagnostic agents, developed through collaboration between Shanghai Jiao Tong University, Fudan University, and other institutions (published October 2025). Unlike instruction-tuned models trained on static case summaries, DiagAgent acquires diagnostic strategies through interactive exploration and outcome-based feedback in a virtual clinical environment. The framework consists of three core components: (1) DiagGym - a diagnostics world model trained with electronic health records (EHR) that emits examination outcomes conditioned on patient history and recommended examinations, serving as a virtual clinical environment; (2) DiagAgent - an RL-trained agent that learns diagnostic policies through end-to-end, multi-turn reinforcement learning to optimize both information yield and diagnostic accuracy; (3) DiagBench - a diagnostic benchmark comprising 750 cases with physician-validated examination recommendations and 99 cases annotated with 973 physician-written rubrics. DiagAgent significantly outperforms 10 state-of-the-art LLMs including DeepSeek-v3, GPT-4o, and Claude-sonnet-4. In single-turn settings, it achieves 9.34% higher diagnostic accuracy and 44.03% improvement in examination recommendation hit ratio. In end-to-end settings, it delivers 15.12% increase in diagnostic accuracy and 23.09% boost in examination recommendation F1 score. In rubric-based evaluation, it surpasses Claude-sonnet-4 by 7.1% in weighted rubric score, demonstrating that learning policies in interactive clinical environments confers dynamic and clinically meaningful diagnostic management abilities unattainable through passive training alone."
mission: To develop reinforcement learning-based diagnostic agents that can manage multi-turn diagnostic processes, adaptively select examinations, and commit to accurate final diagnoses through interactive learning in virtual clinical environments, advancing AI-assisted clinical decision support.
entity_data:
  name: DiagAgent Framework
  status: published
  objectives:
    - Develop DiagGym as a diagnostics world model trained on EHR data for realistic clinical simulation
    - Train DiagAgent via multi-turn reinforcement learning to optimize diagnostic policies
    - Create DiagBench benchmark with physician-validated cases and rubrics
    - Demonstrate superior performance over state-of-the-art LLMs in diagnostic tasks
    - Enable dynamic diagnostic management through interactive exploration vs passive training
    - Provide framework for training clinically meaningful diagnostic agents
  start_date: 2024-10-01
  publication_date: 2025-10-28
  description: "Reinforcement learning framework for training LLMs as diagnostic agents in virtual clinical environment. Three-component architecture: (1) DiagGym - world model trained on 114,239 EHRs from MIMIC-IV spanning 4,897 distinct diseases, achieving 96.91% full-chain consistency and 0.128 Wasserstein distance for numerical examinations; (2) DiagAgent - RL-trained agent (Qwen2.5-7B/14B, Llama3.1-8B base models) using GRPO algorithm with multi-objective reward function (diagnosis accuracy + examination quality + turn efficiency), trained on 15,324 interactive diagnostic trajectories; (3) DiagBench - 750 physician-validated cases + 99 cases with 973 detailed physician-written rubrics for process evaluation. Training dataset: 118,478 restructured EHRs (114,239 training, 4,239 test). Achieves superior performance: single-turn (+9.34% diagnostic accuracy, +44.03% examination hit ratio), end-to-end (+15.12% accuracy, +23.09% examination F1), rubric-based (+7.1% weighted score vs Claude-sonnet-4). Outperforms 10 SOTA LLMs (GPT-4o, Claude-4-sonnet, DeepSeek-v3-671B, Qwen2.5-72B, Qwen3-235B, Llama3.3-70B, GPT-OSS-120B, OpenBioLLM-70B, Baichuan-M1-14B, MedGemma-27B) and 2 agentic systems (MedAgents, MDAgents)."
  methodology: "Interactive reinforcement learning approach with detailed implementation: (1) DiagGym Data Construction - 331,794 MIMIC-IV discharge notes processed, filtered for physical examinations and diagnostic relevance, mapped to 118,171,368 lab events, 3,228,714 microbiology events, 66,542,177 radiology reports. Final dataset: 114,239 training EHRs (avg 29 examinations per case: 26 lab, 2 microbiology, 1 radiology) spanning 4,897 diseases. Model: Qwen2.5-Instruct-7B fine-tuned with auto-regressive generation loss, trained 15 epochs on 8x A100 GPUs (learning rate 4×10⁻⁵, max length 8192 tokens, DeepSpeed ZeRO Stage 2). Evaluation on 863 test cases (863 distinct diseases). (2) DiagAgent Data Construction - 41,245 cases reformatted using DeepSeek-v3 to generate: initial inquiry (without diagnosis), referenced multi-turn diagnostic trajectory (examination recommendations with rationale), and final diagnosis. Two-stage quality filtering resulted in 15,324 interactive diagnostic trajectories for training. (3) Cold-start Phase - 1,000 high-quality cases used for supervised fine-tuning with auto-regressive loss over assistant tokens, initializing proper output format before RL. (4) GRPO Reinforcement Learning - Multi-objective reward function: R = λ₁r_diag + λ₂r_exam + λ₃r_turn where r_diag evaluates diagnosis accuracy (binary, judged by Qwen2.5-72B), r_exam measures examination recommendation quality (F1 score against reference), r_turn penalizes excessive dialogue turns (max 12 turns). Weights: λ₁=1.0, λ₂=0.5, λ₃=1.0. Training: 4 nodes × 8 A100 GPUs per node, batch size 512, max response 8192 tokens, learning rate 1×10⁻⁶, 5 rollouts per sample, 200 training steps. DiagGym deployed on 2 nodes via vLLM for interactive training. (5) Model Variants - Three base models trained: Qwen2.5-Instruct-7B, Qwen2.5-Instruct-14B, Llama3.1-Instruct-8B. All share identical training pipeline."
  results: "DiagGym Evaluation (863 test cases, 863 diseases): Instance-wise metrics with automated evaluator - Step-level similarity 3.565/5 (vs DeepSeek-v3 2.576, Qwen2.5-72B 2.495), Full-chain consistency 96.91% (vs DeepSeek-v3 88.81%, Qwen2.5-72B 92.39%). Instance-wise with physician raters (100 cases, 3 physicians): Similarity 4.49/5 (vs DeepSeek-v3 4.09, Qwen2.5-72B 3.97), Majority-vote consistency 95.00% (vs DeepSeek-v3 54.00%, Qwen2.5-72B 44.00%). Examination-wise numerical: Wasserstein Distance 0.128 (vs GT baseline, DeepSeek-v3 1.336), Normalized Variance 3.46 (GT 5.31, DeepSeek-v3 24.56). Examination-wise free-text: FID 0.747 (vs DeepSeek-v3 4.158), LPIPS 0.378 (GT 0.427). Computational efficiency: 1 GPU, 0.52s per generation (vs DeepSeek-v3: 16 GPUs, 62.72s). DiagAgent Single-Turn Evaluation (750 cases, 4,485 turns: 3,735 examination + 750 diagnosis): DiagAgent-14B achieves Hit Ratio 68.49% and Accuracy 87.87% (vs best baseline MedGemma-27B: 28.57%/60.53%, Claude-4-sonnet: 31.63%/74.31%, DeepSeek-v3: 20.08%/72.27%). DiagAgent-7B: 72.56%/85.60%. DiagAgent-8B: 56.57%/82.27%. Agentic systems underperform: MDAgents 20.24%/73.47%, MedAgents 19.31%/70.27%. End-to-End Evaluation (750 cases): DiagAgent-14B - Avg Turns 6.66, Precision 42.12%, Recall 52.12%, F1 46.59%, Accuracy 61.27% (vs best baseline Claude-4-sonnet: 3.91 turns, 33.06%/23.41%/27.41%/46.14%; DeepSeek-v3: 2.49 turns, 36.49%/13.58%/19.80%/47.08%). DiagAgent-7B: 5.45 turns, 46.14%/46.33%/46.23%/60.78%. MDAgents: 2.40 turns, 34.04%/12.56%/18.35%/44.96%. Rubric-Based Evaluation (99 cases, 973 physician-written rubrics): DiagAgent-14B weighted rubric score 32.86% (vs Claude-sonnet-4 25.39%, Qwen3-235B 24.49%, MDAgents 21.64%, DeepSeek-v3 19.07%). Ablation Studies: RL significantly outperforms SFT - Qwen2.5-7B: 60.78% vs 44.40% (SFT), Qwen2.5-14B: 61.27% vs 45.98% (SFT), Llama3.1-8B: 53.45% vs 45.35% (SFT). Dual-reward (diagnosis + examination) crucial: Qwen2.5-7B F1 improves from 32.76% (diagnosis-only) to 46.23% (dual-reward)."
  collaboration_period:
    start: 2024-10
    publication_date: 2025-10-28
  author_contributions:
    primary_authors:
      - Pengcheng Qiu
      - Chaoyi Wu
      - Junwei Liu
    co_authors:
      - Qiaoyu Zheng
      - Yusheng Liao
      - Haowen Wang
      - Yun Yue
      - Qiaoyu Fan
      - Shuai Zhen
      - Jian Wang
      - Jinjie Gu
    corresponding_authors:
      - Yanfeng Wang
      - Ya Zhang
      - Weidi Xie
  supplementary_data:
    arxiv_id: "2510.24654"
    github_repository: "https://github.com/MAGIC-AI4Med/DiagGym"
    data_availability: "DiagBench benchmark comprising 750 cases with physician-validated examination recommendations and 99 cases with 973 physician-written rubrics on diagnosis process. Source data: MIMIC-IV electronic health records. Due to licensing restrictions, data cannot be directly open-sourced but communication ongoing for potential release on PhysioNet.org."
    code_availability: "All source codes released on GitHub at https://github.com/MAGIC-AI4Med/DiagGym"
taxonomy:
  geography: China
  ai_technology:
    - LLMs
    - Reinforcement Learning
  ai_approach:
    - Reinforcement Learning
    - Supervised Learning
  ai_architecture:
    - LLMs
    - Transformers
  ai_specialization:
    - Multi-Agent AI
  primary_focus:
    - Diagnostics & Preventive Health
    - Autonomous AI Scientists
  aging_approach:
    - Diagnostics/Age Assessment
  target_biology:
    - General Aging/Longevity
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality: []

organizations:
  - name: Shanghai Jiao Tong University
    role: primary
    org_type: institution
    status: active
    role_description: Primary research institution for DiagAgent development
    contribution_description: "Shanghai Jiao Tong University served as the primary institution for developing the DiagAgent framework. Multiple co-authors including Pengcheng Qiu, Chaoyi Wu, Qiaoyu Zheng, Yusheng Liao, Yanfeng Wang, Ya Zhang, and Weidi Xie are affiliated with SJTU. The university contributed to the theoretical foundation, technical implementation, model training infrastructure, and comprehensive validation of the reinforcement learning approach for diagnostic agents."
    description: Leading comprehensive research university in Shanghai, China with strong programs in artificial intelligence, computer science, and medical informatics
    focus: AI research, computer science, medical AI, reinforcement learning
    website: "https://www.sjtu.edu.cn"
  - name: Shanghai Artificial Intelligence Laboratory
    role: primary
    org_type: research_center
    status: active
    role_description: Co-primary research institution providing AI research infrastructure
    contribution_description: "Shanghai AI Laboratory served as a co-primary institution alongside SJTU. Multiple co-authors (Pengcheng Qiu, Chaoyi Wu, Qiaoyu Zheng, Yusheng Liao, Yanfeng Wang, Ya Zhang, Weidi Xie) hold dual affiliation with Shanghai AI Lab. The laboratory provided advanced AI research infrastructure, computational resources, and expertise in large language models and reinforcement learning that were critical for the DiagAgent framework development."
    description: Leading AI research institution in Shanghai focused on advancing artificial intelligence research and applications
    focus: Large language models, reinforcement learning, AI for healthcare, medical AI
  - name: AntGroup Intelligence Healthcare Department
    role: partner
    org_type: company
    status: operational
    role_description: Industrial partner providing healthcare AI expertise and resources
    contribution_description: "AntGroup's Intelligence Healthcare Department contributed significant industry expertise and resources to the project. Six co-authors (Junwei Liu, Haowen Wang, Yun Yue, Qianrui Fan, Shuai Zhen, Jian Wang, Jinjie Gu) from AntGroup participated in the research, bringing practical healthcare AI implementation experience and contributing to the development of DiagGym world model and validation methodologies."
    description: Healthcare AI division of AntGroup (formerly Ant Financial), a major Chinese fintech company, focusing on AI-driven healthcare solutions
    focus: Healthcare AI, medical informatics, clinical decision support systems
    location:
      city: Hangzhou
      country: China
  - name: Peking University Intelligence Computing and Sensing Laboratory
    role: collaborator
    org_type: lab
    status: active
    parent_organization_id: peking-university
    role_description: Collaborating research laboratory
    contribution_description: "Intelligence Computing and Sensing Laboratory at Peking University contributed through co-author Junwei Liu, providing expertise in intelligent computing and sensing technologies applicable to medical diagnosis scenarios."
    description: Research laboratory at Peking University focused on intelligent computing, sensing technologies, and AI applications
    focus: Intelligent computing, sensing technologies, AI algorithms
    location:
      city: Beijing
      country: China

products:
  - name: DiagGym
    type: ai_model
    status: published
    development_stage: Research / Preclinical
    description: "Diagnostics world model trained with electronic health records (EHR) that emits examination outcomes conditioned on patient history and recommended examination. Serves as a virtual clinical environment for realistic diagnosis training and evaluation."
    capabilities:
      - Simulate examination outcomes based on patient history
      - Generate realistic clinical scenarios for agent training
      - Provide interactive environment for multi-turn diagnostic processes
      - Model conditional relationships between patient state and examination results
      - Enable scalable training of diagnostic agents without real patient data
    applications:
      - Training environment for diagnostic AI agents
      - Evaluation framework for clinical decision-making models
      - Simulation platform for medical education and training
      - Testing ground for diagnostic strategies and policies
    technical_details:
      ai_methods: "World modeling, conditional outcome generation"
      architecture: "EHR-trained world model that conditions examination outcomes on patient history and examination type"
      training_data: "Electronic health records (EHR) data"
      performance_metrics: "Realistic simulation of clinical examination outcomes"
      validation: "Physician validation of simulated examination outcomes and clinical realism"
  - name: DiagAgent
    type: ai_model
    status: published
    development_stage: Research / Preclinical
    description: "Reinforcement learning-trained diagnostic agent that learns diagnostic policies through end-to-end, multi-turn reinforcement learning to optimize both information yield and diagnostic accuracy. Manages complete diagnostic workflows including examination selection and final diagnosis."
    capabilities:
      - Manage multi-turn diagnostic processes
      - Adaptively select examinations based on patient history
      - Optimize information yield from examination requests
      - Balance exploration of examination space with diagnostic efficiency
      - Commit to accurate final diagnoses
      - Learn diagnostic strategies through interactive exploration
    applications:
      - Clinical decision support for diagnostic workflows
      - Automated diagnostic assistance
      - Medical training and education tool
      - Diagnostic strategy optimization
    technical_details:
      ai_methods: "Multi-turn reinforcement learning, policy optimization, interactive exploration"
      architecture: "RL agent with diagnostic policy network trained end-to-end"
      training_data: "DiagGym virtual environment interactions"
      performance_metrics: "Single-turn: +9.34% diagnostic accuracy, +44.03% examination hit ratio. End-to-end: +15.12% diagnostic accuracy, +23.09% examination F1. Rubric-based: +7.1% weighted score vs Claude-sonnet-4"
      validation: "Comparison with 10 SOTA LLMs (GPT-4o, DeepSeek-v3, Claude-sonnet-4, etc.), 2 prompt-engineered agents, and physician-validated rubrics across 99 cases with 973 annotations"
  - name: DiagBench
    type: platform
    status: published
    development_stage: Research / Preclinical
    description: "Diagnostic benchmark comprising 750 cases with physician-validated examination recommendations and 99 cases annotated with 973 physician-written rubrics on diagnosis process. Provides standardized evaluation framework for diagnostic AI systems."
    capabilities:
      - Standardized evaluation of diagnostic agents
      - Physician-validated ground truth for examination recommendations
      - Detailed rubric-based assessment of diagnostic processes
      - Multi-dimensional evaluation across diagnostic scenarios
      - Benchmarking framework for comparing diagnostic AI systems
    applications:
      - Evaluation of diagnostic AI models
      - Benchmarking clinical decision support systems
      - Validation of diagnostic strategies
      - Assessment of examination recommendation quality
    components:
      - name: Case Dataset
        description: "750 cases with physician-validated examination recommendations"
        technical_details: "Comprehensive coverage of diagnostic scenarios with expert-validated ground truth"
      - name: Rubric Annotations
        description: "99 cases with 973 physician-written rubrics on diagnosis process"
        technical_details: "Detailed process-level annotations capturing clinical reasoning and decision-making quality"
    technical_details:
      validation: "All examination recommendations and rubrics validated by practicing physicians"
      coverage: "Diverse diagnostic scenarios spanning multiple medical specialties and complexity levels"

people:
  - name: Pengcheng Qiu
    person_type: researcher
    role: First Author
    affiliations:
      - Shanghai Jiao Tong University
    contribution_description: Primary researcher and first author of the DiagAgent framework
  - name: Chaoyi Wu
    person_type: researcher
    role: Co-author
    contribution_description: Core contributor to DiagAgent development
  - name: Junwei Liu
    person_type: researcher
    role: Co-author
    contribution_description: Core contributor to DiagAgent development
  - name: Qiaoyu Zheng
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Yusheng Liao
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Haowen Wang
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Yun Yue
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Qiaoyu Fan
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Shuai Zhen
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Jian Wang
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Jinjie Gu
    person_type: researcher
    role: Co-author
    contribution_description: Contributor to research and development
  - name: Yanfeng Wang
    person_type: researcher
    role: Corresponding Author
    contribution_description: Corresponding author and senior contributor to research direction
  - name: Ya Zhang
    person_type: researcher
    role: Corresponding Author
    contribution_description: Corresponding author and senior contributor to research direction
  - name: Weidi Xie
    person_type: researcher
    role: Corresponding Author
    contribution_description: Corresponding author and senior contributor to research direction

links:
  - url: "https://arxiv.org/abs/2510.24654"
    type: research_publication
    title: "Evolving Diagnostic Agents in a Virtual Clinical Environment"
    description: "arXiv preprint of the DiagAgent research paper"
    authors:
      - Pengcheng Qiu
      - Chaoyi Wu
      - Junwei Liu
      - Qiaoyu Zheng
      - Yusheng Liao
      - Haowen Wang
      - Yun Yue
      - Qiaoyu Fan
      - Shuai Zhen
      - Jian Wang
      - Jinjie Gu
      - Yanfeng Wang
      - Ya Zhang
      - Weidi Xie
    publication_date: 2025-10-28
    metadata:
      arxiv_id: "2510.24654"
      journal: "arXiv preprint"
    relevance: primary
    category: source
  - url: "https://arxiv.org/pdf/2510.24654"
    type: research_publication
    title: "DiagAgent Paper PDF"
    description: "PDF version of the DiagAgent research paper"
    relevance: primary
    category: source
  - url: "https://arxiv.org/html/2510.24654"
    type: research_publication
    title: "DiagAgent Paper HTML (Experimental)"
    description: "HTML version of the DiagAgent research paper"
    relevance: secondary
    category: source
  - url: "https://doi.org/10.48550/arXiv.2510.24654"
    type: reference
    title: "DOI for DiagAgent Paper"
    description: "Digital Object Identifier for the DiagAgent publication"
    metadata:
      doi: "10.48550/arXiv.2510.24654"
    relevance: primary
    category: reference
  - url: "https://github.com/MAGIC-AI4Med/DiagGym"
    type: github
    title: "DiagGym GitHub Repository"
    description: "Official open-source code repository for DiagAgent framework including DiagGym world model, DiagAgent training pipeline, and evaluation scripts"
    relevance: primary
    category: source

events:
  - event_date: 2025-10-28
    event_type: publication
    title: DiagAgent Paper Publication
    description: Publication of "Evolving Diagnostic Agents in a Virtual Clinical Environment" on arXiv
    details:
      location: arXiv preprint server
      outcomes: "First demonstration of RL-trained diagnostic agents outperforming GPT-4o and Claude-sonnet-4 in clinical diagnostic tasks"
---

## Executive Summary

DiagAgent represents a paradigm shift in training diagnostic AI systems, moving from passive learning on static case summaries to active learning through interactive exploration in virtual clinical environments. Published in October 2025, this collaborative research project introduces a three-component framework that achieves state-of-the-art performance in clinical diagnostic tasks.

The framework's core innovation lies in **DiagGym**, a world model trained on electronic health records that creates a realistic virtual clinical environment. Unlike traditional supervised learning approaches, DiagAgent learns diagnostic policies through reinforcement learning, managing complete multi-turn diagnostic workflows including adaptive examination selection and final diagnosis commitment. This interactive learning approach enables the agent to develop dynamic diagnostic strategies that significantly outperform existing large language models.

Validated against **DiagBench** (750 physician-validated cases + 99 cases with 973 expert rubrics), DiagAgent demonstrates substantial improvements: 9.34% higher diagnostic accuracy in single-turn settings, 15.12% increase in end-to-end diagnostic accuracy, and 7.1% improvement over Claude-sonnet-4 in rubric-based evaluation. These results, validated by practicing physicians, demonstrate that interactive learning confers clinically meaningful diagnostic management abilities unattainable through passive training alone.

## Technical Details

```yaml
system_architecture:
  overview: "Three-component framework for training diagnostic agents via reinforcement learning in virtual clinical environment. Complete end-to-end pipeline from EHR data construction to RL-trained agent deployment."
  
  diaggym_world_model:
    description: "Conditional textual EHR generator that simulates examination results based on patient state"
    base_model: "Qwen2.5-Instruct-7B"
    training_objective: "Auto-regressive text generation minimizing negative log-likelihood of ground-truth examination results"
    loss_function: "L_sim = -∑(t=0 to T-1) log Φ_env(ê_(t+1) | a_(t+1), E_t, B)"
    input_format:
      patient_profile_B: "Chief complaint, present medical history, past medical history, social history, allergies, family history, final diagnosis"
      examination_history_E_t: "Sequence of past examinations {(a1,e1), (a2,e2), ..., (at,et)} where a=exam name, e=result"
      examination_query_a: "Next examination to simulate (e.g., 'Complete Blood Count', 'CT Abdomen')"
    output_format: "Free text examination results (numerical values embedded as text or narrative reports)"
    training_data_construction:
      source: "MIMIC-IV v2.2 database"
      discharge_notes: "331,794 notes processed"
      lab_events: "118,171,368 records"
      microbiology_events: "3,228,714 records"
      radiology_reports: "66,542,177 reports"
      filtering_criteria:
        - "Physical examination records present"
        - "Final diagnosis not in past/current medical history (using DeepSeek-v3 validation)"
        - "One-day window for pre-admission examinations"
      final_dataset: "114,239 training cases + 4,239 test cases = 118,478 total"
      disease_coverage: "4,897 distinct diseases in training set"
      examination_statistics_per_case:
        average_total: "29 examinations"
        lab_tests: "26 (average)"
        microbiology: "2 (average)"
        radiology: "1 (average)"
    training_implementation:
      framework: "Hugging Face Transformers with DeepSpeed ZeRO Stage 2"
      hardware: "8x NVIDIA A100-80GB GPUs"
      epochs: 15
      learning_rate: "4×10⁻⁵"
      max_sequence_length: "8,192 tokens"
      convergence: "Achieved within 15 epochs"
    inference_efficiency:
      minimal_gpus: "1x A100-80GB"
      generation_time: "0.52 seconds per examination result"
      deployment: "vLLM for high-throughput serving during RL training"
    
  diagagent_rl_agent:
    description: "Multi-turn diagnostic agent trained via GRPO reinforcement learning"
    base_models:
      - "Qwen2.5-Instruct-7B"
      - "Qwen2.5-Instruct-14B"
      - "Llama3.1-Instruct-8B"
    state_definition: "s_t = (I, E_t) where I=initial inquiry (without diagnosis), E_t=examination history"
    action_space: "A = {a1, a2, ..., aN, final_diagnosis} - all clinical examinations + diagnosis action"
    policy_function: "π_θ(a|s_t) = Φ_diag(s_t) - maps state to action distribution"
    training_data_construction:
      source_cases: "41,245 randomly sampled from DiagGym training set"
      llm_reformatter: "DeepSeek-v3 with structured prompts"
      generated_components:
        initial_inquiry: "Patient history without diagnosis (refined for realistic format)"
        diagnostic_trajectory: "Multi-turn sequence with current diagnosis → examination query + rationale → results"
        final_diagnosis: "Single primary condition focus"
      quality_filtering:
        stage_1: "Two-stage filtering with DeepSeek-v3"
        stage_2: "Check diagnosis leakage into initial inquiry"
        final_dataset: "15,324 interactive diagnostic trajectories"
      dialogue_format: "Alternating assistant (diagnosis + examination query) and user (results) messages"
    training_phases:
      cold_start:
        description: "Supervised fine-tuning for format initialization"
        dataset: "1,000 manually selected high-quality cases"
        loss: "L_cold = -∑ log Φ_diag(yi | y_≤i-1) over assistant tokens only"
        framework: "Transformers + DeepSpeed ZeRO Stage 2"
        hardware: "8x A100 GPUs"
        hyperparameters:
          max_length: "8,192 tokens"
          learning_rate: "1×10⁻⁵"
          epochs: 3
      reinforcement_learning:
        algorithm: "GRPO (Group Relative Policy Optimization)"
        reward_function: "R = λ₁·r_diag + λ₂·r_exam + λ₃·r_turn"
        reward_components:
          diagnosis_reward_r_diag:
            formula: "Binary: 1 if correct diagnosis, 0 otherwise"
            judge: "Qwen2.5-72B with semantic equivalence prompt"
            weight_lambda_1: 1.0
          examination_reward_r_exam:
            formula: "F1 score: 2·|Ê∩E| / (|Ê|+|E|)"
            description: "Overlap between predicted and reference examination sets"
            judge: "Qwen2.5-72B with union set prompts"
            weight_lambda_2: 0.5
          turn_penalty_r_turn:
            formula: "0.1 if T≤T_max, 0 otherwise"
            description: "Penalize excessive dialogue without termination"
            max_turns_T_max: 12
            weight_lambda_3: 1.0
        training_infrastructure:
          total_nodes: 4
          gpus_per_node: 8
          gpu_type: "NVIDIA A100-80GB"
          diaggym_deployment: "2 nodes with vLLM"
          judge_deployment: "1 node (Qwen2.5-72B)"
          agent_training: "All 4 nodes coordinated"
        hyperparameters:
          batch_size: 512
          max_response_length: "8,192 tokens"
          learning_rate: "1×10⁻⁶"
          rollouts_per_sample: 5
          training_steps: 200
          convergence: "Observed within 200 steps"
        framework: "Modified Verl for interactive training"
    
  diagbench_benchmark:
    description: "Comprehensive evaluation benchmark for multi-turn diagnostic trajectories"
    initial_dataset_generation:
      pipeline: "Same as DiagAgent training data construction"
      candidate_cases: 957
      physician_review:
        reviewers: "Multiple practicing physicians"
        review_criteria:
          - "Clinical appropriateness of each analysis step"
          - "Validity of examination recommendations"
          - "Overall case plausibility"
        validated_cases: 750
    standard_evaluation_set:
      cases: 750
      coverage: "Diverse medical specialties and complexity levels"
      components_per_case:
        - "Initial patient inquiry"
        - "Physician-curated referenced diagnostic trajectory"
        - "Final confirmed diagnosis"
      evaluation_metrics:
        examination_recommendation: "Precision, Recall, F1-score"
        diagnosis_accuracy: "Binary correctness"
    rubric_based_evaluation_set:
      initial_sample: "100 cases randomly selected"
      rubric_development_process:
        phase_1:
          reviewers: "2 independent physicians"
          task: "Author process-oriented rubrics for each case"
          focus: "Reasoning process, not just final diagnosis"
        phase_2:
          reviewer: "Third physician"
          task: "Secondary review for completeness and coherence"
          excluded_cases: 1
        phase_3:
          reviewer: "Fourth physician"
          task: "Assign importance weights (0-10 scale)"
          weighting_logic: "10=essential, 0=non-informative"
      final_rubric_set:
        cases: 99
        total_rubrics: 973
        average_rubrics_per_case: "~10 rubrics"
      evaluation_methodology:
        judge: "GPT-4o (gpt-4o-2024-08-06)"
        process: "Binary judgment per rubric (satisfied: Yes/No)"
        scoring: "Weighted sum of satisfied rubrics / total possible weighted score"
    
  evaluation_settings:
    single_turn:
      description: "Oracle single-turn evaluation at each step of reference trajectory"
      setup: "Model extends reference trajectory by one turn (examination or diagnosis)"
      forced_action: "Explicit prompt specifies whether to query examination or make diagnosis"
      data: "750 cases → 4,485 evaluation turns (3,735 examination + 750 diagnosis)"
      metrics:
        examination: "Hit Ratio - whether recommended exam appears in patient's historical records"
        diagnosis: "Accuracy - compared with ground truth"
      judge: "GPT-4o for synonym handling"
    end_to_end:
      description: "Complete diagnostic trajectory generation with simulator interaction"
      initialization: "Initial inquiry only, no examination data"
      interaction: "Model repeatedly queries DiagGym until making final diagnosis"
      simulation: "All examination results generated by DiagGym based on patient profile"
      rationale: "Real EHRs lack results for examinations not performed, preventing full interactive evaluation"
      data: "750 cases for automatic metrics, 99 cases for rubric-based"
      metrics:
        automatic:
          examination: "Precision, Recall, F1 (vs reference trajectory)"
          diagnosis: "Accuracy"
          trajectory_length: "Number of turns"
        rubric_based:
          judge: "GPT-4o evaluating trajectory against 973 rubrics"
          scoring: "Weighted proportion of satisfied rubrics"

ai_methods:
  reinforcement_learning:
    - "Multi-turn policy learning"
    - "End-to-end RL training"
    - "Interactive exploration"
    - "Outcome-based reward signals"
  large_language_models:
    - "Foundation model for diagnostic reasoning"
    - "Natural language understanding of patient history"
    - "Medical knowledge integration"
  world_modeling:
    - "EHR-based simulation"
    - "Conditional outcome generation"
    - "Clinical environment modeling"
  policy_optimization:
    - "Information yield optimization"
    - "Diagnostic accuracy maximization"
    - "Exploration-exploitation balancing"

training_methodology:
  diaggym_development:
    description: "World model trained on electronic health records"
    approach: "Learn to simulate examination outcomes conditioned on patient state"
    data: "Electronic Health Records (EHR)"
    objective: "Create realistic virtual clinical environment"
  diagagent_training:
    description: "RL-based diagnostic policy learning"
    approach: "Multi-turn reinforcement learning"
    environment: "DiagGym virtual clinical environment"
    reward_structure: "Diagnostic accuracy + examination efficiency"
    learning_process:
      - "Interactive exploration of diagnostic strategies"
      - "Outcome-based feedback from DiagGym"
      - "Policy optimization for multi-turn workflows"
      - "Balance information gathering with diagnosis commitment"
  evaluation_framework:
    benchmark: "DiagBench"
    evaluation_types:
      - "Single-turn diagnostic accuracy"
      - "End-to-end multi-turn performance"
      - "Rubric-based process evaluation"
    comparison: "10 SOTA LLMs + 2 prompt-engineered agents"

performance_metrics:
  diaggym_world_model_evaluation:
    test_set: "863 cases (863 distinct diseases)"
    examination_statistics:
      physical_exams_per_case: "8.77 average"
      lab_events_per_case: "28.37 average"
      microbiology_events_per_case: "2.04 average"
      radiology_events_per_case: "2.01 average"
      total_examinations: "35,548 examination records"
    instance_wise_automated_evaluator:
      diaggym:
        step_level_similarity: "3.565/5"
        full_chain_consistency: "96.91%"
      deepseek_v3_671b:
        step_level_similarity: "2.576/5"
        full_chain_consistency: "88.81%"
      qwen2_5_72b:
        step_level_similarity: "2.495/5"
        full_chain_consistency: "92.39%"
      medgemma_27b:
        step_level_similarity: "2.438/5"
        full_chain_consistency: "89.87%"
      qwen2_5_7b:
        step_level_similarity: "2.181/5"
        full_chain_consistency: "81.64%"
    instance_wise_physician_raters:
      sample_size: "100 cases, 3 independent physicians"
      diaggym:
        similarity_physician_1: "4.71/5"
        similarity_physician_2: "4.70/5"
        similarity_physician_3: "4.05/5"
        average_similarity: "4.49/5"
        consistency_physician_1: "96.00%"
        consistency_physician_2: "94.00%"
        consistency_physician_3: "92.00%"
        majority_vote_consistency: "95.00%"
      deepseek_v3_671b:
        average_similarity: "4.09/5"
        majority_vote_consistency: "54.00%"
        failure_mode: "Over-extrapolate from diagnosis, overly severe findings, disjointed narrative"
      qwen2_5_72b:
        average_similarity: "3.97/5"
        majority_vote_consistency: "44.00%"
        failure_mode: "Unsupported neutral/false-positive findings with tenuous diagnosis links"
      medgemma_27b:
        average_similarity: "3.89/5"
        majority_vote_consistency: "74.00%"
        failure_mode: "Logical inconsistencies, conflicting statements across sections"
    examination_wise_numerical:
      selected_examinations: "11 examinations, 24 sub-events (>500 occurrences each)"
      diaggym:
        wasserstein_distance: "0.128 (closer to 0 = better fidelity)"
        normalized_variance: "3.46 (GT baseline: 5.31)"
      deepseek_v3_671b:
        wasserstein_distance: "1.336"
        normalized_variance: "24.56 (highest diversity but lower fidelity)"
      qwen2_5_72b:
        wasserstein_distance: "1.839"
        normalized_variance: "1.21 (overly deterministic)"
      qwen2_5_7b:
        wasserstein_distance: "9.680"
        normalized_variance: "20.18"
      medgemma_27b:
        wasserstein_distance: "16.936"
        normalized_variance: "18.70"
    examination_wise_free_text:
      selected_examinations: "5 radiology types (>100 occurrences each)"
      encoder: "BioLORD biomedical text encoder"
      diaggym:
        fid: "0.747 (lower = better fidelity)"
        lpips: "0.378 (GT baseline: 0.427, higher = more diversity)"
      deepseek_v3_671b:
        fid: "4.158"
        lpips: "0.237"
      qwen2_5_72b:
        fid: "4.901"
        lpips: "0.183"
      qwen2_5_7b:
        fid: "4.800"
        lpips: "0.256"
      medgemma_27b:
        fid: "4.158"
        lpips: "0.341"
    computational_efficiency:
      diaggym:
        minimal_gpus: 1
        time_gpu_seconds: "0.52"
      deepseek_v3_671b:
        minimal_gpus: 16
        time_gpu_seconds: "62.72 (121x slower)"
      qwen2_5_72b:
        minimal_gpus: 4
        time_gpu_seconds: "18.68 (36x slower)"
      medgemma_27b:
        minimal_gpus: 2
        time_gpu_seconds: "9.1 (17.5x slower)"
      qwen2_5_7b:
        minimal_gpus: 1
        time_gpu_seconds: "0.54"
  
  diagagent_single_turn_evaluation:
    dataset: "750 cases → 4,485 evaluation turns (3,735 examination + 750 diagnosis)"
    diagagent_variants:
      diagagent_7b:
        hit_ratio: "72.56%"
        diagnosis_accuracy: "85.60%"
      diagagent_8b:
        hit_ratio: "56.57%"
        diagnosis_accuracy: "82.27%"
      diagagent_14b:
        hit_ratio: "68.49%"
        diagnosis_accuracy: "87.87%"
    basic_llms_closed_source:
      gpt_4o:
        hit_ratio: "20.21%"
        diagnosis_accuracy: "72.13%"
      claude_4_sonnet:
        hit_ratio: "31.63%"
        diagnosis_accuracy: "74.31%"
    basic_llms_open_source:
      deepseek_v3_671b:
        hit_ratio: "20.08%"
        diagnosis_accuracy: "72.27%"
      qwen3_235b:
        hit_ratio: "21.39%"
        diagnosis_accuracy: "72.40%"
      qwen2_5_72b:
        hit_ratio: "19.20%"
        diagnosis_accuracy: "74.80%"
      llama3_3_70b:
        hit_ratio: "19.97%"
        diagnosis_accuracy: "66.27%"
      gpt_oss_120b:
        hit_ratio: "17.37%"
        diagnosis_accuracy: "67.37%"
    medical_llms:
      medgemma_27b:
        hit_ratio: "28.57%"
        diagnosis_accuracy: "60.53%"
        note: "Highest hit ratio among baselines"
      baichuan_m1_14b:
        hit_ratio: "19.60%"
        diagnosis_accuracy: "78.93%"
        note: "Highest diagnosis accuracy among baselines"
      openbiollm_70b:
        hit_ratio: "23.53%"
        diagnosis_accuracy: "66.27%"
    agentic_systems:
      mdagents:
        base_model: "DeepSeek-v3"
        hit_ratio: "20.24%"
        diagnosis_accuracy: "73.47%"
      medagents:
        base_model: "DeepSeek-v3"
        hit_ratio: "19.31%"
        diagnosis_accuracy: "70.27%"
      note: "Agentic systems fail to improve over base models, may worsen hallucination-driven errors"
  
  diagagent_end_to_end_evaluation:
    dataset: "750 cases (automatic metrics), 99 cases (rubric-based)"
    diagagent_variants:
      diagagent_14b:
        avg_turns: "6.66"
        precision: "42.12%"
        recall: "52.12%"
        f1_score: "46.59%"
        accuracy: "61.27%"
      diagagent_7b:
        avg_turns: "5.45"
        precision: "46.14%"
        recall: "46.33%"
        f1_score: "46.23%"
        accuracy: "60.78%"
      diagagent_8b:
        avg_turns: "5.73"
        precision: "39.66%"
        recall: "43.15%"
        f1_score: "41.33%"
        accuracy: "53.45%"
    basic_llms:
      claude_4_sonnet:
        avg_turns: "3.91"
        precision: "33.06%"
        recall: "23.41%"
        f1_score: "27.41%"
        accuracy: "46.14%"
        note: "Best baseline performance"
      deepseek_v3_671b:
        avg_turns: "2.49"
        precision: "36.49%"
        recall: "13.58%"
        f1_score: "19.80%"
        accuracy: "47.08%"
      qwen3_235b:
        avg_turns: "3.34"
        precision: "31.20%"
        recall: "19.23%"
        f1_score: "23.80%"
        accuracy: "45.36%"
      gpt_4o:
        avg_turns: "3.30"
        precision: "32.31%"
        recall: "15.33%"
        f1_score: "20.80%"
        accuracy: "43.24%"
      qwen2_5_72b:
        avg_turns: "2.47"
        precision: "36.03%"
        recall: "12.36%"
        f1_score: "18.40%"
        accuracy: "44.30%"
      llama3_3_70b:
        avg_turns: "4.25"
        precision: "29.02%"
        recall: "22.30%"
        f1_score: "25.22%"
        accuracy: "38.46%"
      gpt_oss_120b:
        avg_turns: "4.08"
        precision: "25.94%"
        recall: "16.16%"
        f1_score: "19.92%"
        accuracy: "44.02%"
      medgemma_27b:
        avg_turns: "4.10"
        precision: "35.38%"
        recall: "21.28%"
        f1_score: "26.58%"
        accuracy: "44.30%"
      baichuan_m1_14b:
        avg_turns: "2.30"
        precision: "32.42%"
        recall: "12.04%"
        f1_score: "17.56%"
        accuracy: "33.16%"
      openbiollm_70b:
        avg_turns: "2.59"
        precision: "35.96%"
        recall: "15.33%"
        f1_score: "21.49%"
        accuracy: "34.35%"
    agentic_systems:
      mdagents:
        avg_turns: "2.40"
        precision: "34.04%"
        recall: "12.56%"
        f1_score: "18.35%"
        accuracy: "44.96%"
      medagents:
        avg_turns: "2.31"
        precision: "33.93%"
        recall: "12.56%"
        f1_score: "18.34%"
        accuracy: "45.62%"
      note: "Limited dialogue turns suggest premature closure without critical information gathering"
    key_observations:
      - "DiagAgent achieves 6-7 turns vs 2-4 for baselines, enabling more comprehensive evidence gathering"
      - "Extended interaction does not sacrifice precision (43.87% DiagAgent-14B vs 32.60% DeepSeek-v3)"
      - "15.12% diagnostic accuracy improvement over best baseline (Claude-4-sonnet)"
      - "Medical-specialized LLMs show no advantage in dynamic setting without robust decision-making"
  
  diagagent_rubric_based_evaluation:
    dataset: "99 cases with 973 physician-written rubrics"
    evaluation_method: "GPT-4o judges trajectory against weighted rubrics (0-10 importance scale)"
    diagagent_14b:
      weighted_rubric_score: "32.86%"
    basic_llms_best_performers:
      claude_4_sonnet:
        weighted_rubric_score: "25.39%"
        delta: "-7.47% vs DiagAgent-14B"
      qwen3_235b:
        weighted_rubric_score: "24.49%"
        delta: "-8.37% vs DiagAgent-14B"
      deepseek_v3_671b:
        weighted_rubric_score: "19.07%"
    agentic_systems:
      mdagents:
        weighted_rubric_score: "21.64%"
        delta: "-11.22% vs DiagAgent-14B"
        note: "Multi-agent discussion provides some improvement over base DeepSeek-v3"
    key_observations:
      - "DiagAgent excels on high-importance rubrics (10-weight criteria)"
      - "Demonstrates superior procedural reasoning beyond final diagnostic accuracy"
      - "Frontier LLMs outperform domain-specialized models due to better generalization"
      - "Process-aware training critical for satisfying physician-validated quality criteria"
  
  ablation_studies:
    sft_vs_rl_comparison:
      qwen2_5_7b:
        zero_shot_accuracy: "16.38%"
        sft_accuracy: "44.40%"
        rl_diagagent_accuracy: "60.78%"
        improvement_sft_to_rl: "+16.38% absolute"
      qwen2_5_14b:
        zero_shot_accuracy: "33.83%"
        sft_accuracy: "45.98%"
        rl_diagagent_accuracy: "61.27%"
        improvement_sft_to_rl: "+15.29% absolute"
      llama3_1_8b:
        zero_shot_accuracy: "25.16%"
        sft_accuracy: "45.35%"
        rl_diagagent_accuracy: "53.45%"
        improvement_sft_to_rl: "+8.10% absolute"
      key_finding: "RL consistently outperforms SFT across all model sizes, reducing dialogue length while improving accuracy"
    reward_design_impact:
      qwen2_5_7b:
        cold_start_only_f1: "38.76%"
        diagnosis_reward_only_accuracy: "59.41%"
        diagnosis_reward_only_f1: "32.76%"
        dual_reward_accuracy: "60.78%"
        dual_reward_f1: "46.23%"
        f1_improvement: "+13.47% with examination reward"
      qwen2_5_14b:
        diagnosis_reward_only_accuracy: "59.73%"
        diagnosis_reward_only_f1: "35.95%"
        dual_reward_accuracy: "61.63%"
        dual_reward_f1: "47.89%"
        f1_improvement: "+11.94% with examination reward"
      llama3_1_8b:
        diagnosis_reward_only_accuracy: "54.12%"
        diagnosis_reward_only_f1: "35.17%"
        dual_reward_accuracy: "53.85%"
        dual_reward_f1: "43.02%"
        f1_improvement: "+7.85% with examination reward"
      key_finding: "Dual-reward (diagnosis + examination) essential for balancing diagnostic accuracy and examination planning quality"
    model_size_impact:
      finding: "All model sizes benefit from RL, but larger/stronger base models achieve higher post-training ceilings"
      qwen2_5_14b_best: "61.63% accuracy, 47.89% F1 (best overall)"
      qwen2_5_7b_strong: "60.78% accuracy, 46.86% F1 (close performance to 14B)"
      llama3_1_8b_lower: "53.85% accuracy, 43.02% F1 (weaker base constrains ceiling)"

validation_approach:
  physician_validation:
    examination_recommendations: "750 cases with expert-validated ground truth"
    process_rubrics: "99 cases with 973 detailed physician annotations"
    clinical_meaningfulness: "Confirmed by practicing physicians"
  comparative_evaluation:
    model_comparison: "10 state-of-the-art LLMs"
    baseline_agents: "2 prompt-engineered diagnostic agents"
    evaluation_dimensions:
      - "Diagnostic accuracy"
      - "Examination recommendation quality"
      - "Process-level reasoning quality"
      - "Multi-turn management capability"
```

## Scientific Background

### Problem Statement

Traditional approaches to training diagnostic AI systems rely on **passive learning from static case summaries**. Instruction-tuned large language models are trained on curated datasets where patient cases, examination results, and final diagnoses are presented in a fixed format. While these models can memorize patterns from training data, they lack the ability to develop **dynamic diagnostic strategies** through interactive exploration.

Key limitations of passive training approaches:

1. **Static Knowledge**: Models learn from fixed case presentations rather than exploring diagnostic pathways
2. **No Exploration**: No mechanism to discover optimal examination selection strategies
3. **Limited Adaptation**: Cannot learn to balance information gathering with diagnostic efficiency
4. **Process vs Outcome**: Focus on final diagnosis rather than diagnostic process quality
5. **Missed Opportunities**: Cannot learn from trial-and-error in safe simulated environments

### Reinforcement Learning Advantage

The DiagAgent framework addresses these limitations through **interactive reinforcement learning** in a virtual clinical environment:

1. **Active Exploration**: Agent discovers diagnostic strategies through trial-and-error
2. **Dynamic Policies**: Learns when to request examinations vs commit to diagnosis
3. **Outcome-Based Learning**: Reward signals based on diagnostic accuracy and efficiency
4. **Process Optimization**: Learns complete diagnostic workflows, not just final decisions
5. **Safe Training**: Exploration in DiagGym simulation without risk to real patients

### Virtual Clinical Environment

**DiagGym** serves as the training ground, providing:

- **Realistic Simulation**: EHR-trained world model generates authentic examination outcomes
- **Conditional Responses**: Outcomes depend on patient history and selected examinations
- **Interactive Feedback**: Agent receives immediate feedback on diagnostic actions
- **Scalable Training**: Unlimited practice cases without real patient data requirements
- **Controlled Evaluation**: Standardized environment for comparing diagnostic strategies

## Methodology

### 1. DiagGym: World Model Development and Training

**Objective**: Create a high-fidelity virtual clinical environment that can simulate realistic examination results for any patient state and examination query, enabling safe, scalable RL training of diagnostic agents.

**MIMIC-IV Data Construction Pipeline**:

**Step 1: Raw Data Collection**
- **Source**: MIMIC-IV v2.2 database (Medical Information Mart for Intensive Care)
- **Discharge Notes**: 331,794 notes containing structured patient information
- **Laboratory Events**: 118,171,368 numerical test results (e.g., CBC, metabolic panels)
- **Microbiology Events**: 3,228,714 culture and sensitivity results
- **Radiology Reports**: 66,542,177 free-text imaging findings

**Step 2: Discharge Note Processing**
- **Extraction Method**: Heuristic string matching on structured headings
- **Patient Profile Components** (extracted from each note):
  - Physical Examination (from "Physical Exam" heading)
  - Chief Complaint (from "Chief Complaint" heading)
  - History of Present Illness (from "Current Medical History" heading)
  - Past Medical History (from "Past Medical History" heading)
  - Social History (from "Social History" heading)
  - Family History (from "Family History" heading)
  - Final Diagnosis (from "Discharge Diagnosis" heading)

**Step 3: Quality Filtering**
- **Filter 1 - Physical Examination**: Exclude cases without physical examination records
- **Filter 2 - Diagnostic Relevance**: Use DeepSeek-v3 with structured prompt to identify and remove cases where:
  - Final diagnosis appears in past medical history (indicates transfer with established diagnosis)
  - Final diagnosis appears in current medical history (lacks diagnostic investigation)
- **Rationale**: Such cases often involve transfers and typically lack diagnostically relevant examinations

**Step 4: Physical Examination Reformatting**
- **Tool**: DeepSeek-v3 with structured prompt
- **Process**: Convert free-text physical examination narratives into structured JSON format
- **Output Format**: `[{exam_name: "...", exam_results: "..."}]`
- **Purpose**: Ensure consistency with other MIMIC-IV structured examination records

**Step 5: Time-Ordered Examination Chain Construction**
- **Initial Examination**: Reformatted physical examination (designated as step 0)
- **Temporal Window**: Select examinations conducted within 1 day prior to admission
  - **Rationale**: Examinations performed earlier have limited diagnostic relevance
  - **Sources**: labevents.csv, microbiologyevents.csv, radiology.csv
- **Laboratory & Microbiology**: Use original structured records from MIMIC-IV
- **Examination Name Standardization**: Apply MIMIC-CDM mapping table to group related items
  - Example: "Red Blood Cell Count" grouped under broader "Complete Blood Count"
- **Radiology Name Completion**: Extract missing names via string-matching from EXAMINATION section
- **Chronological Ordering**: Use timestamps in MIMIC-IV for accurate temporal sequence
- **Deduplication**: For repeated examinations, retain only earliest occurrence per patient

**Step 6: Final Dataset Statistics**
- **Total Cases**: 118,478 restructured EHRs
- **Training Set**: 114,239 cases spanning 4,897 distinct diseases
- **Test Set**: 863 cases (disease-wise sampling: 1 case per disease for balanced evaluation)
- **Average Examinations per Training Case**:
  - Total: 29 examinations
  - Laboratory tests: 26
  - Microbiology tests: 2
  - Radiology tests: 1

**Model Training Specification**:

**Architecture**: 
- **Base Model**: Qwen2.5-Instruct-7B (7 billion parameters)
- **Model Type**: Auto-regressive language model fine-tuned for conditional generation

**Training Objective**:
- **Loss Function**: Token-wise auto-regressive negative log-likelihood
- **Formula**: `L_recon = -∑(t=1 to T) ∑(i) log Φ_env(ê_i^t | a_(t+1), E_t, B)`
  - `ê_i^t`: i-th token of ground-truth examination result at step t
  - `a_(t+1)`: examination query
  - `E_t`: past examination records
  - `B`: patient background profile
- **Treatment**: All examination results treated as free text (numerical values embedded as text)

**Training Configuration**:
- **Framework**: Hugging Face Transformers library with DeepSpeed ZeRO Stage 2
- **Hardware**: 8× NVIDIA A100-80GB GPUs
- **Training Epochs**: 15 (convergence achieved within this period)
- **Learning Rate**: 4×10⁻⁵
- **Max Input Length**: 8,192 tokens
- **Batch Processing**: Distributed optimization across GPUs
- **Convergence**: Validated on held-out set after each epoch

**Deployment for RL Training**:
- **Inference Setup**: Single A100-80GB GPU sufficient for production
- **Generation Speed**: 0.52 seconds per examination result
- **Serving Framework**: vLLM for high-throughput interactive serving
- **Deployment Scale**: 2 nodes during DiagAgent RL training for parallel rollouts

**Key Innovation**: Unlike prior role-playing simulators (AgentClinic, AgentHospital, SDBench) constrained by static pre-collected data, DiagGym can generate novel, clinically plausible trajectories beyond original patient records through learned conditional dependencies.

### 2. DiagAgent: Reinforcement Learning Training Pipeline

**Objective**: Train diagnostic agents that can actively manage complete multi-turn diagnostic trajectories by iteratively selecting informative examinations and committing to accurate final diagnoses through end-to-end reinforcement learning in the DiagGym virtual environment.

**Training Data Construction**:

**Step 1: Source Case Selection**
- **Initial Pool**: 110,000 cases randomly sampled from DiagGym training dataset
- **Subset Selection**: 41,245 cases selected for trajectory generation

**Step 2: LLM-Assisted Trajectory Generation**
- **Tool**: DeepSeek-v3 (671B parameters) with structured prompts
- **Generation Process**: Single-pass generation of three tightly connected components:

**Component 1: Initial Inquiry**
- **Source**: Refinement of existing patient profile
- **Critical Exclusion**: No final diagnosis information included
- **Contents**:
  - Chief Complaint: Primary symptom/reason for seeking care
  - History of Present Illness: Detailed symptom timeline and characteristics
  - Past Medical History: Prior conditions and treatments
  - Family History: Hereditary disease patterns
  - Social History: Lifestyle factors (smoking, alcohol, occupation)
  - Allergy History: Known drug or environmental allergies
- **Refinement**: LLM ensures alignment with realistic clinical inquiry formats
- **Purpose**: Serves as starting point for diagnostic dialogue

**Component 2: Referenced Multi-Turn Diagnostic Trajectory**
- **Source**: Time-ordered examination chain from restructured EHR
- **Selection Criteria**: DeepSeek-v3 prioritizes most informative tests related to final diagnosis
- **Filtering**: Omit non-essential routine examinations
- **Structure per Step**:
  1. **Current Preliminary Diagnosis**: Evolving hypothesis based on accumulated evidence
  2. **Next Recommended Examination**: Specific test name (e.g., "Complete Blood Count", "CT Abdomen")
  3. **Detailed Rationale**: Explanation for why this examination is needed at this point
  4. **Corresponding Test Results**: Actual outcome from EHR records
- **Agent vs Environment Split**:
  - Agent Response (Assistant): Preliminary diagnosis + examination query + rationale (Steps 1-3)
  - Environment Feedback (User): Test results (Step 4)
- **Trajectory Conclusion**: Final diagnostic decision at end-turn
- **Ground Truth**: Examination order and results directly from real EHR physician decisions

**Component 3: Final Diagnosis**
- **Focus**: Single primary condition (self-contained process)
- **Selection**: LLM identifies main diagnostic target from potentially multi-condition original diagnosis
- **Alignment**: Examination selection in trajectory focused on this primary diagnosis

**Step 3: Quality Filtering (Two-Stage Process)**
- **Stage 1 - Format Validation**: DeepSeek-v3 checks adherence to specified data format
- **Stage 2 - Diagnosis Leakage Prevention**: Detect and remove cases where LLM hallucination inadvertently included final diagnosis in initial inquiry
  - **Risk**: Model might reveal diagnosis in earlier text due to next-token prediction bias
  - **Detection Method**: Structured prompt checks initial inquiry against final diagnosis
- **Final Dataset**: 15,324 interactive diagnostic trajectories after filtering

**Step 4: Dialogue Format Conversion**
- **Standard**: Multi-turn conversational format following LLM instruction-tuning datasets
- **Structure**:
  - Turn 1: User message (initial inquiry)
  - Turn 2: Assistant message (preliminary diagnosis + exam query + rationale)
  - Turn 3: User message (examination results)
  - Turn 4: Assistant message (updated diagnosis + next exam query + rationale)
  - ...
  - Turn N: Assistant message (final diagnosis + supporting rationale)
- **Purpose**: Compatible with standard LLM training pipelines

**Training Phase 1: Cold-Start Supervised Fine-Tuning**

**Objective**: Initialize model to produce well-formatted, contextually appropriate diagnostic responses before RL interaction

**Dataset**:
- **Size**: 1,000 cases manually selected from 15,324 training trajectories
- **Quality Criteria**: No formatting issues, no diagnostic reasoning errors
- **Purpose**: Teach output format and basic diagnostic response structure

**Loss Function**:
- **Formula**: `L_cold = -∑(y_i∈assistant) log Φ_diag(y_i | y_≤(i-1))`
- **Computation**: Only over tokens labeled as assistant response
- **Exclusion**: User message tokens (examination results) not included in loss
- **Type**: Standard auto-regressive text generation loss

**Training Configuration**:
- **Framework**: Hugging Face Transformers + DeepSpeed ZeRO Stage 2
- **Hardware**: 8× NVIDIA A100-80GB GPUs
- **Base Models Trained**:
  - Qwen2.5-Instruct-7B
  - Qwen2.5-Instruct-14B
  - Llama3.1-Instruct-8B
- **Hyperparameters** (shared across all models):
  - Max Sequence Length: 8,192 tokens
  - Learning Rate: 1×10⁻⁵
  - Training Epochs: 3
  - Convergence: Observed within 3 epochs
- **Output**: Format-initialized models ready for RL phase

**Training Phase 2: GRPO Reinforcement Learning**

**Algorithm**: Group Relative Policy Optimization (GRPO)
- **Advantage over PPO**: More sample-efficient for LLM fine-tuning
- **Key Feature**: Computes policy gradients using group-based baselines from multiple rollouts

**Interactive Training Setup**:

**Infrastructure**:
- **Total Compute**: 4 nodes, each with 8× NVIDIA A100-80GB GPUs (32 GPUs total)
- **DiagGym Deployment**: 2 nodes running vLLM servers for parallel examination simulation
- **Judge Model Deployment**: 1 node running Qwen2.5-72B for reward evaluation
- **Agent Training**: All 4 nodes coordinated for policy optimization
- **Framework**: Modified Verl library for interactive multi-turn RL

**Rollout Process**:
1. **Initialization**: Agent receives initial inquiry → state s_0 = I
2. **Action Selection**: Agent samples action from policy π_θ(a | s_t)
   - Action space: All clinical examinations + final diagnosis action
   - Sampled examination query sent to DiagGym
3. **Environment Response**: DiagGym generates examination results e_(t+1)
   - Conditioned on patient profile B and examination history E_t
4. **State Update**: s_(t+1) = s_t ∪ (a_(t+1), e_(t+1))
5. **Iteration**: Repeat steps 2-4 until agent selects final diagnosis action (or max 12 turns)
6. **Parallel Rollouts**: 5 different trajectory rollouts per training sample

**Multi-Objective Reward Function**:

**Formula**: `R = λ₁·r_diag + λ₂·r_exam + λ₃·r_turn`

**Component 1: Diagnosis Accuracy Reward (r_diag)**
- **Definition**: Binary indicator of diagnostic correctness
- **Formula**: `r_diag = 1 if ˆd = d, else 0`
  - ˆd: Agent's predicted diagnosis
  - d: Ground-truth diagnosis
- **Judge**: Qwen2.5-72B with structured prompt for semantic equivalence
  - Handles synonyms (e.g., "myocardial infarction" = "heart attack")
  - Checks inclusion relationships (correct diagnosis present even if extra complications mentioned)
- **Weight**: λ₁ = 1.0

**Component 2: Examination Recommendation Reward (r_exam)**
- **Definition**: F1 score measuring overlap with reference examination set
- **Formula**: `r_exam = F1(Ê, E) = 2·|Ê∩E| / (|Ê|+|E|)`
  - Ê: Set of examinations recommended by agent
  - E: Reference examination set from curated trajectory
- **Intersection Computation**: Qwen2.5-72B judges with two prompts:
  - Prompt 1: Count examinations in Ê that appear in E
  - Prompt 2: Count examinations in E that appear in Ê
  - Handles synonyms and examination name variations
- **Weight**: λ₂ = 0.5
- **Rationale**: Balances quality of diagnostic process, not just final outcome

**Component 3: Turn Efficiency Penalty (r_turn)**
- **Definition**: Penalty for excessive dialogue without conclusion
- **Formula**: `r_turn = 0.1 if T ≤ T_max, else 0`
  - T: Number of turns used in rollout
  - T_max = 12: Maximum allowed turns
- **Weight**: λ₃ = 1.0
- **Purpose**: Encourage timely diagnostic decisions, avoid indefinite exploration

**Hyperparameters**:
- **Training Batch Size**: 512 samples
- **Max Response Length**: 8,192 tokens (full examination result narratives)
- **Learning Rate**: 1×10⁻⁶ (10x lower than cold-start for stable RL)
- **Rollouts per Sample**: 5 (for group-relative baseline estimation)
- **Training Steps**: 200
- **Convergence**: Observed within 200 steps for all model variants

**Key Innovations**:
1. **End-to-End Multi-Turn**: Agents manage complete trajectories, not single-step decisions
2. **Outcome-Based Learning**: Reward from diagnostic success, not static supervision
3. **Balanced Objectives**: Dual optimization of accuracy and examination efficiency
4. **Interactive Environment**: Safe exploration in DiagGym before real-world deployment
5. **Scalable Training**: Parallelized infrastructure enables rapid policy iteration

### 3. DiagBench: Comprehensive Diagnostic Benchmark Construction

**Objective**: Create a rigorous, physician-validated benchmark for evaluating multi-turn diagnostic interaction trajectories that assesses both final diagnostic accuracy and the quality of the diagnostic reasoning process.

**Phase 1: Standard Evaluation Set Development (750 Cases)**

**Step 1: Initial Dataset Generation**
- **Pipeline**: Same data construction process as DiagAgent training data
- **Tool**: DeepSeek-v3 generates initial inquiry, diagnostic trajectory, and final diagnosis
- **Candidate Cases**: 957 cases generated

**Step 2: Physician Validation Process**
- **Review Materials Provided**:
  - Patient's initial inquiry (presenting symptoms and history)
  - Complete referenced diagnostic trajectory (step-by-step reasoning and examinations)
  - Final diagnosis
- **Validation Tasks**:
  1. **Step-wise Clinical Appropriateness**: Evaluate each analysis and examination recommendation
  2. **Overall Plausibility**: Assess whether case represents realistic clinical scenario
  3. **Diagnostic Coherence**: Verify logical flow from presentation to diagnosis
- **Reviewer Qualification**: Practicing physicians with clinical diagnostic experience
- **Quality Criteria**:
  - Examination recommendations clinically appropriate for patient state
  - Diagnostic reasoning follows evidence-based medicine principles
  - No internal contradictions or implausible sequences
  - Case complexity appropriate for evaluation purposes

**Step 3: Final Validated Set**
- **Accepted Cases**: 750 out of 957 (78.5% pass rate)
- **Rejection Reasons**: Clinical inappropriateness, implausible scenarios, logical inconsistencies

**Dataset Structure (per case)**:
1. **Initial Patient Inquiry**: Presenting complaint and history (no diagnosis information)
2. **Referenced Multi-Turn Diagnostic Trajectory**: Physician-validated sequence of:
   - Preliminary diagnoses at each step
   - Recommended examinations with rationale
   - Examination results
3. **Final Diagnosis**: Ground-truth diagnostic conclusion

**Usage**: Standard automatic evaluation with precision/recall/F1 for examinations and binary accuracy for diagnosis

**Phase 2: Rubric-Based Evaluation Set Development (99 Cases)**

**Motivation**: Automatic metrics (accuracy, F1) focus on final outcomes and examination overlap but fail to capture the quality of diagnostic reasoning processes. Physician-authored rubrics enable fine-grained assessment of clinical decision-making quality.

**Step 1: Case Sampling**
- **Sample Size**: 100 cases randomly selected from 750 validated cases
- **Purpose**: Enable intensive, time-consuming physician annotation

**Step 2: Independent Rubric Development (2 Physicians)**
- **Reviewers**: 2 practicing physicians assigned independently
- **Materials**: Each physician receives initial inquiry and complete diagnostic trajectory for each case
- **Task**: Author process-oriented rubrics capturing critical evaluation criteria
- **Focus Areas** (emphasized to reviewers):
  - **Diagnostic Reasoning Process**: Not just final diagnosis correctness
  - **History Taking**: Completeness of information gathering
  - **Hypothesis Generation**: Quality of differential diagnoses
  - **Test Ordering Logic**: Appropriateness and timing of examinations
  - **Evidence Integration**: How new results update diagnostic thinking
  - **Decision Points**: When to continue investigation vs commit to diagnosis
- **Independence**: Physicians work separately to ensure diverse rubric coverage
- **Output**: Each physician generates ~10 rubrics per case describing ideal diagnostic process

**Step 3: Secondary Review for Completeness (1 Physician)**
- **Reviewer**: Third physician (different from rubric authors)
- **Task**: Ensure rubric framework comprehensively covers end-to-end diagnostic pipeline
- **Evaluation Criteria**:
  - **Holistic Coverage**: Do rubrics span all critical phases (history → hypothesis → testing → diagnosis)?
  - **Rubric Clarity**: Are criteria well-defined and unambiguous?
  - **Clinical Relevance**: Do rubrics reflect real-world diagnostic standards?
- **Screening Result**: 1 case excluded due to insufficient rubric coverage
- **Final Set**: 99 cases with comprehensive rubric coverage

**Step 4: Importance Weighting Assignment (1 Physician)**
- **Reviewer**: Fourth physician (different from all previous reviewers)
- **Task**: Assign clinical importance weight to each rubric
- **Scale**: 0-10 integer scale
  - **10 points**: Essential, non-negotiable criterion (e.g., "Recognize hemodynamic instability requiring immediate intervention")
  - **7-9 points**: High-importance steps (e.g., "Order appropriate imaging for suspected diagnosis")
  - **4-6 points**: Important but not critical (e.g., "Consider additional differential diagnoses")
  - **1-3 points**: Minor considerations (e.g., "Document patient education")
  - **0 points**: Non-informative or irrelevant criterion
- **Weighting Logic**:
  - High-impact clinical steps (safety-critical decisions) receive maximum weights
  - Routine procedures with lower consequences receive moderate weights
  - Ancillary actions without clear clinical rationale receive minimal weights
- **Example**: "Prioritize emergency resuscitation in unstable patient" = 10 points; "Schedule follow-up appointment" = 2 points

**Final Rubric Statistics**:
- **Total Cases**: 99
- **Total Rubrics**: 973 physician-written criteria
- **Average Rubrics per Case**: ~10 rubrics
- **Rubric Characteristics**:
  - Process-focused (reasoning quality, not just outcomes)
  - Weighted by clinical importance (0-10 scale)
  - Cover multiple diagnostic phases (history, testing, interpretation, decision)
  - Reflect real-world clinical standards

**Evaluation Methodology**:

**Judge Model**: GPT-4o (gpt-4o-2024-08-06)
- **Chosen for**: Strong reasoning capabilities and medical knowledge

**Evaluation Process**:
1. **Input**: Generated diagnostic trajectory from model being evaluated
2. **Task**: For each rubric, judge whether criterion is satisfied
3. **Output**: Binary decision per rubric (Yes/No, or Present/Absent)
4. **Scoring Formula**:
   ```
   Weighted Rubric Score = ∑(satisfied_rubrics) weight_i / ∑(all_rubrics) weight_i
   ```
   - Numerator: Sum of weights for satisfied rubrics
   - Denominator: Sum of weights for all rubrics in case
5. **Aggregation**: Average weighted score across all 99 cases

**Key Innovation**: Unlike HealthBench which evaluates question-answering, DiagBench evaluates complete interactive diagnostic trajectories with step-by-step process assessment, providing granular insights into clinical reasoning quality beyond final diagnostic accuracy.

**Benchmark Usage**:
- **Single-Turn Evaluation**: Test model's ability to extend reference trajectory by one turn
- **End-to-End Automatic**: Evaluate complete generated trajectories with automatic metrics
- **End-to-End Rubric-Based**: Assess trajectory quality against physician-validated criteria

**Public Availability**: Due to MIMIC-IV licensing restrictions, benchmark cannot be directly open-sourced. Authors are communicating with relevant parties regarding potential release on PhysioNet.org.

### 4. Evaluation Methodology

**Three Evaluation Settings**:

**Single-Turn Evaluation**:
- Measure: Diagnostic accuracy, examination recommendation hit ratio
- Setup: Agent makes single diagnostic decision based on patient presentation
- Comparison: 10 SOTA LLMs + 2 prompt-engineered agents

**End-to-End Multi-Turn Evaluation**:
- Measure: Final diagnostic accuracy, examination recommendation F1 score
- Setup: Complete diagnostic workflow with multiple examination selection turns
- Assessment: Both final diagnosis quality and examination selection process

**Rubric-Based Process Evaluation**:
- Measure: Weighted rubric score across 973 physician annotations
- Setup: Detailed process-level assessment of diagnostic reasoning
- Focus: Quality of clinical decision-making and diagnostic pathways
- Validation: Physician-defined criteria for diagnostic excellence

## Results & Validation

### Performance Comparison

**Single-Turn Setting**:
- **Diagnostic Accuracy**: +9.34% improvement over baseline SOTA LLMs
- **Examination Hit Ratio**: +44.03% improvement in selecting appropriate examinations
- **Significance**: Demonstrates superior knowledge integration for diagnostic decisions

**End-to-End Multi-Turn Setting**:
- **Diagnostic Accuracy**: +15.12% increase compared to baseline models
- **Examination F1 Score**: +23.09% boost in examination recommendation quality
- **Significance**: Interactive learning enables superior multi-turn diagnostic management

**Rubric-Based Process Evaluation**:
- **Weighted Score**: +7.1% improvement over Claude-sonnet-4 (next best model)
- **Coverage**: 973 physician-written rubrics across 99 cases
- **Significance**: Clinically meaningful diagnostic processes validated by physicians

### Model Comparison

DiagAgent outperforms all comparison models:

**Frontier LLMs Outperformed**:
1. DeepSeek-v3 (latest model)
2. GPT-4o (OpenAI flagship)
3. Claude-sonnet-4 (Anthropic's best performer)

**Additional 7 SOTA LLMs Outperformed** (names not specified in abstract)

**Prompt-Engineered Agents Outperformed**:
- 2 specialized diagnostic agents with carefully crafted prompts
- Demonstrates that RL training provides advantages beyond prompt engineering

### Key Findings

1. **Interactive Learning Superiority**: Learning policies in interactive clinical environments confers dynamic diagnostic management abilities unattainable through passive training on static data

2. **Multi-Turn Management**: Significant performance gains in end-to-end settings (+15.12% accuracy) demonstrate effective multi-turn diagnostic process management

3. **Examination Selection**: Massive improvement (+44.03% hit ratio) in selecting appropriate examinations shows learned information-gathering strategies

4. **Clinical Meaningfulness**: Physician-validated rubrics confirm that learned diagnostic strategies are clinically appropriate, not just statistically effective

5. **Process Quality**: Superior rubric-based scores (+7.1% vs Claude-sonnet-4) indicate high-quality diagnostic reasoning beyond final accuracy

### Clinical Validation

**Physician Validation Coverage**:
- 750 cases with validated examination recommendations
- 99 cases with detailed process annotations (973 rubrics)
- Multiple physicians involved in validation process
- Clinical expertise confirms meaningfulness of learned strategies

**Validation Dimensions**:
- Appropriateness of examination selections
- Quality of diagnostic reasoning
- Clinical safety and standard-of-care compliance
- Efficiency of diagnostic pathways
- Multi-turn decision-making quality

## Implications for Aging and Longevity

While DiagAgent focuses on general diagnostic capabilities, the framework has significant implications for **preventive health and early detection of age-related conditions**:

### Preventive Diagnostics

1. **Early Disease Detection**: Optimized examination selection could improve early detection of age-related diseases (cardiovascular disease, cancer, neurodegenerative conditions)

2. **Efficient Screening**: Multi-turn diagnostic strategies could optimize screening protocols for aging populations

3. **Risk Assessment**: Adaptive diagnostic policies could improve identification of individuals at risk for age-related decline

### Aging-Related Applications

1. **Geriatric Assessment**: Framework applicable to comprehensive geriatric assessments requiring multi-domain evaluation

2. **Frailty Diagnosis**: Multi-turn approach suitable for frailty assessment involving multiple physiological systems

3. **Cognitive Decline**: Adaptive examination selection for detecting early cognitive impairment

4. **Multimorbidity Management**: Dynamic diagnostic strategies for complex cases common in aging populations

### Future Directions for Longevity Medicine

1. **Biomarker Selection**: RL approach could optimize selection of aging biomarkers for individual assessment

2. **Preventive Interventions**: Diagnostic agents could identify optimal timing for preventive interventions

3. **Personalized Screening**: Learn personalized diagnostic pathways based on individual aging trajectories

4. **Health Optimization**: Extend beyond disease diagnosis to health optimization and longevity promotion

## Lessons Learned

```yaml
achievements:
  diaggym_world_model:
    - "First high-fidelity diagnostics world model achieving 96.91% full-chain consistency"
    - "Closest distribution match to real EHRs: 0.128 Wasserstein distance (vs 1.336 for DeepSeek-v3)"
    - "Physician validation: 4.49/5 similarity score, 95% majority-vote consistency"
    - "121x faster than DeepSeek-v3 (0.52s vs 62.72s) with 16x fewer GPUs"
    - "Trained on 114,239 EHRs spanning 4,897 diseases from MIMIC-IV"
    - "Enables safe, scalable RL training without real patient data access"
    - "Generates novel clinically plausible trajectories beyond original records"
  diagagent_performance:
    - "First RL-trained diagnostic agents significantly outperforming GPT-4o, Claude-sonnet-4, DeepSeek-v3"
    - "Single-turn: 68.49% hit ratio vs 31.63% best baseline (Claude-4), 87.87% accuracy vs 78.93% best baseline"
    - "End-to-end: 61.27% accuracy vs 46.14% best baseline (+15.12% absolute improvement)"
    - "End-to-end examination F1: 46.59% vs 27.41% best baseline (+19.18% absolute improvement)"
    - "Rubric-based: 32.86% weighted score vs 25.39% best baseline (+7.47% absolute improvement)"
    - "Manages 6-7 turn dialogues vs 2-4 for baselines, enabling comprehensive evidence gathering"
    - "Outperforms all 10 SOTA LLMs and 2 agentic systems across all evaluation settings"
  diagbench_contribution:
    - "First comprehensive benchmark for multi-turn diagnostic trajectory evaluation"
    - "750 physician-validated cases with referenced diagnostic pathways"
    - "99 cases with 973 detailed physician-written process rubrics"
    - "Rubric importance weighting (0-10 scale) enables nuanced quality assessment"
    - "Standardized evaluation framework for comparing diagnostic AI systems"
    - "Process-oriented evaluation beyond final diagnostic accuracy"
  methodological_innovations:
    - "First end-to-end multi-turn RL framework for diagnostic agents"
    - "Proved RL consistently outperforms SFT: +16.38% accuracy (Qwen2.5-7B), +15.29% (Qwen2.5-14B)"
    - "Demonstrated dual-reward necessity: +13.47% F1 improvement with examination reward"
    - "GRPO algorithm enables efficient multi-turn policy learning"
    - "Interactive exploration discovers strategies beyond static training data"
    - "Scalable training infrastructure: 32 A100 GPUs, 15,324 training trajectories, 200 RL steps"

implications:
  theoretical_foundations:
    - "Interactive learning in virtual clinical environments confers dynamic diagnostic management abilities fundamentally unattainable through passive training on static data"
    - "Multi-turn diagnostic reasoning requires outcome-based feedback from environment interaction, not just supervised imitation of static trajectories"
    - "Reinforcement learning enables simultaneous optimization of diagnostic accuracy, examination efficiency, and process quality"
    - "World models trained on EHR data can capture conditional dependencies across diseases, histories, and prior tests for realistic simulation"
    - "Diagnostic policies learned through RL can discover strategies beyond recorded physician decisions when they lead to better outcomes"
  clinical_implications:
    - "Physician-validated rubrics (973 annotations) confirm clinical meaningfulness of RL-learned diagnostic strategies"
    - "Extended dialogue length (6-7 turns vs 2-4 for baselines) enables comprehensive evidence gathering without sacrificing precision"
    - "Adaptive examination selection through RL achieves 44.03% higher hit ratio, indicating more informed test ordering"
    - "Process-level evaluation reveals procedural quality beyond final diagnostic correctness"
    - "Virtual clinical environment enables safe exploration of diagnostic strategies before real-world deployment"
    - "Framework addresses fundamental limitation: existing LLMs collapse multi-turn diagnosis into single-shot prediction"
  practical_deployment:
    - "DiagGym's computational efficiency (1 GPU, 0.52s) enables scalable RL training and rapid deployment"
    - "Closed-loop simulation addresses EHR limitation: real records lack results for examinations not performed"
    - "Benchmark with physician-validated rubrics enables standardized comparison of future diagnostic AI systems"
    - "Framework extensible to preventive diagnostics, age-related disease detection, and specialty-specific applications"
    - "Interactive training paradigm applicable to other clinical decision-making tasks beyond diagnosis"
  limitations_of_existing_approaches:
    - "State-of-the-art LLMs (GPT-4o, Claude-4, DeepSeek-v3) trained on passively collected data struggle with multi-turn diagnostic planning"
    - "Medical-specialized LLMs (MedGemma, OpenBioLLM) show no advantage in dynamic settings without robust decision-making training"
    - "Agentic systems (MedAgents, MDAgents) fail to improve over base models, may encourage premature diagnostic closure"
    - "Static instruction-tuning eliminates interaction with environment, preventing policy refinement through feedback"
    - "Supervised fine-tuning limited by static trajectory data that doesn't reflect dynamic branching in interactive consultations"
    - "Prompt engineering alone insufficient: RL training provides advantages beyond careful prompt design"
  scaling_and_generalization:
    - "Performance scales with base model quality: larger/stronger foundation models achieve higher post-training ceilings"
    - "All model sizes (7B, 8B, 14B) benefit from RL, but intrinsic base capabilities constrain attainable performance"
    - "Framework broadly applicable: consistent improvements across Qwen2.5 and Llama3.1 model families"
    - "Dual-reward shaping essential: diagnosis-only reward insufficient for quality examination recommendation"

challenges:
  data_and_resources:
    - "Requires access to high-quality, comprehensive EHR data (MIMIC-IV: 331,794 discharge notes, 118M+ lab events)"
    - "EHR data licensing restrictions: MIMIC-IV requires credentialed access, limits direct benchmark sharing"
    - "Data construction labor-intensive: filtering, quality control, physician validation for 750 benchmark cases"
    - "Rubric development resource-intensive: 4 physicians, 100+ hours for 973 rubrics across 99 cases"
    - "Computational cost: RL training requires 32 A100 GPUs, DiagGym deployment 2 nodes, judge model 1 node"
    - "Training duration: cold-start 3 epochs + RL 200 steps, total training time several days per model"
  clinical_safety_and_validation:
    - "RL-trained agents require rigorous clinical validation before real-world deployment"
    - "Exploration during RL training must be balanced with adherence to clinical safety standards"
    - "Model may discover novel diagnostic strategies that require physician review and validation"
    - "Potential for learned policies to reflect biases present in EHR training data"
    - "Integration with real clinical workflows requires addressing liability and regulatory concerns"
    - "Physicians must retain final decision authority; agents serve as decision support, not replacement"
  technical_limitations:
    - "Models limited to 7B-14B parameters; larger models (DeepSeek-v3 671B, GPT-OSS 120B) not yet trained"
    - "Rubric-based absolute scores modest (32.86%) because rubrics include out-of-scope treatment actions"
    - "DiagAgent focuses on diagnostic reasoning, not emergency resuscitation or surgical team notification"
    - "Generalization to diagnostic scenarios beyond training distribution requires further study"
    - "Current framework limited to diagnosis task; extension to treatment planning and prognosis needed"
    - "Maximum 12-turn constraint may be insufficient for extremely complex diagnostic workups"
  deployment_and_integration:
    - "Integration with existing electronic health record systems requires significant engineering effort"
    - "Real-time deployment requires low-latency inference (DiagGym 0.52s acceptable, but agent response time matters)"
    - "Maintaining performance as medical knowledge evolves requires periodic retraining on updated data"
    - "Handling out-of-distribution cases (rare diseases, atypical presentations) requires robustness guarantees"
    - "Multi-language support needed for international deployment (current framework English-only via MIMIC-IV)"
    - "Interfacing with diverse examination ordering systems across different healthcare institutions"
  evaluation_challenges:
    - "Single ground-truth trajectory limitation: multiple valid diagnostic pathways may exist"
    - "GPT-4o as judge introduces potential biases and limitations in rubric evaluation"
    - "Rubric weights assigned by single physician, may not reflect consensus across medical community"
    - "Automated metrics (F1, accuracy) don't capture all dimensions of diagnostic quality"
    - "Difficult to evaluate agent's handling of ambiguous or incomplete information"
  scope_limitations:
    - "Current scope: diagnosis only, not comprehensive patient management"
    - "Excludes critical emergency actions (resuscitation, surgical consults) reflected in rubric failures"
    - "Limited to single primary diagnosis; multimorbidity management not addressed"
    - "Does not model patient-physician communication nuances, informed consent, shared decision-making"
    - "Assumes perfect information retrieval; doesn't model scenarios where tests unavailable or delayed"

impact_on_field:
  clinical_ai: "Established new paradigm for training diagnostic AI through interactive RL vs passive learning"
  medical_education: "Virtual clinical environments could transform medical training and education"
  decision_support: "Framework foundation for next-generation clinical decision support systems"
  diagnostic_optimization: "Demonstrated that diagnostic processes can be optimized through RL"
  benchmark_development: "DiagBench provides standardized evaluation for future diagnostic AI research"
  preventive_health: "Approach applicable to preventive diagnostics and early disease detection"
  aging_research: "Potential for application to age-related disease detection and geriatric assessment"
```

## Future Directions

### Technical Enhancements

1. **Multi-Modal Integration**: Incorporate imaging, laboratory results, and genomic data into DiagGym
2. **Larger Scale Training**: Expand EHR training data and diagnostic scenario coverage
3. **Transfer Learning**: Apply learned diagnostic strategies across medical specialties
4. **Real-Time Adaptation**: Enable dynamic policy updates based on emerging medical knowledge

### Clinical Applications

1. **Deployment Studies**: Clinical trials evaluating DiagAgent in real healthcare settings
2. **Specialty Adaptation**: Customize for specific medical specialties (cardiology, neurology, oncology)
3. **Decision Support Integration**: Incorporate into electronic health record systems
4. **Physician Collaboration**: Develop hybrid human-AI diagnostic workflows

### Aging and Longevity Applications

1. **Geriatric Diagnostics**: Adapt framework for comprehensive geriatric assessment
2. **Biomarker Optimization**: Apply RL to optimize aging biomarker selection
3. **Preventive Screening**: Develop personalized screening protocols for age-related diseases
4. **Healthspan Optimization**: Extend beyond disease diagnosis to health optimization

### Research Directions

1. **Explainability**: Enhance interpretability of learned diagnostic strategies
2. **Safety Guarantees**: Develop formal verification methods for diagnostic agents
3. **Continuous Learning**: Enable agents to learn from real clinical outcomes
4. **Cross-Cultural Validation**: Test generalization across diverse patient populations

## Detailed Case Studies

### Case Study 1: DiagGym World Model Fidelity

**Patient Profile** (Note ID: 16988189-DS-3)
- **Sex**: Female
- **Chief Complaint**: S/p ERCP with brushing, biliary stent for CHD stricture
- **Presentation**: Painless jaundice
- **History**: Breast cancer (s/p bilateral mastectomy, Adriamycin/Taxol, radiation), hypertension, non-ischemic cardiomyopathy
- **Timeline**: 1 week of nausea, constipation, light-colored stools, itching, yellowing of skin
- **Labs at presentation**: AST 148, ALT 312, Alk phos 421, Tbili 7.6
- **Imaging**: CT showed duct tumor involving common hepatic duct bifurcation (concerning for Klatskin tumor)
- **Final Diagnosis**: CBD obstruction from common hepatic duct mass

**Examination Comparison: DiagGym Prediction vs Ground Truth**

| Examination | DiagGym Prediction | Ground Truth | Clinical Assessment |
|------------|-------------------|--------------|---------------------|
| **General PE** | Well appearing older woman, sitting upright in bed | Well appearing thin woman sitting up in bed in NAD, pleasant | No significant difference; both describe well-appearing patient |
| **Eyes PE** | EOMI, PERRL, anicteric | Icteric sclera, PERRL, EOMI | Prediction missed icterus, but GT confirms jaundice supporting diagnosis |
| **GI PE** | Non-distended, soft, non-tender, hypoactive bowel sounds | Soft, nondistended, mild ttp in epigastrum without rebound | Mild tenderness in GT, but overall benign with no peritonitis |
| **Skin PE** | Yellow hue, multiple nevi, no rash, warm | No rashes noted, icteric skin | Both note jaundice; difference in description detail not significant |
| **Liver Function** | INR 1.1, PT 11.5, ALT 188, Alk phos 388, AST 118 | INR 1.2, PT 12.5, ALT 342, Alk phos 300, AST 195 | All abnormal showing cholestasis/hepatocellular damage; GT values higher but same severe pattern |
| **Total Bilirubin** | 6.7 mg/dL (ref 0-1.5) | 4.3 mg/dL (ref 0-1.5) | Both markedly elevated supporting obstructive jaundice |
| **CBC** | Hct 35.8%, Hgb 12.3, WBC 7.4 | Hct 33.2%, Hgb 11.0, WBC 12.6 | Both show mild anemia; GT WBC higher but not critical |

**Key Finding**: Total Bilirubin predicted at 6.7 mg/dL vs actual 4.3 mg/dL—both well above reference range (0-1.5), both strongly support biliary obstruction diagnosis. Minor numerical variations don't alter clinical interpretation, demonstrating DiagGym's ability to generate plausible realistic results while maintaining clinical fidelity.

### Case Study 2: DiagAgent Dynamic Diagnostic Trajectory (Appendicitis)

**Initial Inquiry** (Note ID: 13544756-DS-14)
- **Sex**: Male
- **Chief Complaint**: Abdominal pain
- **History of Present Illness**: Several hours of periumbilical pain migrating to right lower quadrant. Associated chills, nausea, diarrhea, anorexia. Progressive worsening. Earlier diarrhea, only consumed soup/bread due to nausea.
- **Past Medical History**: Sleep apnea
- **Family History**: Hypertension, diabetes mellitus
- **Allergies**: Penicillins
- **Final Diagnosis**: Appendicitis

**DiagAgent-14B Interactive Trajectory**:

**Turn 1 - Initial Assessment**:
- **Agent Analysis**: "Right lower quadrant pain with nausea, diarrhea, anorexia. Differential: appendicitis, gastroenteritis, other abdominal pathologies."
- **Recommended Test**: Complete Blood Count (CBC)
- **Rationale**: "Evaluate for signs of infection or inflammation (leukocytosis) commonly seen in appendicitis"
- **DiagGym Response**: 
  - Neutrophils: 83.6% (ref 34.0-71.0) - **ABNORMAL**
  - WBC: Normal range
  - Absolute Lymphocyte Count: 0.67 K/uL (ref 1.2-3.7) - ABNORMAL

**Turn 2 - Evidence Integration**:
- **Agent Analysis**: "Elevated neutrophil count (83.6%) suggests inflammatory/infectious process, supporting appendicitis possibility"
- **Recommended Test**: CT Abdomen and Pelvis with Contrast
- **Rationale**: "Visualize appendix and surrounding structures to confirm appendicitis or identify other causes"
- **DiagGym Response**:
  - "Appendix is fluid-filled and abnormally dilated, measuring up to 1.2 cm"
  - "Associated fat stranding and fluid in right lower quadrant"
  - "Findings compatible with acute appendicitis"
  - "No drainable fluid collection or extraluminal gas seen"

**Turn 3 - Final Diagnosis**:
- **Agent Decision**: "Available information sufficient to make diagnosis"
- **Diagnosis**: Appendicitis
- **Supporting Evidence**: "Clinical presentation of RLQ pain, nausea, diarrhea + CT findings of fluid-filled dilated appendix with fat stranding and RLQ fluid confirm acute appendicitis"

**Comparison with Referenced Trajectory**:
- **Step 1**: Both recommend CBC based on clinical presentation ✓
- **Step 2**: Both identify elevated neutrophils as inflammatory sign ✓
- **Step 3**: Both proceed to CT imaging for confirmation ✓
- **Step 4**: Both correctly diagnose appendicitis based on imaging ✓

**Clinical Assessment**: Agent's decisions follow standard diagnostic reasoning, appropriate step progression from initial labs to confirmatory imaging, accurate interpretation of findings at each stage.

### Case Study 3: Rubric-Based Success Case (Left Lower Extremity Infection)

**Case Details** (Note ID: 13309322-DS-4)
- **Sex**: Male
- **History**: Left pilon fracture from fall, treated with external fixation → ORIF
- **Presentation**: Progressive pain, swelling, erythema in LLE. One area of serosanguineous drainage. On Keflex for cellulitis concern.
- **Clinical State**: Able to bear full weight, no motor/sensory deficits
- **Final Diagnosis**: LLE cellulitis caused by Staphylococcus aureus

**DiagAgent-14B Trajectory with Rubric Evaluation**:

| Turn | Action | Rubric Criterion | Weight | Satisfied |
|------|--------|-----------------|--------|-----------|
| 1 | Order CBC | "Prioritize CBC in initial assessment to evaluate infection signs (leukocytosis/bandemia)" | 9/10 | ✓ Yes |
| 2 | Order Wound Culture after elevated neutrophils | "Timely recommend wound culture to identify causative organism and guide antibiotics" | 8/10 | ✓ Yes |
| 3 | Order Blood Cultures after S. aureus isolated | "Reasonably suggest blood cultures to rule out bacteremia/systemic infection" | 7/10 | ✓ Yes |
| 4 | Finalize diagnosis after negative blood cultures | "Timely confirm final diagnosis after negative cultures, avoiding unnecessary further investigation" | 6/10 | ✓ Yes |
| - | Consistent differential consideration | "Consistently consider osteomyelitis possibility without over-relying on it, prioritizing more probable cellulitis" | 5/10 | ✓ Yes |
| - | Correct lab interpretation | "Correctly interpret elevated neutrophil % without misinterpreting as systemic infection" | 4/10 | ✓ Yes |
| - | Demonstrate antibiotic resistance awareness | "Demonstrate awareness of S. aureus resistance patterns in antibiotic selection" | 3/10 | ✗ No |
| - | Consider vascular complications | "Appropriately consider/rule out vascular complications (DVT) during diagnostic process" | 2/10 | ✗ No |

**Rubric Score**: 45/50 satisfied weight points = 90% weighted rubric score

**Key Strengths**:
1. **High Coherence**: Logical progression from initial assessment → organism identification → systemic spread evaluation
2. **Dynamic Strategy**: After negative blood cultures, efficiently terminates investigation (avoids over-testing)
3. **Process Quality**: Satisfies all high-weight rubrics (6-10 points), demonstrating clinically sound decision-making

**Analysis**: Agent demonstrates robust procedural performance with step-by-step reasoning matching physician expectations for high-priority diagnostic actions.

### Case Study 4: Rubric-Based Failure Case (Ruptured Ectopic Pregnancy)

**Case Details** (Note ID: 10172388-DS-17)
- **Sex**: Female
- **Presentation**: Sudden-onset abdominal pain while driving, pulled over
- **Clinical State**: Hemodynamically unstable (SBP 80, tachycardia)
- **FAST Scan**: Positive for intra-abdominal fluid
- **History**: Unaware of pregnancy, spontaneous abortion ×1, SVD ×1
- **Final Diagnosis**: Ruptured ectopic pregnancy with hemodynamic instability

**DiagAgent-14B Trajectory with Rubric Evaluation**:

| Turn | Action | Rubric Criterion | Weight | Satisfied |
|------|--------|-----------------|--------|-----------|
| 1 | Order hCG | "Identify 'Ruptured ectopic pregnancy' as most probable diagnosis" | 10/10 | ✓ Yes |
| 2 | Order Pelvic Ultrasound after positive hCG | "Appropriately manage imaging without delaying surgical intervention in unstable patient" | 8/10 | ✓ Yes |
| 3 | Order CBC after ultrasound shows adnexal mass | "Provide concise differential for hemoperitoneum, correctly prioritizing ruptured ectopic" | 7/10 | ✓ Yes |
| 4 | Order Coagulation Profile | "Explain necessity of each test and how it alters immediate management" | 6/10 | ✓ Yes |
| 5 | Make final diagnosis | **"Propose prioritized resuscitation plan: Simultaneous fluid resuscitation, immediate OB/Gyn team, emergent OR transfer"** | **10/10** | **✗ No** |
| - | - | **"Recommend hemorrhagic shock resuscitation: 2 large-bore IVs, rapid crystalloids, massive transfusion protocol"** | **9/10** | **✗ No** |
| - | - | **"Order necessary labs: Type/screen/crossmatch, coags, BMP, Lactate, Rh typing"** | **8/10** | **✗ No** |
| - | - | **"State Rh-D immunoglobulin for Rh-negative patient"** | **7/10** | **✗ No** |
| - | - | **"Describe surgical management options (Salpingectomy vs Salpingostomy) based on findings"** | **5/10** | **✗ No** |

**Rubric Score**: 31/57 satisfied weight points = 54% weighted rubric score

**Diagnostic Strengths**:
- Correctly orders hCG based on presentation (unstable female with abdominal pain)
- Appropriately progresses to pelvic ultrasound after positive pregnancy test
- Successfully identifies ruptured ectopic pregnancy as final diagnosis

**Critical Omissions** (All High-Weight Rubrics):
1. **Emergency Resuscitation** (10/10 weight): No mention of immediate fluid resuscitation, transfusion protocol
2. **Surgical Team Notification** (implied in 10/10 rubric): No explicit call for OB/Gyn and OR preparation
3. **Hemorrhagic Shock Management** (9/10 weight): Missing large-bore IV access, massive transfusion protocol
4. **Critical Lab Orders** (8/10 weight): No type/crossmatch for blood products, no Rh typing
5. **Rh Immunoglobulin** (7/10 weight): Critical for Rh-negative patients, completely absent

**Scope Limitation**: DiagAgent designed as diagnostic reasoning model, not comprehensive emergency management system. Core diagnostic capability (accurate differential + sequential information gathering) remains intact and validated. Gap in acute therapeutic/stabilization management falls outside initial scope. This case illustrates the distinction between diagnostic excellence and complete clinical management.

**Future Extension**: Integrating long-term management with timely treatment planning alongside diagnostic procedure represents clear direction for aligning clinical LLMs with practical usage demands.

## Conclusion

DiagAgent represents a fundamental advance in training diagnostic AI systems, demonstrating that **interactive reinforcement learning in virtual clinical environments** produces superior diagnostic agents compared to passive learning on static data. The framework's three components—DiagGym (world model), DiagAgent (RL agent), and DiagBench (evaluation benchmark)—work synergistically to enable dynamic diagnostic management abilities unattainable through traditional training approaches.

With demonstrated superiority over 10 state-of-the-art LLMs including GPT-4o and Claude-sonnet-4, validated by practicing physicians through comprehensive rubrics, DiagAgent establishes a new paradigm for clinical AI development. The framework's potential applications extend to **preventive health and age-related disease detection**, offering promising avenues for improving diagnostic accuracy and efficiency in aging populations.

The detailed case studies demonstrate:
1. **DiagGym Fidelity**: Generates clinically realistic examination results with appropriate variability
2. **DiagAgent Competence**: Manages multi-turn diagnostic workflows with coherent step-by-step reasoning
3. **Rubric Validation**: High performance on physician-defined process criteria confirms clinical meaningfulness
4. **Scope Awareness**: Current focus on diagnostic reasoning; extension to comprehensive management needed

As the field moves toward more sophisticated AI-assisted clinical decision support, DiagAgent's interactive learning approach provides a blueprint for developing agents that can truly manage complex diagnostic workflows with clinical meaningfulness and safety.

