---
id: sr-scientist-equation-discovery
slug: sr-scientist-equation-discovery
entity_type: research
status: published
data_completeness: exceptional
last_researched: 2025-01-20
research_category: collaboration
researcher: AI Assistant
version: 2.0
name: "SR-Scientist: Scientific Equation Discovery With Agentic AI"
description: "SR-Scientist is a revolutionary framework that elevates Large Language Models (LLMs) from simple equation proposers to autonomous AI scientists capable of writing code to analyze data, implementing equations as code, submitting them for evaluation, and optimizing equations based on experimental feedback. Unlike traditional methods that confine LLMs to the role of equation generators within search algorithms like genetic programming, SR-Scientist wraps the code interpreter into a set of tools for data analysis and equation evaluation, enabling the agent to optimize equations over long horizons with minimal human-defined pipelines. The framework demonstrates superior performance, outperforming baseline methods by an absolute margin of 6% to 35% on datasets covering four science disciplines (chemistry, biology, physics, and material science). The system achieves 63.57% accuracy at 0.01 tolerance and 49.35% at 0.001 tolerance with GPT-OSS-120B as backbone. Additionally, SR-Scientist demonstrates robustness to noise (tested with Gaussian noise σ = 0.01, 0.05, 0.1), generalization to out-of-domain data, and symbolic accuracy in discovering ground truth equations. The framework includes an end-to-end reinforcement learning pipeline using Group Relative Policy Optimization (GRPO) that enhances agent capabilities, with training on 1024 synthetic problems resulting in significant performance improvements across all scientific domains."
mission: To transform LLMs into autonomous AI scientists that can independently discover scientific equations through long-horizon, tool-driven data analysis and equation evaluation, eliminating the need for extensive human-defined pipelines and accelerating scientific discovery across multiple disciplines.
entity_data:
  name: SR-Scientist
  status: published
  objectives:
    - Elevate LLMs from equation proposers to autonomous AI scientists
    - Enable autonomous data analysis through code interpreter tools
    - Implement long-horizon optimization with minimal human-defined pipelines
    - Optimize equations based on experimental feedback over multiple iterations (up to 40)
    - Demonstrate superior performance across chemistry, biology, physics, and material science
    - Validate robustness to noise in observed data
    - Demonstrate generalization to out-of-domain data
    - Validate symbolic accuracy of discovered equations
    - Develop end-to-end reinforcement learning framework using GRPO
    - Reduce computational cost while maintaining or improving performance
  start_date: 2024
  publication_date: 2025-10-13
  methodology: "Agentic AI framework using ReAct paradigm with code interpreter tools wrapped as data analyzer and equation evaluator. Agent performs long-horizon optimization (up to 25 turns per iteration, 40 iterations total) with experience buffer to manage explored equations. LLM agent writes code for data analysis, implements equations as Python functions with parameter placeholders, submits to BFGS optimizer for parameter fitting, and iteratively refines based on Mean Absolute Percentage Error (MAPE) feedback. Experience buffer maintains heap of explored equations, fetching top-K best performers for subsequent iterations to overcome context length limitations. Reinforcement learning training uses GRPO algorithm with log-linear reward function, 1024 synthetic training problems, batch-level asynchronous rollouts on 32 H200 GPUs using verl framework with SGLang rollout engine and FSDP training engine."
  results: "Outperforms baseline methods by 6% to 35% absolute margin on LSR-Synth benchmark covering 129 problems across four science disciplines. Best performance achieved with GPT-OSS-120B: 63.57% Acc₀.₀₁ and 49.35% Acc₀.₀₀₁ overall. Material science: 86.67% (Qwen3-Coder-480B), Chemistry: 81.48% (GPT-OSS-120B), Biology: 66.67% (GPT-OSS-120B), Physics: 40.91% (GPT-OSS-120B) at 0.01 tolerance. Demonstrates robustness to Gaussian noise (σ = 0.01, 0.05, 0.1) with consistent superior performance. Generalizes well to out-of-domain data across all disciplines. Achieves 7.75% symbolic accuracy (highest among all methods). Reinforcement learning training on Qwen3-Coder-30B improves performance from 32.30% to 40.92% Acc₀.₀₁ and 16.02% to 20.69% Acc₀.₀₀₁. Ablation studies show data analysis tool contributes 17.91-27.91% improvement and experience buffer contributes 6.21-11.15% improvement. Cost-effective: $0.25 per problem with GPT-OSS-120B, $0.1 with GPT-OSS-20B. Inference time: maximum 5 hours for 129 problems with GPT-OSS-120B on 2×H100."
  collaboration_period:
    start: 2024
    publication_date: 2025-10-13
    status: published
  author_contributions:
    co_first_authors:
      - Shijie Xia
      - Yuhan Sun
    corresponding_author: Pengfei Liu
    methodology:
      - Shijie Xia
      - Yuhan Sun
      - Pengfei Liu
    investigation:
      - Shijie Xia
      - Yuhan Sun
      - Pengfei Liu
    writing_original_draft:
      - Shijie Xia
      - Yuhan Sun
      - Pengfei Liu
  competing_interests:
    no_conflicts: All authors
  supplementary_data:
    github_repository: "https://github.com/GAIR-NLP/SR-Scientist"
    models: "SR-Scientist-30B"
    benchmark: "LSR-Synth (LLM-SRBench synthetic subset)"
taxonomy:
  geography: China
  ai_approach:
    - Generative AI
    - Reinforcement Learning
    - Active Learning
  ai_technology:
    - LLMs
    - Generative AI
    - Reinforcement Learning
  ai_architecture:
    - LLMs
  ai_specialization:
    - Multi-Agent AI
    - RAG
  primary_focus:
    - Autonomous AI Scientists
  aging_approach: []
  target_biology: []
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration
  therapeutic_modality: []
organizations:
  - name: Shanghai Jiao Tong University
    role: primary
    org_type: institution
    legal_name: Shanghai Jiao Tong University
    status: active
    website: "https://www.sjtu.edu.cn/"
    role_description: Primary research institution for all authors
    contribution_description: Provided research infrastructure and academic environment for developing SR-Scientist framework. All three authors are affiliated with Shanghai Jiao Tong University.
    description: Major research university in Shanghai, China, one of the oldest and most prestigious universities in China
    focus: Engineering, technology, science, medicine, and research
  - name: SII (Shanghai Institute of Intelligent Science and Technology)
    role: primary
    org_type: research_center
    status: active
    role_description: Research institute affiliation for Shijie Xia and Pengfei Liu
    contribution_description: Provided research support and institutional framework for the project
    description: Research institute focused on intelligent science and technology
    focus: AI research, intelligent systems, technology development
  - name: GAIR (Generative AI Research)
    role: primary
    org_type: research_center
    status: active
    role_description: Research center affiliation for all three authors
    contribution_description: Provided research environment focused on generative AI, supporting the development of SR-Scientist as an agentic AI system
    description: Research center specializing in generative AI research
    focus: Generative AI, large language models, AI agents, scientific AI applications
people:
  - name: Shijie Xia
    person_type: researcher
    role: Co-first Author
    affiliations:
      - Shanghai Jiao Tong University
      - SII
      - GAIR
    contribution_description: Co-first author who co-developed SR-Scientist framework, designed methodology, conducted experiments, and co-wrote manuscript
    expertise: Agentic AI, Scientific discovery, Equation discovery, Reinforcement learning
  - name: Yuhan Sun
    person_type: researcher
    role: Co-first Author
    affiliations:
      - Shanghai Jiao Tong University
      - GAIR
    contribution_description: Co-first author who co-developed SR-Scientist framework, designed methodology, conducted experiments, and co-wrote manuscript
    expertise: Agentic AI, Scientific discovery, Equation discovery, Large language models
  - name: Pengfei Liu
    person_type: pi
    role: Corresponding Author
    affiliations:
      - Shanghai Jiao Tong University
      - SII
      - GAIR
    contribution_description: Corresponding author who supervised the project, co-developed SR-Scientist framework, provided research direction, and co-wrote manuscript
    expertise: Natural language processing, Large language models, Agentic AI, Scientific AI
products:
  - name: SR-Scientist Framework
    type: platform
    status: published
    development_stage: Research / Preclinical
    description: "Autonomous AI scientist framework that transforms LLMs into agents capable of discovering scientific equations through long-horizon optimization. Uses ReAct framework with code interpreter tools for data analysis and equation evaluation."
    capabilities:
      - Autonomous data analysis via code interpreter
      - Equation implementation as Python functions with parameter placeholders
      - Automated parameter optimization using BFGS algorithm
      - Long-horizon optimization (25 turns × 40 iterations)
      - Experience buffer for managing explored equations
      - Minimal human-defined pipelines
      - Reinforcement learning enhancement via GRPO
      - Robustness to noise
      - Generalization to out-of-domain data
      - Symbolic accuracy validation
      - Multi-disciplinary application (chemistry, biology, physics, material science)
    technical_details:
      ai_methods: "Agentic AI with ReAct framework, Code interpreter tools, GRPO reinforcement learning, BFGS parameter optimization, Long-horizon optimization, Experience buffer management"
      architecture: "LLM-based autonomous agent with two wrapped tools: data_analyzer (code interpreter for data exploration) and equation_evaluator (code interpreter + BFGS optimizer for parameter fitting and performance evaluation)"
      training_data: "1024 synthetic problems across four scientific domains using mixed rule-based and model-based synthesis"
      performance_metrics: "Best overall: 63.57% Acc₀.₀₁, 49.35% Acc₀.₀₀₁ (GPT-OSS-120B). Material science: 86.67% Acc₀.₀₁. RL training improves Qwen3-30B from 32.30% to 40.92% Acc₀.₀₁"
      validation: "Validated on LSR-Synth benchmark (129 problems), robustness to noise tests, out-of-domain generalization tests, symbolic accuracy evaluation"
  - name: SR-Scientist-30B
    type: ai_model
    status: published
    description: "Fine-tuned model based on Qwen3-Coder-30B-A3B with reinforcement learning training on 1024 SR problems"
    technical_details:
      base_model: "Qwen3-Coder-30B-A3B-Instruct"
      training_method: "GRPO reinforcement learning (60 steps, 32 H200 GPUs)"
      performance: "40.92% Acc₀.₀₁ (vs 32.30% base), 20.69% Acc₀.₀₀₁ (vs 16.02% base)"
links:
  - url: "https://arxiv.org/abs/2510.11661"
    type: research_publication
    title: "SR-Scientist: Scientific Equation Discovery With Agentic AI"
    authors:
      - Shijie Xia
      - Yuhan Sun
      - Pengfei Liu
    publication_date: 2025-10-13
    relevance: primary
    category: source
    description: "Primary research publication describing SR-Scientist framework, methodology, results, and reinforcement learning approach"
    metadata:
      arxiv_id: "2510.11661"
      doi: "10.48550/arXiv.2510.11661"
  - url: "https://github.com/GAIR-NLP/SR-Scientist"
    type: github
    title: "SR-Scientist GitHub Repository"
    description: "Official implementation of SR-Scientist framework with code, models, and experimental setup"
    relevance: primary
    category: source
financials:
  - category: grant
    source: "National Natural Science Foundation of China"
    funding_type: "Research Grant"
    description: "Research funding for the project"
    details:
      grant_number: "62476168"
  - category: grant
    source: "National High Technology Research and Development Program of China"
    funding_type: "Research Grant"
    description: "High technology research program funding"
    details:
      grant_number: "2015AA015408"
  - category: grant
    source: "Shanghai Science and Technology Development Funds"
    funding_type: "Research Grant"
    description: "Local science and technology development funding"
    details:
      grant_number: "14ZR1403200"
  - category: grant
    source: "Shanghai Municipal Commission of Economy and Informatization"
    funding_type: "AI for Science Program"
    description: "AI for Science program funding"
    details:
      grant_number: "2025-GZL-RGZN-BTBX-01013"
---

# SR-Scientist: Scientific Equation Discovery With Agentic AI

*Published October 13, 2025 | Shanghai Jiao Tong University, SII, GAIR*  
*Authors: Shijie Xia\*, Yuhan Sun\*, Pengfei Liu† (\*Co-first authors, †Corresponding author)*

**Code**: https://github.com/GAIR-NLP/SR-Scientist | **Models**: SR-Scientist-30B

## Executive Summary

SR-Scientist представляет собой революционный фреймворк, который преобразует Large Language Models (LLMs) из простых генераторов уравнений в автономных AI-учёных, способных самостоятельно открывать научные уравнения. Опубликованный 13 октября 2025 года исследователями из Shanghai Jiao Tong University, система демонстрирует, что при правильном дизайне LLMs могут автономно открывать научные уравнения через длительную оптимизацию, управляемую экспериментальной обратной связью.

**Ключевые достижения:**
- **63.57% точность** (Acc₀.₀₁) с GPT-OSS-120B против 29.46% у лучшего baseline (PySR) - **+34.11% absolute improvement**
- **Улучшение на 6-35%** абсолютных пунктов на 4 научных дисциплинах
- **Высшая символическая точность** (7.75%) среди всех методов
- **Робастность к шуму** (Gaussian σ до 0.1)  
- **Сильная обобщаемость** на out-of-domain данные
- **Cost-effective**: $0.10-0.25 за задачу, 5 часов для 129 задач

**Ключевые инновации:**
1. **Minimal human-defined pipelines**: Агент определяет собственный workflow
2. **Long-horizon optimization**: До 25 turns × 40 iterations
3. **Experience buffer**: Преодолевает ограничения context length
4. **End-to-end RL**: GRPO обучение на 1024 задачах

## 1. Введение и мотивация

### 1.1 Эволюция символической регрессии

Математические уравнения являются центральными для научного прогресса, служа краткими и интерпретируемыми моделями физических явлений. Задача **data-driven equation discovery**, также известная как **symbolic regression (SR)**, является NP-hard проблемой из-за огромного пространства поиска.

**Исторический контекст:**

**Traditional Era (до 2020)**:
- **Genetic Programming**: PySR, GPLearn - комбинаторный поиск через evolution
- **Deep Learning**: E2E, NeSymReS, DSR, uDSR - обучение на synthetic data
- **Проблемы**: Inefficiency, scalability issues, требуют огромных computational resources

**LLM Era (2020-2024)**:
- LLMs embedded в GP algorithms как equation proposers
- LaSR: Library-Augmented SR с concept evolution
- LLM-SR: LLM генерирует candidate equations для GP
- **Ограничения**: LLMs остаются статическими компонентами в human-crafted pipelines

**Agentic AI Era (2025+)**:
- **SR-Scientist**: LLM как autonomous agent с tools
- Minimal human-defined pipelines
- Long-horizon optimization с feedback
- Self-improvement через reinforcement learning

### 1.2 Почему Agentic AI для SR?

В эпоху Agentic AI, LLMs эволюционировали от simple retrievers к agentic models способным выполнять сложные задачи через interaction с environment. Примеры: Claude Code (Anthropic), Gemini CLI (Google).

**Характеристики autonomous AI scientists:**
- **Long-horizon interaction** с environmental feedback
- **Operational autonomy** - определяют собственный workflow
- **Tool-driven exploration** вместо fixed procedures
- **Learning from experience** через trial and error

**Проблема с существующими LLM-SR методами:**
1. **Fixed pipelines**: LLMs генерируют equations, GP evaluates - нет гибкости
2. **No data analysis**: LLMs не могут explore data напрямую
3. **Short interactions**: Limited feedback loops
4. **No learning**: Каждая задача starts from scratch

**SR-Scientist решение:**
1. **Autonomous agent** с code interpreter tools
2. **Direct data analysis** перед generation
3. **Long-horizon optimization** (25 turns × 40 iterations)
4. **Experience buffer** для learning across iterations
5. **RL training** для capability enhancement

### 1.3 Ключевые принципы дизайна

**1. Minimal Human-Defined Pipelines** (Sutton's "Bitter Lesson"):
> "The biggest lesson that can be read from 70 years of AI research is that general methods that leverage computation are ultimately the most effective." — Richard Sutton, 2019

**SR-Scientist approach:**
- Provide: **Tools** (data analyzer, equation evaluator) + **Goal** (MAPE < threshold)
- Agent determines: How to use tools, when to analyze data, which equations to try
- No pre-defined steps or procedures

**2. Long-Horizon Optimization:**
- Traditional: 1-3 turns per attempt
- SR-Scientist: Up to 25 turns × 40 iterations
- Enables: Deep exploration, iterative refinement, learning from failures

**3. Tool-Driven Autonomy:**
- Not just equation generation
- Active data analysis
- Residual error inspection
- Parameter interpretation

**4. Learning from Experience:**
- Experience buffer: Stores explored equations with scores
- RL training: Learns general strategies across problems

## 2. Формулировка проблемы

### 2.1 Symbolic Regression Definition

**Given:** Dataset D = {(x_i, y_i)}ⁿ_{i=1}, where:
- **x_i ∈ ℝᵈ**: Input vector (d variables)
- **y_i ∈ ℝ**: Scalar output

**Find:** Symbolic function f such that f(x_i) ≈ y_i

**Requirements:**
1. **Accuracy**: Minimize prediction error on training data
2. **Generalization**: Perform well on unseen (OOD) inputs  
3. **Interpretability**: Symbolic form understandable by humans
4. **Parsimony**: Simple equations preferred over complex ones
5. **Physical plausibility**: Respect known physical constraints (when applicable)

### 2.2 Why is SR NP-Hard?

**Challenges:**

1. **Infinite search space**: 
   - Infinite possible structures (addition, multiplication, sin, exp, log, ...)
   - Infinite possible constants
   - Combinatorial explosion with depth

2. **Non-convex optimization**:
   - Parameter fitting is non-convex (multiple local optima)
   - Structure search is discrete (no gradients)

3. **Accuracy-interpretability trade-off**:
   - More complex equations → better fit
   - Simple equations → better interpretation
   - Finding optimal balance is hard

**Example complexity:**
- Depth 3 equation: ~10³ possible structures
- Depth 5 equation: ~10⁷ possible structures  
- Depth 10 equation: ~10¹⁵ possible structures

### 2.3 Evaluation Metric: MAPE

SR-Scientist использует **Mean Absolute Percentage Error (MAPE)** как primary optimization metric:

**MAPE = (100%/n) × Σⁿ_{i=1} |y_i - f(x_i)| / |y_i|**

**Why MAPE instead of MSE/NMSE?**

1. **Uniform precision target**: MAPE < 0.1% means <0.1% error regardless of data scale
2. **Interpretability**: Percentage error intuitive for scientists
3. **Natural stopping criterion**: Clear target (e.g., MAPE < 0.1%)
4. **Aggregation**: Works better when averaging across multiple problems

**Comparison:**
- **MSE**: Sensitive to outliers, scale-dependent
- **NMSE**: Better than MSE, but still less interpretable
- **R²**: Too easy (most methods achieve >0.99)
- **MAPE**: Best balance of interpretability and challenge ✓

### 2.4 Benchmark: LSR-Synth

**LLM-SRBench Synthetic Subset:**
- **Total problems**: 129
- **Domains**: Chemistry (36), Biology (24), Physics (44), Material Science (25)
- **Design philosophy**: Prevent memorization

**How to prevent LLM memorization:**
1. **Known + Novel terms**: Each equation combines:
   - At least 1 known term (from standard equations)
   - At least 1 novel term (creative, outside typical knowledge)
2. **Synthesis verification**: Authors manually checked for duplicates
3. **Moderate complexity**: 2-4 terms per equation

**Data splits:**
- **Training set**: Accessible to SR method during optimization
- **In-Domain (ID) test**: Same distribution as training
- **Out-of-Domain (OOD) test**: Extreme conditions (high T, long t, etc.)

**Example problems:**
- **Chemistry**: Reaction rate with novel autocatalytic term
- **Biology**: Population growth with non-standard mortality function
- **Physics**: Nonlinear oscillator with cubic damping
- **Material Science**: Stress-strain with temperature-dependent modulus

## 3. Архитектура SR-Scientist

### 3.1 Общая схема системы

SR-Scientist состоит из четырех ключевых компонентов:

1. **LLM Agent** (ReAct framework) - core autonomous scientist
2. **Two Wrapped Tools** - data_analyzer и equation_evaluator
3. **Experience Buffer** - heap-based storage explored equations
4. **RL Training Pipeline** - GRPO для capability enhancement

### 3.2 Component 1: Tool Design

#### Data Analyzer Tool (T₁)

**Purpose**: Enable agent to explore and understand data before proposing equations

**Capabilities:**
- Print data samples for inspection
- Calculate statistics (mean, std, correlation, min/max)
- Analyze patterns and relationships
- Perform residual analysis
- Any Python code for numerical analysis

**Restrictions:**
- No visualization libraries (Matplotlib forbidden)
- Synchronous execution
- Timeout: 30 seconds
- Max output: 10,000 characters

**Common usage patterns:**

```python
# Pattern 1: Data inspection
print(data_list[:5])
print(f"Total rows: {len(data_list)}")

# Pattern 2: Statistical analysis
outputs = [row[0] for row in data_list]
inputs_1 = [row[1] for row in data_list]
print(f"Output range: [{min(outputs)}, {max(outputs)}]")
print(f"Correlation: {np.corrcoef(outputs, inputs_1)[0,1]:.3f}")

# Pattern 3: Residual analysis (after equation proposed)
residuals = [abs(outputs[i] - predictions[i]) for i in range(len(outputs))]
print(f"Mean residual: {np.mean(residuals):.6f}")
```

#### Equation Evaluator Tool (T₂)

**Purpose**: Automatically optimize equation parameters and return performance metrics

**Input format:**
```python
def equation(var1: np.ndarray, var2: np.ndarray, ..., params: np.ndarray) -> np.ndarray:
    """Mathematical function for [Target Variable]
    
    Args:
        var1, var2, ...: Input variables (numpy arrays)
        params: Constants to be optimized (up to 10)
    
    Returns:
        Predicted output values
    """
    return params[0] * var1 + params[1] * var2**2 + params[2]
```

**Internal workflow:**
1. Extract equation function from code
2. Define loss: MSE = mean((y_pred - y_true)²)
3. Optimize params using BFGS (scipy.optimize.minimize)
4. Calculate metrics: MSE, NMSE, MAPE
5. Return formatted results with success/failure status

**Output format:**
```
MSE: 1.234e-03; NMSE: 2.345e-02; Mean absolute percentage error: 0.0567%
Success: The mean absolute percentage error is smaller than 0.1%.
```

**Key features:**
- MAX_NPARAMS = 10 (supports up to 10 parameters)
- BFGS optimizer (Quasi-Newton, efficient for smooth landscapes)
- Robust error handling (NaN, Inf, zero outputs)
- Clear success/failure feedback

### 3.3 Component 2: Experience Buffer

**Problem:** LLM context length limits ability to remember all explored equations

**Solution:** Heap-based experience buffer with top-K retrieval

**Structure:**
- Min-heap ordered by MAPE score
- Stores (equation_code, mape_score) pairs
- Deduplication to avoid redundant storage

**Usage flow:**

**Iteration 1:**
- Agent starts with empty context
- Explores equations: E₁ = [(eq₁, score₁), (eq₂, score₂), ...]
- All added to buffer H

**Iteration 2+:**
- Fetch top-K best equations from H (typically K=5)
- Provide as context: "Previously explored equations: ..."
- Agent sees what worked, proposes improvements
- Add new equations to buffer

**Benefits:**
1. Overcomes context limits (store unlimited, retrieve only best K)
2. Learning across iterations (agent sees successful patterns)
3. Continuous improvement (each iteration builds on best)
4. Efficient memory (O(log n) insertion, O(k log n) retrieval)

**Ablation results:**
- Without buffer: -6.21% to -13.43% performance drop
- Optimal K: 3-5 equations

### 3.4 Component 3: ReAct Framework

**Reason + Act paradigm**: Interleaves internal reasoning with external tool invocations

**Trajectory structure:**
```
(r₁, T₁, o₁), (r₂, T₂, o₂), ..., (r_k, T_k, o_k)
```

Where:
- **r_i**: Natural language reasoning (agent's thoughts)
- **T_i ⊆ {data_analyzer, equation_evaluator}**: Tools invoked
- **o_i**: Observation from tool execution

**Example trajectory** (Physics PO10 - Nonlinear Oscillator):

```
Turn 1:
r₁: "First, let's explore the data structure"
T₁: data_analyzer
Code: print(data_list[:5])
o₁: [[0.010, 16.543, 95.159], ...]

Turn 2:
r₂: "Let's check correlations to understand relationships"
T₂: data_analyzer
Code: print(f"Corr(accel, pos): {np.corrcoef(outputs, pos)[0,1]:.3f}")
o₂: Corr(accel, pos): -0.856

Turn 3:
r₃: "Strong negative correlation with position suggests spring force. Try harmonic oscillator."
T₃: equation_evaluator
Code: def equation(t, x, v, params): return -params[0] * x - params[1] * v
o₃: MAPE: 1234.5% - Failure

Turn 4:
r₄: "Linear damping not sufficient. Analyze residuals."
T₄: data_analyzer
Code: [residual vs v³ correlation analysis]
o₄: Corr(residual, v³): -0.921

Turn 5:
r₅: "Strong v³ correlation! Try cubic damping."
T₅: equation_evaluator
Code: def equation(t, x, v, params): return -params[0] * x - params[1] * v**3
o₅: MAPE: 0.0234% - Success!
```

### 3.5 Component 4: Long-Horizon Optimization

**Configuration:**
- **M**: Max turns per iteration (default: 25)
- **N**: Total iterations (default: 40)
- **Total budget**: ~1,000 LLM calls per problem

**Why 25 turns?**

Ablation study results:
- **10 turns**: Baseline performance
- **15 turns**: +8% improvement
- **25 turns**: +15-20% improvement ✓ (optimal)
- **40 turns**: +16% improvement (diminishing returns)

**Conclusion**: 25 turns optimal, use remaining budget for more iterations

**Typical turn breakdown:**
- Turns 1-5: Data exploration and statistical analysis
- Turns 6-10: Initial equation attempts based on domain knowledge
- Turns 11-15: Residual analysis and hypothesis refinement
- Turns 16-20: Advanced equation variants with learned insights
- Turns 21-25: Final validation and parameter interpretation

## 4. Детальный алгоритм

### Algorithm 1: SR-Scientist Inference Framework

```
Input: 
  - N: Number of iterations (default: 40)
  - M: Maximum turns per iteration (default: 25)
  - K: Number of equations to fetch from buffer (default: 5)
  - G₁: Initial MAPE goal (default: 0.1%)
  - termination_threshold: Stop when MAPE below this (default: 0.0001%)

Initialize:
  H ← empty_heap()  # Experience buffer (min-heap by MAPE)
  G_i ← G₁          # Current goal

Main Loop:
for i = 1 to N:
  # Generate candidate equations from LLM
  if i == 1:
    # First iteration: no context
    E_i ← LLM_Agent_Rollout(data, G_i, M, temperature=0.7)
  else:
    # Subsequent iterations: provide top-K context
    top_K_equations ← H.topk(K)
    E_i ← LLM_Agent_Rollout(data, G_i, M, temperature=0.7, context=top_K_equations)
  
  # Add explored equations to buffer
  for (equation, score) in E_i:
    H.push((score, equation))
  
  # Check stopping condition
  best_score ← H.topk(1).score
  if best_score < termination_threshold:
    break  # Success!
  
  # Update goal if reached
  if best_score < G_i:
    G_{i+1} ← max(best_score / 10, termination_threshold)
  else:
    G_{i+1} ← G_i

Output: H.topk(1)  # Return best equation
```

### LLM Agent Rollout (Single Iteration)

```
Input:
  - data: Training data accessible to agent
  - goal: Current MAPE goal
  - max_turns: Maximum turns (M)
  - context: Top-K equations from previous iterations (optional)

Initialize:
  messages ← [system_prompt, user_prompt(data, goal, context)]
  explored_equations ← []

Interaction Loop:
for turn = 1 to max_turns:
  # LLM generates reasoning + tool call
  response ← LLM_API_Call(messages, T=0.7, max_tokens=8192)
  messages.append(response)
  
  # Parse tool calls
  tool_calls ← Parse_Tool_Calls(response)
  
  if no tool_calls:
    break  # Agent finished
  
  # Execute tools
  for (tool_name, tool_input) in tool_calls:
    if tool_name == "data_analyzer":
      observation ← Execute_Data_Analyzer(tool_input, data)
    elif tool_name == "equation_evaluator":
      observation ← Execute_Equation_Evaluator(tool_input, data)
      # Track explored equation
      equation, mape ← Extract_Equation_And_Score(observation)
      explored_equations.append((equation, mape))
    
    messages.append(observation)
  
  # Check if goal reached
  if min(explored_equations, key=lambda x: x[1])[1] < goal:
    break  # Goal reached!

Output: explored_equations
```

## 5. Система промптов (Полные тексты из статьи)

### 5.1 System Prompt (Figure 13 - Complete)

```
Your goal is to determine the correct equation, implement it as a Python function, and optimize it until the mean absolute percentage error is less than 0.1%.

You should use the 'equation_evaluator' tool to evaluate the equation's goodness of fit and the 'data_analyzer' tool to write code for data analysis.

For the 'equation_evaluator', it is a code interpreter that wraps your function with evaluation code that:
1. Optimizes parameters using SciPy's BFGS algorithm
2. Calculates MSE, NMSE, and MAPE metrics
3. Returns success/failure status

The tool accepts Python function with this format:
- Function header must include all input variables and params argument
- Use params[0], params[1], ... params[9] for constants (MAX_NPARAMS = 10)
- Return numpy array of predicted outputs

For the 'data_analyzer' tool, it is a code interpreter that can run your data exploration code. You can access data via:
- input_data_str: JSON string of data
- data_list: Parsed list where each entry is [output, input1, input2, ...]

Example data access:
import json
data_list = json.loads(input_data_str)
print(data_list[:5])  # First 5 rows

IMPORTANT: You are forbidden from using Matplotlib or other plotting libraries.
```

### 5.2 User Prompt Template (Figure 14 - Complete)

```
Find the mathematical function skeleton that represents {TARGET_VARIABLE}, given data on {INPUT_VARIABLES}.

Follow these steps to solve the problem:

**1. Implement the Equation in Code**
* Based on your knowledge and analysis, identify the standard equation and implement it in code.
* Your equation will likely have one or more constants. Use elements from the 'params' list (e.g., 'params[0]', 'params[1]', 'params[2]') to represent these constants, as the 'equation_evaluator' tool is designed to optimize them. 
* Note that the 'params' list has a fixed size of 10 ('MAX_NPARAMS = 10'), so you can use up to 10 parameters in your model.

**2. Test, Analyze, and Refine**
* Evaluate the equation's goodness of fit using the 'equation_evaluator' tool.
* You need to pass the entire function, including the function header, to the tool.

Example:
def equation(x: np.ndarray, t: np.ndarray, v: np.ndarray, params: np.ndarray) -> np.ndarray:
    """ Mathematical function for {TARGET_VARIABLE}
    Args:
        x: A numpy array representing observations of {INPUT_VAR_1}.
        t: A numpy array representing observations of {INPUT_VAR_2}.
        v: A numpy array representing observations of {INPUT_VAR_3}.
        params: Array of numeric constants or parameters to be optimized
    Return:
        A numpy array representing {TARGET_VARIABLE} as the result
        of applying the mathematical function to the inputs.
    """
    output = params[0] * x + params[1] * t + params[2] * v + params[3]
    return output

* You can modify the function body, but the function header must remain unchanged.
* Your goal is to reduce the mean absolute percentage error to less than 0.1000%. Meeting this condition indicates that your equation is a good fit for the data.
* If this goal is not met, refine your equation in Python and observe its performance. You can write your own data exploration snippet and use the 'data_analyzer' tool to execute it, allowing you to inspect the data for potential relationships or anomalies.

**3. Submit Your Final Answer**
* Once you are confident your equation has met the condition, or if you conclude after numerous attempts that you cannot meet it, provide the completed Python function as your answer.
```

### 5.3 Context Prompt (Experience Buffer)

При iteration > 1, к user prompt добавляется:

```
--- Previously Explored Equations ---

Here are the top {K} performing equations from previous iterations:

Equation 1 (MAPE: {score_1}%):
def equation(...):
    return {equation_body_1}
Optimized parameters: [{param_values_1}]

Equation 2 (MAPE: {score_2}%):
def equation(...):
    return {equation_body_2}
Optimized parameters: [{param_values_2}]

...

These equations were previously explored. You can use them as inspiration, but try to improve upon them or explore different directions.

---

[Rest of user prompt follows]
```

### 5.4 Symbolic Accuracy Evaluation Prompt (Figure 15)

```
Given the ground truth mathematical expression A and the hypothesis B, determine if there exist any constant parameter values that would make the hypothesis equivalent to the given ground truth expression.

Let's think step by step. Explain your reasoning and then provide the final answer as:
{"reasoning": "Step-by-step analysis", "answer": "Yes/No"}

Ground Truth A: {ground_truth_equation}
Hypothesis B: {predicted_equation}
```

**Evaluation protocol:**
- Use GPT-OSS-120B as evaluator
- 10 independent evaluations per case
- If all 10 agree → accept LLM verdict
- If any disagreement → human expert review
- Measured consistency: 98.3% LLM-human agreement

### 5.5 Tool Call Classification Prompt (Figure 16)

```
You are an expert code analyst. Your task is to classify Python code snippets written by an AI agent that is trying to discover scientific equations from data.

Category Definitions:

- Data Statistics: Calculates statistical property (mean, variance, correlation, min, max)
  IMPORTANT: Respond as "Data Statistics: [STATISTIC_NAME]"

- Data Print: Prints raw data samples for initial inspection

- Residual Error Analysis: Evaluates equation by calculating residuals or error metrics

If code doesn't fit these categories, create a new, concise, specific category name.

Classify the following Python code snippet:
---
{code}
---
```

**Measured agreement**: 94.4% LLM-human on 54 cases

## 6. Reinforcement Learning Framework

### 6.1 Training Data Construction

**Hybrid Model-Based + Rule-Based Synthesis**

**Step 1: Equation Skeleton Generation**

Using Claude 4 Sonnet to generate skeletons:
- Each skeleton: ≥1 known term + ≥1 novel term
- Combined using addition
- Limited to 2-4 total terms
- Covers 4 domains: Chemistry, Biology, Physics, Material Science

**Anti-contamination measures:**
- Two authors independently review all skeletons
- Compare against LSR-Synth evaluation set
- Remove duplicates and similar equations
- Final agreement required

**Step 2: Parameter Instantiation**

LLM assigns physically meaningful values:
- Based on scientific context and significance
- Example: T₀ = 273.15 K (water triple point) for material science
- Human validation of all assignments

**Step 3: Data Point Generation**

**Static Systems** (Material Science):
```python
# 5000 uniform samples
T: [273 K, 573 K]  # Temperature range
ε: [0, 0.6]        # Strain range

# OOD test: 500 highest T points (extreme temperature)
# ID test: 500 random points
# Train: remaining 4000 points
```

**Dynamic Systems** (Chemistry, Biology, Physics):
```python
# Solve ODE using scipy.integrate.solve_ivp with RK45
t: [0, 60]  # Time range
5000 uniformly sampled time points

# OOD test: 500 highest t values (extended time)
# ID test: 500 random points
# Train: remaining 4000 points
```

**Step 4: Filtering**

Remove equations with:
- Scientifically anomalous data points
- Numerical instabilities
- Unsolvable ODEs

**Final Dataset**: 1024 training problems across 4 domains

### 6.2 Reward Design

**Log-Linear Reward Function** (Equation 2 in paper):

**R = clip((lg s_max - lg s) / (lg s_max - lg s_goal), 0, 1)**

Where:
- **s**: MAPE of best explored equation
- **s_max**: 100% (1.0) - maximum MAPE for non-zero reward
- **s_goal**: 0.1% (0.001) - target MAPE

**Why log-linear?**
- Continuous rewards (avoids sparsity)
- Encourages precision improvement
- Smooth gradient for RL optimization
- Tested alternative: stepwise function (performed worse)

**Stepwise alternative** (Equation 5, underperformed):
```
R = 1.0    if s < 0.001
    0.5    if 0.001 ≤ s < 0.01
    0.25   if 0.01 ≤ s < 0.1
    0.1    if 0.1 ≤ s < 1
    0.0    if s ≥ 1
```

### 6.3 Training Algorithm: GRPO

**Group Relative Policy Optimization** (modified - no KL penalty):

**J_GRPO(θ) = 𝔼[min(π_θ(o|q)/π_θ_old(o|q) × A, clip(π_θ(o|q)/π_θ_old(o|q), 1-ε, 1+ε) × A)]**

Where:
- Sample group {o₁, o₂, ..., o_G} from old policy
- Compute advantage A from group rewards
- Optimize with clipping parameter ε
- **NO KL penalty** → faster convergence + more exploration

**Training Infrastructure:**
- **Hardware**: 32× NVIDIA H200 GPUs
- **Framework**: verl (https://github.com/volcengine/verl)
- **Rollout engine**: SGLang (batch-level asynchronous)
- **Training engine**: FSDP (Fully Sharded Data Parallel)
- **Batch size**: 32 prompts, 8 rollouts per prompt
- **Temperature**: 1.0 (high for exploration)
- **Max response**: 10,240 tokens
- **Max turns per rollout**: 20
- **Training steps**: 60
- **KL coefficient**: 0.0 (no penalty)

**Training Dynamics:**
- Reward progressively increases, saturates around step 60
- Response length increases (agent learns long-horizon strategies)
- Tool usage improves (more data statistics, better analysis)

### 6.4 RL Training Results

**Qwen3-Coder-30B-A3B improvements:**

| Metric | Before RL | After RL | Improvement |
|--------|-----------|----------|-------------|
| Acc₀.₀₁ Overall | 32.30% | 40.92% | +8.62% (+26.7% relative) |
| Acc₀.₀₀₁ Overall | 16.02% | 20.69% | +4.67% (+29.2% relative) |
| Material Science | 81.33% | 85.33% | +4.00% |
| Chemistry | 22.22% | 37.38% | +15.16% |
| Biology | 22.22% | 29.17% | +6.95% |
| Physics | 18.18% | 25.00% | +6.82% |

**Other models tested** (Appendix A.3.4):

| Model | Before RL | After RL | Gain |
|-------|-----------|----------|------|
| Qwen3-8B | 15.50% | 20.93% | +5.43% |
| Qwen3-14B | 18.60% | 23.26% | +4.66% |
| Qwen3-32B | 29.46% | 39.53% | +9.07% |

**Conclusion**: RL training significantly improves performance across ALL model sizes!

## 7. Экспериментальная оценка

### 7.1 Benchmark Setup

**LSR-Synth Dataset:**
- **Total**: 129 problems
- **Chemistry**: 36 problems (reaction rates, concentrations)
- **Biology**: 24 problems (population dynamics, growth rates)
- **Physics**: 44 problems (oscillators, motion, forces)
- **Material Science**: 25 problems (stress-strain, thermal properties)

**Data splits per problem:**
- Training set (~4000 points): Accessible to SR method
- ID test set (500 points): Same distribution
- OOD test set (500 points): Extreme conditions

**Design to prevent memorization:**
- Known + Novel term combinations
- Authors manually verified uniqueness
- No overlap with common textbook equations

### 7.2 Evaluation Metrics

**Primary: Accuracy-to-Tolerance**

**Acc_τ = 𝟙[max_{1≤i≤N} |ŷᵢ - yᵢ|/|yᵢ| ≤ τ]**

- Discard 5% worst predictions (outlier handling)
- **Acc₀.₀₁**: 1% tolerance (main metric)
- **Acc₀.₀₀₁**: 0.1% tolerance (stringent)

**Why Acc_τ over R² and NMSE?**
- R²: Too easy, most methods achieve >0.99
- NMSE: Sensitive to outliers, hard to aggregate
- Acc_τ: Clear differentiation, robust aggregation ✓

**Secondary: Symbolic Accuracy**
- Checks if discovered equation ≡ ground truth
- Two-step: LLM evaluation (10 votes) + human review (if disagreement)
- 98.3% LLM-human agreement on unanimous cases

### 7.3 Baseline Methods

**Non-LLM Methods:**
1. **GPLearn**: GP library (population=500, generations=200)
2. **E2E**: Transformer direct prediction (max_points=200, trees=10)
3. **NeSymReS**: Pre-trained Transformer (points=500, beam=32)
4. **DSR**: RNN + RL search (samples=100K, batch=512)
5. **uDSR**: Unified framework (DSR + GP hybrid)
6. **PySR**: Julia backend GP (iterations=125, cycles=550, populations=15)

**LLM-Based Methods:**
1. **LaSR**: Library-Augmented SR with concept evolution
2. **LLM-SR**: LLM as equation proposer in GP

**Constraints:**
- Non-LLM: 100,000 equation candidates per problem
- LLM-based: 1,000 LLM calls, ≤1,000 candidates

### 7.4 Models Evaluated

**5 LLM backbones tested:**
1. **Qwen3-Coder-480B-A35B-Instruct** (FP8 quantization)
2. **GLM-4.5-Air** (FP8 quantization)
3. **GPT-OSS-120B**
4. **GPT-OSS-20B**
5. **Qwen3-Coder-30B-A3B-Instruct** (+ RL-trained version)

**Additional RL experiments:**
- Qwen3-8B, Qwen3-14B, Qwen3-32B

**Configuration:**
- Iterations: 40
- Turns per iteration: 25
- Initial MAPE goal: 0.1%
- Termination threshold: 0.0001%
- Temperature: 0.7
- Max completion length: 8,192 tokens
- Experience buffer: top-5 equations
- Experiments repeated: 3 times, average reported

## 8. Результаты и анализ

### 8.1 Main Results (Table 1 from paper)

**Best Overall Performer: GPT-OSS-120B**

| Metric | SR-Scientist | Best Baseline (PySR) | Improvement |
|--------|--------------|----------------------|-------------|
| Acc₀.₀₁ Overall | **63.57%** | 29.46% | **+34.11%** |
| Acc₀.₀₀₁ Overall | **49.35%** | 14.47% | **+34.88%** |

**By Domain (Acc₀.₀₁):**

| Domain | SR-Scientist | PySR | Improvement |
|--------|--------------|------|-------------|
| Material Science | 74.67% | 53.33% | +21.34% |
| Chemistry | **81.48%** | 25.93% | **+55.55%** |
| Biology | **66.67%** | 16.67% | **+50.00%** |
| Physics | 40.91% | 25.76% | +15.15% |

**Qwen3-Coder-480B** (Best on Material Science):

| Domain | Acc₀.₀₁ | Acc₀.₀₀₁ |
|--------|---------|----------|
| Overall | 49.09% | 24.55% |
| **Material Science** | **86.67%** | **69.33%** |
| Chemistry | 40.74% | 5.56% |
| Biology | 50.00% | 26.39% |
| Physics | 34.09% | 13.64% |

**Consistent superiority**: SR-Scientist with 4 out of 5 models outperforms ALL baselines by 6-35%

### 8.2 Symbolic Accuracy (Table 2)

Percentage of equations matching ground truth exactly:

| Method | Symbolic Accuracy |
|--------|-------------------|
| uDSR | 0.77% |
| PySR | 4.65% |
| LLM-SR (Qwen) | 5.43% |
| LLM-SR (GPT) | 4.65% |
| LLM-SR (GLM) | 5.43% |
| **SR-Scientist (GLM)** | **7.75%** ✓ |
| SR-Scientist (GPT) | 7.00% |
| SR-Scientist (Qwen) | 7.00% |

SR-Scientist achieves **highest symbolic accuracy** among all methods!

**Case Study: Physics PO10 & PO37** (Figure 5 - Nonlinear Oscillators):

Variables: ˙v(t) (acceleration), t (time), x (position), v (velocity)

**PO10 Ground Truth**: -ω₀² × x - γ × v³

**SR-Scientist Discovery**:
```python
def equation(t, x, v, params):
    return -params[0] * x - params[1] * v**3
# Optimized: params[0] ≈ ω₀², params[1] ≈ γ
# Symbolic match: YES ✓
```

**Baseline (more complex, less accurate)**:
```python
# LLM-SR result (example):
return -params[0]*x - params[1]*v**3 + params[2]*t*v + params[3]*x**2*v
# Extra terms, lower accuracy
```

**SR-Scientist advantages:**
- Correctly identifies core structure
- Accurate parameter values
- Provides interpretable trajectory showing derivation process

### 8.3 Out-of-Domain Generalization (Figure 2)

Performance on OOD test sets:

**Material Science**: ID→OOD performance **improves** (easier generalization to high T)
**Chemistry**: Slight degradation but still superior to baselines
**Biology**: Maintained strong performance
**Physics**: Consistent with ID performance

**Best OOD performer**: GPT-OSS-120B across all domains

**Key finding**: SR-Scientist maintains superiority on OOD data, demonstrating strong generalization

### 8.4 Robustness to Noise (Figure 3)

Tested with Gaussian noise: **σ ∈ {0.01, 0.05, 0.1}** added to training data

**GPT-OSS-120B results:**

| Noise Level | Acc₀.₀₁ | Performance Drop |
|-------------|---------|------------------|
| σ = 0.00 (clean) | 63.57% | baseline |
| σ = 0.01 | ~60% | -3.57% (minimal) |
| σ = 0.05 | ~55% | -8.57% |
| σ = 0.10 | ~45% | -18.57% |

**Key finding**: SR-Scientist consistently outperforms baselines at ALL noise levels, demonstrating superior robustness

### 8.5 RL Training Impact

**Qwen3-Coder-30B-A3B:**

| Metric | Before RL | After RL | Improvement |
|--------|-----------|----------|-------------|
| Overall Acc₀.₀₁ | 32.30% | 40.92% | **+8.62%** (+26.7% relative) |
| Overall Acc₀.₀₀₁ | 16.02% | 20.69% | **+4.67%** (+29.2% relative) |

**Improvements across ALL domains:**
- Material Science: 81.33% → 85.33% (+4.00%)
- Chemistry: 22.22% → 37.38% (+15.16%)
- Biology: 22.22% → 29.17% (+6.95%)
- Physics: 18.18% → 25.00% (+6.82%)

**Learned behaviors:**
- Increased data statistics usage
- Longer response generation (more thorough exploration)
- Better tool utilization patterns

## 9. Ablation Studies (Table 3)

### 9.1 Impact of Data Analyzer Tool

Performance drop **without data_analyzer** (w/o T₁):

| Model | With T₁ | Without T₁ | Drop |
|-------|---------|------------|------|
| GPT-OSS-120B | 63.57% | 35.66% | **-27.91%** |
| Qwen3-Coder-480B | 49.09% | 41.08% | -8.01% |
| GLM-4.5-Air | 48.32% | 46.51% | -1.81% |

**Key finding**: Data analysis capability CRUCIAL, especially for stronger models that can leverage it effectively

### 9.2 Impact of Experience Buffer

Performance drop **without experience buffer** (w/o experience):

| Model | With Buffer | Without Buffer | Drop |
|-------|-------------|----------------|------|
| GPT-OSS-120B | 63.57% | 57.36% | -6.21% |
| Qwen3-Coder-480B | 49.09% | 35.66% | **-13.43%** |
| GLM-4.5-Air | 48.32% | 37.21% | -11.15% |

**Key finding**: Experience buffer essential for continuous optimization across iterations

### 9.3 Effect of Turn Number (Figure 4)

Fixed ~1,000 LLM calls, trade-off between max turns and iterations:

| Max Turns | Performance | Notes |
|-----------|-------------|-------|
| 10 | Baseline | Insufficient exploration |
| 15 | +8% | Better but still limited |
| **25** | **+15-20%** | **Optimal** ✓ |
| 40 | +16% | Diminishing returns |

**Recommendation**: Use 25 turns per iteration, allocate remaining budget to more iterations

### 9.4 Tool Call Analysis (Figure 6)

**Distribution by model family:**

**Qwen/GLM families:**
- ~80% equation evaluation calls
- ~20% data analysis calls
  - Within data analysis: Higher % data statistics (mean, correlation, etc.)

**GPT-OSS models:**
- More residual error analysis (fine-grained feedback)
- Direct constant definition through data analysis
- Greater flexibility in tool usage

**After RL training** (Qwen3-Coder-30B):
- Increased data statistics usage ✓
- More advanced analysis patterns
- Better tool utilization (learned from experience)

## 10. Computational Cost and Efficiency

### 10.1 API Costs (Table 8)

| Model | Input Price | Output Price | Cost per Problem |
|-------|-------------|--------------|------------------|
| GPT-OSS-120B | $0.05/1M tokens | $0.25/1M tokens | **$0.25** |
| GPT-OSS-20B | $0.03/1M tokens | $0.15/1M tokens | **$0.10** |

*Note: Without cached tokens - withcaching even cheaper*

**Practical cost examples:**
- 100 problems with GPT-OSS-120B: $25
- 100 problems with GPT-OSS-20B: $10
- Acceptable for research scenarios

### 10.2 Inference Time

**GPT-OSS-120B deployed on 2×NVIDIA H100 GPUs:**
- 129 problems in batch mode
- Maximum wall-clock time: **5 hours**
- Acceptable for practical research usage

### 10.3 Training Cost

**Qwen3-Coder-30B RL training:**
- 32× NVIDIA H200 GPUs
- 60 training steps
- 1024 training problems
- Batch-level asynchronous rollouts

Training cost amortized across many inference runs

## 11. Technical Details

```yaml
ai_methods:
  agentic_framework:
    - ReAct paradigm (Reason + Act)
    - Code interpreter tools
    - Long-horizon optimization (25 turns × 40 iterations)
    - Experience buffer with heap management
    - Minimal human-defined pipelines
  
  reinforcement_learning:
    algorithm: Group Relative Policy Optimization (GRPO)
    reward_function: Log-linear (lg-based)
    training_problems: 1024 synthetic
    training_steps: 60
    hardware: 32× H200 GPUs
    framework: verl + SGLang + FSDP
    kl_penalty: 0.0 (no penalty for exploration)
  
  optimization:
    parameter_optimizer: BFGS (SciPy)
    metric: Mean Absolute Percentage Error (MAPE)
    initial_goal: 0.1% MAPE
    termination: 0.0001% MAPE
    adaptive_goal: Yes (10× stricter when reached)
  
  tools:
    data_analyzer:
      type: Code interpreter
      capabilities: [data inspection, statistics, residual analysis]
      restrictions: No visualization libraries
      timeout: 30 seconds
    
    equation_evaluator:
      type: Code interpreter + BFGS optimizer
      max_parameters: 10
      metrics: [MSE, NMSE, MAPE]
      success_threshold: 0.1% MAPE

data_types:
  training:
    - 1024 synthetic problems (4 domains)
    - 5000 points per problem
    - Train/ID test/OOD test splits
  
  evaluation:
    - LSR-Synth: 129 problems
    - Chemistry: 36
    - Biology: 24
    - Physics: 44
    - Material Science: 25
  
  characteristics:
    static_systems: Material Science (stress-strain-temperature)
    dynamic_systems: Chemistry/Biology/Physics (ODEs, time-series)
    noise_testing: Gaussian σ = 0.01, 0.05, 0.1
    ood_testing: Extreme conditions (high T, extended time)

platforms:
  inference:
    - LLM APIs (OpenAI, Anthropic, local deployments)
    - Python 3.8+ with NumPy, SciPy
    - Code interpreter environment
  
  training:
    - verl framework (https://github.com/volcengine/verl)
    - SGLang (rollout engine)
    - FSDP (Fully Sharded Data Parallel)
    - 32× NVIDIA H200 GPUs

system_architecture:
  agent_layer:
    component: LLM Agent
    framework: ReAct
    capabilities: [reasoning, tool invocation, hypothesis generation, feedback interpretation]
  
  tool_layer:
    data_analyzer:
      function: Data exploration
      implementation: Code interpreter
      access: Direct to training data
    
    equation_evaluator:
      function: Equation evaluation
      implementation: Code interpreter + BFGS
      output: MSE, NMSE, MAPE + success/failure
  
  memory_layer:
    experience_buffer:
      structure: Min-heap by MAPE score
      retrieval: Top-K best equations
      purpose: Overcome context length limits
  
  learning_layer:
    rl_pipeline:
      algorithm: GRPO
      reward: Log-linear function
      infrastructure: verl + SGLang + FSDP

performance_metrics:
  best_overall:
    model: GPT-OSS-120B
    acc_0_01: 63.57%
    acc_0_001: 49.35%
    improvement_vs_baseline: +34.11% absolute
  
  by_domain:
    material_science:
      best_model: Qwen3-Coder-480B
      acc_0_01: 86.67%
      acc_0_001: 69.33%
    
    chemistry:
      best_model: GPT-OSS-120B
      acc_0_01: 81.48%
      acc_0_001: 64.81%
      improvement: +55.55% vs PySR
    
    biology:
      best_model: GPT-OSS-120B
      acc_0_01: 66.67%
      acc_0_001: 43.05%
      improvement: +50.00% vs PySR
    
    physics:
      best_model: GPT-OSS-120B
      acc_0_01: 40.91%
      acc_0_001: 34.09%
  
  symbolic_accuracy:
    sr_scientist_best: 7.75%
    llm_sr_best: 5.43%
    pysr: 4.65%
    udsr: 0.77%
  
  rl_improvement:
    model: Qwen3-Coder-30B-A3B
    before: 32.30%
    after: 40.92%
    gain: +8.62% absolute (+26.7% relative)
  
  ablation_results:
    without_data_analyzer: -1.81% to -27.91% drop
    without_experience_buffer: -6.21% to -13.43% drop
    optimal_turns: 25 (vs 10: +15-20%)
  
  cost_efficiency:
    gpt_oss_120b: $0.25 per problem
    gpt_oss_20b: $0.10 per problem
    inference_time: 5 hours for 129 problems (2×H100)

validation:
  benchmark:
    name: LSR-Synth
    source: LLM-SRBench synthetic subset
    problems: 129
    domains: [Chemistry, Biology, Physics, Material Science]
    design: Known + novel terms (prevent memorization)
  
  tests_conducted:
    - In-domain accuracy (ID test set)
    - Out-of-domain generalization (OOD test set)
    - Noise robustness (σ = 0.01, 0.05, 0.1)
    - Symbolic accuracy (exact equation matching)
    - Ablation studies (tools, buffer, turns)
    - Model comparison (5 LLM backbones)
    - RL training validation (4 model sizes)
  
  comparison_methods:
    non_llm: [GPLearn, E2E, NeSymReS, DSR, uDSR, PySR]
    llm_based: [LaSR, LLM-SR]
    sr_scientist: 5 backbone LLMs tested
  
  results_summary:
    - Consistent superiority over all baselines
    - Strong OOD generalization maintained
    - Robust to noise (outperforms at all σ levels)
    - Highest symbolic accuracy achieved
    - Effective RL improvement demonstrated
    - Cost-effective for practical deployment
```

## 12. Lessons Learned

```yaml
achievements:
  performance:
    - Achieved 63.57% Acc₀.₀₁ (vs 29.46% best baseline) - 116% relative improvement
    - Outperformed baselines by 6-35% absolute margin across four science disciplines
    - Highest symbolic accuracy (7.75%) among all methods tested
    - Strong OOD generalization across all domains
    - Robust to noise up to σ=0.1 Gaussian
  
  methodology:
    - Successfully transformed LLMs into autonomous AI scientists
    - Demonstrated viability of minimal human-defined pipelines approach
    - Validated long-horizon optimization (25 turns optimal)
    - Proved experience buffer overcomes context length limitations
    - Developed end-to-end RL framework with 26.7% relative improvement
  
  technical:
    - Tool-wrapping approach enables autonomous agent behavior
    - ReAct framework effective for scientific reasoning
    - GRPO without KL penalty accelerates convergence
    - Log-linear reward function superior to stepwise
    - Data analysis capability critical (up to 27.91% impact)
  
  practical:
    - Cost-effective: $0.10-0.25 per problem (affordable for research)
    - Reasonable inference time: 5 hours for 129 problems
    - Open-source release enables community adoption
    - Trained model (SR-Scientist-30B) available for use

implications:
  scientific_discovery:
    - Opens new paradigm for autonomous equation discovery
    - Demonstrates LLMs can perform complete scientific workflows
    - Shows potential for accelerating discovery across disciplines
    - Provides interpretable trajectories offering insights to human scientists
    - Validates tool-augmented autonomous agents for scientific tasks
  
  agentic_ai_principles:
    - Confirms "Bitter Lesson" - minimal pipelines + computation > detailed procedures
    - Shows tool-augmented LLMs exhibit emergent scientific reasoning
    - Demonstrates long-horizon optimization crucial for complex tasks
    - Proves agents can learn and improve through self-experience (RL)
    - Establishes blueprint for autonomous AI scientists in other domains
  
  methodological_advances:
    - Experience buffer mechanism elegantly solves context limitations
    - Log-linear reward enables effective continuous-reward RL
    - GRPO without KL penalty: faster convergence, maintained quality
    - Hybrid data synthesis prevents memorization while enabling training
    - Tool-wrapping pattern generalizable to various code-based problems
  
  broader_impact:
    - Framework applicable beyond equation discovery
    - Long-horizon optimization pattern useful for complex reasoning
    - RL training pipeline extensible to other agentic systems
    - Demonstrates path toward AI systems contributing to scientific progress

challenges:
  technical:
    - Long-horizon optimization computationally intensive (1000 LLM calls/problem)
    - Context management requires sophisticated buffering
    - BFGS can fail on poorly-conditioned problems
    - Symbolic accuracy validation requires LLM + human review (labor intensive)
  
  model_dependency:
    - Performance highly dependent on base model capability
    - Weaker models (8B, 14B) struggle with complex analysis
    - Tool usage patterns vary significantly across model families
    - Not all models benefit equally from RL training
  
  evaluation:
    - Preventing memorization requires careful benchmark design
    - Multiple equivalent symbolic forms complicate accuracy measurement
    - Balancing functional accuracy vs symbolic accuracy challenging
    - OOD evaluation requires thoughtful extreme condition design
  
  scalability:
    - RL training requires significant compute (32×H200 GPUs)
    - Training data synthesis needs domain expertise and manual validation
    - Inference time scales with problem complexity
    - API costs accumulate with many problems
  
  domain_specific:
    - Physics problems (especially oscillators) more challenging than material science
    - Complex dynamical systems require more sophisticated approaches
    - Novel phenomena beyond training distribution remain challenging
    - Domain-specific knowledge integration still limited

limitations:
  - Symbolic accuracy still relatively low (7.75%) despite being highest
  - Physics domain performance (40.91%) lower than other domains
  - Requires extensive computational resources for training
  - Inference not real-time (hours for batch processing)
  - Limited to problems with <10 parameters
  - Cannot handle multi-output equations or systems of equations

impact_on_field:
  immediate:
    - "SR-Scientist establishes new state-of-the-art in symbolic regression"
    - "Demonstrates paradigm shift from LLMs as tools to LLMs as autonomous scientists"
    - "Validates minimal human-defined pipelines approach for scientific discovery"
    - "Open-source release enables broad research community adoption"
  
  long_term:
    - "Provides blueprint for autonomous AI scientists in domains beyond equation discovery"
    - "Shows path toward AI systems that formulate hypotheses, design experiments, validate discoveries"
    - "Demonstrates reinforcement learning can enhance scientific reasoning capabilities"
    - "Opens possibilities for human-AI collaborative scientific workflows"

future_directions:
  immediate:
    - Extend to partial differential equations (PDEs) and systems of ODEs
    - Apply to additional scientific domains (economics, ecology, engineering)
    - Integrate with experimental design and data collection systems
    - Develop multi-agent systems with specialized roles
  
  methodological:
    - Enhanced RL algorithms for scientific reasoning
    - Better reward shaping with physical constraints
    - Improved experience buffer (diversity-based selection)
    - Adaptive turn/iteration count based on complexity
  
  interpretability:
    - Methods to explain agent reasoning
    - Visualization of hypothesis evolution
    - Extract learned strategies from successful agents
    - Enable human trust in AI discoveries
  
  integration:
    - Connect to experimental validation systems
    - Integrate with scientific literature databases
    - Develop human-AI collaborative interfaces
    - Create automated publication pipelines
```

## 13. Key Insights from Paper

### 13.1 Autonomy Dramatically Improves Performance

Elevation от passive equation proposer к autonomous agent:
- Self-determined workflow
- Data-driven hypothesis generation
- Iterative refinement based on feedback
- Learning from experience across iterations

**Result**: 6-35% absolute improvement over fixed-pipeline methods

### 13.2 Long-Horizon Optimization Essential

25 turns optimal configuration provides:
- Time for thorough data exploration (5-7 turns)
- Multiple hypothesis testing cycles (10-15 turns)
- Residual-driven refinement (5-8 turns)  
- Final validation (2-3 turns)

**Result**: 15-20% improvement over shorter horizons

### 13.3 Data Analysis Capability Critical

Removing data_analyzer tool causes up to 27.91% drop:
- Stronger models leverage it more effectively
- Enables grounding hypotheses in actual data patterns
- Supports residual-driven iterative refinement

**Conclusion**: Data analysis ≠ optional, it's essential for success

### 13.4 Experience Buffer Enables Learning

Mechanism for continuous optimization:
- Stores all explored equations with scores
- Retrieves top-K for subsequent iterations
- Overcomes context length limitations elegantly

**Result**: 6.21-13.43% contribution to performance

### 13.5 RL Significantly Enhances Capabilities

GRPO training on 1024 problems:
- 26.7% relative improvement (Qwen3-30B)
- Consistent gains across all model sizes
- Learned behaviors: more data statistics, longer explorations
- Shows agents can evolve scientific reasoning abilities

### 13.6 Model Capability Matters

Different models exhibit distinct behaviors:
- **GPT-OSS**: Sophisticated tool usage, direct constant definition
- **Qwen/GLM**: More conservative, primarily statistical analysis
- **Smaller models**: Struggle to leverage data analyzer effectively

**Implication**: Base model quality crucial for agentic approaches

### 13.7 Cost-Effectiveness Achieved

Despite sophistication:
- $0.10-0.25 per problem (API costs)
- 5 hours for 129 problems (batch processing)
- Practical for real-world scientific applications
- RL training cost amortized across inference

## 14. Practical Applications

### 14.1 Scientific Research

**Materials Science:**
- Discover stress-strain relationships
- Thermal expansion coefficients
- Elastic modulus dependencies
- Fracture mechanics equations

**Chemistry:**
- Reaction kinetics
- Concentration dynamics
- Catalytic rate equations
- Temperature dependencies

**Biology:**
- Population growth models
- Epidemic dynamics
- Enzyme kinetics
- Metabolic rate equations

**Physics:**
- Motion equations
- Oscillator behaviors
- Force relationships
- Energy conservation forms

### 14.2 Research Workflow Integration

**Typical usage:**
1. Collect experimental data (measurements, observations)
2. Run SR-Scientist to discover candidate equations
3. Examine agent trajectories for scientific insights
4. Validate equations on new experiments
5. Refine based on validation results
6. Publish discovered relationships

### 14.3 Engineering Applications

- System identification for control
- Empirical model discovery from sensor data
- Performance modeling from benchmarks
- Design parameter optimization

### 14.4 Educational Use

- Demonstrate scientific discovery process
- Show hypothesis formation and testing
- Illustrate data-driven reasoning
- Interactive equation discovery for students

## 15. Reproducibility

### 15.1 Code and Models

**GitHub Repository**: https://github.com/GAIR-NLP/SR-Scientist
- Complete implementation
- Inference scripts
- Training code
- Evaluation scripts

**Pre-trained Models**:
- **SR-Scientist-30B**: Qwen3-Coder-30B with RL training
- Performance: 40.92% Acc₀.₀₁ (8.62% improvement over base)

### 15.2 Benchmark Data

**LSR-Synth**: Part of LLM-SRBench
- Repository: https://github.com/deep-symbolic-mathematics/llm-srbench
- 129 problems with train/ID/OOD splits
- Designed to prevent memorization

### 15.3 Configuration

All experiments use:
- Same hyperparameters across models
- 3 random seeds, results averaged
- Consistent evaluation protocol
- Fair comparison budget (1,000 LLM calls)

## 16. Citation and Acknowledgments

### 16.1 Citation

```bibtex
@article{xia2025srscientist,
  title={SR-Scientist: Scientific Equation Discovery With Agentic AI},
  author={Xia, Shijie and Sun, Yuhan and Liu, Pengfei},
  journal={arXiv preprint arXiv:2510.11661},
  year={2025},
  institution={Shanghai Jiao Tong University, SII, GAIR},
  note={Code: \url{https://github.com/GAIR-NLP/SR-Scientist}}
}
```

### 16.2 Funding

This work was funded by:
1. **National Natural Science Foundation of China** (Grant: 62476168)
2. **National High Technology Research and Development Program of China** (Grant: 2015AA015408)
3. **Shanghai Science and Technology Development Funds** (Grant: 14ZR1403200)
4. **AI for Science Program, Shanghai Municipal Commission of Economy and Informatization** (Grant: 2025-GZL-RGZN-BTBX-01013)

### 16.3 Acknowledgments

The authors thank:
- **Yan Ma**: Assistance with manuscript writing
- **Xuefeng Li**: Advice on RL infrastructure

## 17. Conclusion

SR-Scientist представляет собой фундаментальный прорыв в автономном открытии научных уравнений. Преобразуя Large Language Models из пассивных генераторов уравнений в автономных AI-учёных, система демонстрирует:

**Ключевые достижения:**
- 63.57% точность (vs 29.46% baseline) - **116% relative improvement**
- Высшая символическая точность (7.75%)
- Робастность к шуму и OOD данным
- Cost-effective практическое применение

**Методологические инновации:**
- Minimal human-defined pipelines principle
- Tool-augmented autonomous agents
- Long-horizon optimization framework
- Experience buffer для overcoming context limits
- GRPO RL для capability enhancement

**Влияние на область:**
- Устанавливает новый state-of-the-art в symbolic regression
- Демонстрирует путь к AI systems contributing to scientific progress
- Предоставляет concrete blueprint для autonomous AI scientists
- Открывает possibilities для accelerating discovery across disciplines

Как autonomous AI scientists продолжают эволюционировать, SR-Scientist provides foundational framework и empirical validation того, что LLMs могут не только assist scientists, но и independently formulate hypotheses, analyze data, design experiments, и validate discoveries - двигаясь ближе к AI systems как равноправным партнерам в научных исследованиях.

## 18. References

### Primary Publication
- **arXiv**: https://arxiv.org/abs/2510.11661
- **DOI**: 10.48550/arXiv.2510.11661
- **PDF**: https://arxiv.org/pdf/2510.11661.pdf

### Code and Models
- **GitHub**: https://github.com/GAIR-NLP/SR-Scientist
- **Model**: SR-Scientist-30B (Qwen3-Coder-30B + RL)

### Related Benchmarks
- **LLM-SRBench**: https://github.com/deep-symbolic-mathematics/llm-srbench
- **LSR-Synth**: Synthetic subset (129 problems)

### Related Work
- **PySR**: https://astroautomata.com/PySR/
- **LLM-SR**: https://github.com/deep-symbolic-mathematics/llm-srbench
- **LaSR**: https://github.com/trishullab/LibraryAugmentedSymbolicRegression.jl
- **verl Framework**: https://github.com/volcengine/verl

---

**Last Updated**: January 20, 2025  
**Version**: 2.0  
**Status**: Published (October 13, 2025)  
**Data Completeness**: Exceptional
