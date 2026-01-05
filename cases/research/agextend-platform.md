---
id: agextend-platform
slug: agextend-platform
entity_type: research
status: published
data_completeness: exceptional
last_researched: 2025-01-29
research_category: academic_institution
researcher: AI Assistant
version: 5.0
name: AgeXtend - Explainable AI Platform for Geroprotector Discovery
description: "AgeXtend is a multimodal, bioactivity-based, and biologically explainable AI-supported prediction platform developed by the Ahuja Lab at Indraprastha Institute of Information Technology Delhi (IIIT-Delhi) for discovering geroprotectors - compounds that can slow aging processes. Published in Nature Aging (December 2024), the platform consists of four interconnected modules: geroprediction (identifying geroprotectors), explainability (providing mechanistic insights), toxicity assessment, and target identification. Trained on 583 geroprotectors and 389 neutral compounds using Signaturizer bioactivity descriptors and SVM classifier, AgeXtend achieved 79.2% testing accuracy and 86.4% AUC-ROC in leave-one-out cross-validation. The platform screened ~1.1 billion compounds across 20 databases including small molecules, phytochemicals, and metabolites. AgeXtend successfully predicted known geroprotectors (metformin, taurine) even when excluded from training data and validated numerous predictions through yeast chronological lifespan assays (24 endogenous metabolites), C. elegans longevity assays (fadrozole, anastrozole), and human fibroblast senescence assays (deoxycholic acid, zymosterol). The explainability module links predictions to 9 aging hallmarks: genomic instability, telomere attrition, epigenetic alterations, loss of proteostasis, deregulated nutrient sensing, mitochondrial dysfunction, cellular senescence, stem cell exhaustion, and altered intercellular communication."
mission: To develop a multimodal, explainable AI platform that systematically identifies geroprotectors from vast chemical space, provides mechanistic insights into aging-related biological processes, assesses toxicity, and predicts protein targets to accelerate aging research and therapeutic development.
entity_data:
  name: AgeXtend Platform
  status: published
  objectives:
    - Develop multimodal bioactivity-based AI platform for geroprotector discovery
    - Screen vast chemical space (1.1+ billion compounds across 20 databases) for geroprotective potential
    - Provide explainable predictions linking compounds to 9 aging hallmarks
    - Evaluate ADMET properties through 15-model toxicity module
    - Identify potential protein targets using BindingDB database
    - Validate predictions experimentally in yeast, C. elegans, and human fibroblasts
    - Create publicly available Python package for community use
  start_date: 2023-10-27
  publication_date: 2024-12-03
  description: "Multimodal, bioactivity-based, explainable AI platform for systematic geroprotector discovery. Four-module architecture: (1) Geroprediction module - SVM classifier trained on 583 GPs + 389 neutral compounds using Signaturizer bioactivity descriptors (79.2% accuracy, 86.4% AUC-ROC, LOOCV); (2) Explainability module - 9 binary classifiers for aging hallmarks (genomic instability, telomere attrition, epigenetic alterations, loss of proteostasis, deregulated nutrient sensing, mitochondrial dysfunction, cellular senescence, stem cell exhaustion, altered intercellular communication); (3) Toxicity module - 15 models assessing ADMET properties; (4) Target module - protein target prediction using BindingDB. Screened ~1.1 billion compounds from 20 databases."
  methodology: "Binary classification using bioactivity-based features (Signaturizer v1.1.11) outperformed chemistry-based (Mordred, ECFP) and graph-based (ConvMol) descriptors. SVM classifier selected through 5-fold cross-validation. Feature selection via Boruta algorithm. Hyperparameter tuning with random grid search. Model stability confirmed by 10-fold cross-validation and LOOCV. Class imbalance handled using SMOTE. Stringent cut-off: 0.904 (vs default 0.5) to minimize false positives. Explainability module: 9 independent binary classifiers (SVM for AIC/CS/DNS/EA/LP, RF for GI, XGB for MD, ET for SCE/TA) trained on aging-process-specific datasets with no overlap to geroprediction training data. Toxicity module: 14 binary classifiers + 1 regression model for ADMET properties. Target module: Tanimoto similarity-based screening of BindingDB (2.4M protein-ligand interactions)."
  results: "Validation on 74 new GPs + 10 N compounds: 90.5% accuracy, 94.6% precision/recall. Successfully predicted metformin (0.65), taurine (0.70), N-acetyltaurine (0.80) as GPs when excluded from training. Yeast CLS assay: 24 endogenous metabolites tested, significant pro-longevity effects for d-erythrose 4-phosphate, succinyl-CoA, deoxycholic acid, d-ribulose 5-phosphate, 3-phospho-d-glycerate, l-ascorbic acid, putrescine. C. elegans lifespan assay: fadrozole (+10.8% maximum mean lifespan, p=0.01), anastrozole (+8.4%, p=0.03). Human fibroblast senescence assays: DCA and zymosterol reduced SA-β-gal+ cells under CPT-induced senescence. Microbiome analysis: age-negative gut taxa had significantly higher geroprediction scores (p=0.003), FIM-positive species showed higher scores (p=0.02). Screened 1,139,718,575 compounds identifying high-confidence GPs (probability ≥0.904) across chemical space."
  author_contributions:
    conceptualization:
      - Gaurav Ahuja
    methodology:
      - Gaurav Ahuja
      - Sakshi Arora
    computational_analysis:
      - Sakshi Arora
      - Aayushi Mittal
      - Subhadeep Duari
      - Sanjay Kumar Mohanty
      - Arushi Sharma
      - Saveena Solanki
      - Nikita Kapoor
      - Jeet Nanshi
      - Pushpendra Singh Gahlot
      - Shiva Satija
      - Vishakha Gautam
    software_development:
      - Sanjay Kumar Mohanty
      - Sakshi Arora
    experimental_yeast:
      - Aayushi Mittal
      - Subhadeep Duari
      - Anmol Kumar Sharma
      - Sakshi Arora
    experimental_celegans:
      - Sakshi Arora
      - Aayushi Mittal
      - Sonam Chauhan
      - Subhadeep Duari
    experimental_human_cells:
      - Sakshi Arora
    microbiome_analysis:
      - Sakshi Arora
      - Lavanya CB
      - Tarini Shankar Ghosh
    statistical_guidance:
      - Debarka Sengupta
    illustrations:
      - Aayushi Mittal
      - Sakshi Arora
      - Gaurav Ahuja
    writing:
      - Gaurav Ahuja
      - Sakshi Arora
  collaboration_period:
    start: 2023-10-27
    received_date: 2023-10-27
    accepted_date: 2024-10-25
    publication_date: 2024-12-03
taxonomy:
  geography: India
  ai_technology:
    - Explainable AI
    - Predictive ML/DL
  ai_approach:
    - Supervised Learning
  ai_architecture:
    - Predictive ML/DL
  ai_specialization:
    - Explainable AI
  primary_focus:
    - AI-Driven Drug Discovery
  aging_approach:
    - Target Discovery
    - Molecule Design
  target_biology:
    - General Aging/Longevity
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: academic_institution
  therapeutic_modality: []
organizations:
  - name: Indraprastha Institute of Information Technology Delhi
    role: primary
    org_type: institution
    legal_name: Indraprastha Institute of Information Technology Delhi (IIIT-Delhi)
    website: "https://www.iiitd.ac.in/"
    status: operational
    role_description: Primary research institution hosting Ahuja Lab (Department of Computational Biology)
    contribution_description: "Ahuja Lab at IIIT-Delhi's Department of Computational Biology developed the complete AgeXtend platform including all four modules (geroprediction, explainability, toxicity, target), led computational and experimental research (yeast, C. elegans, human cells), and published the work in Nature Aging. Institution provided research infrastructure, computational resources, and IT support. All 17 IIIT-Delhi authors from Department of Computational Biology except one collaborator from IIT Delhi."
    description: Public research university in New Delhi, India, focused on information technology and interdisciplinary research. Houses Department of Computational Biology where Ahuja Lab developed AgeXtend platform.
    focus: Information technology, AI/ML research, computational biology, aging research
  - name: Indian Institute of Technology Delhi
    role: collaborator
    org_type: institution
    legal_name: Indian Institute of Technology Delhi (IIT Delhi)
    website: "https://www.iitd.ac.in/"
    status: operational
    role_description: Collaborating institution
    contribution_description: "Parul Mehrotra from Kusuma School of Biological Sciences at IIT Delhi contributed to designing C. elegans and human cell culture experimental workflows"
    description: Premier engineering and technology institute in New Delhi, India
    focus: Engineering, technology, biological sciences
products:
  - name: AgeXtend Platform
    type: research_methodology
    status: published
    development_stage: Research / Preclinical
    description: "Multimodal, bioactivity-based, explainable AI platform for geroprotector discovery with four-module architecture: (1) Geroprediction Module - SVM binary classifier (583 GPs + 389 N compounds, Signaturizer descriptors, 79.2% accuracy, 86.4% AUC-ROC LOOCV, stringent cut-off 0.904); (2) Explainability Module - 9 independent binary classifiers for aging hallmarks (GI, TA, EA, LP, DNS, MD, CS, SCE, AIC) using SVM/RF/XGB/ET, no training data overlap with geroprediction; (3) Toxicity Module - 15 ADMET models (14 binary classifiers: AMES, MMP, CYP450 inhibitors, hepatotoxicity, HLM, hERG, DILI, BBB, Pgp-inhibitors/substrates; 1 regression: MRTD); (4) Target Module - Tanimoto similarity-based BindingDB screening (2.4M protein-ligand interactions, H.sapiens/R.norvegicus/M.musculus/S.cerevisiae). Available as Python package with Predictor (execute predictions on user compounds) and Browser (explore pre-computed results for 1.1B+ compounds from 20 databases) functionalities."
    components:
      - name: Geroprediction Module
        description: "Binary SVM classifier trained on bioactivity descriptors"
        technical_details: "Training: 583 GPs (DrugAge build 4, Geroprotectors.org) + 389 N compounds (literature). Features: Signaturizer v1.1.11 bioactivity descriptors (outperformed Mordred, ECFP 1024/2048, ConvMol graph descriptors). Algorithm: SVM. Feature selection: Boruta. Hyperparameters: Random grid search. Validation: 10-fold CV + LOOCV. Performance: 79.2% accuracy, 86.4% AUC-ROC (LOOCV), 90.5% accuracy on independent 74 GPs + 10 N, 94.6% precision/recall. Cut-off: 0.904 (stringent, zero false positives vs 0.5 default). Class balancing: SMOTE (proportion=0.8)."
      - name: Explainability Module
        description: "9 independent binary classifiers linking predictions to aging hallmarks with mechanistic insights"
        technical_details: "Hallmarks: GI (genomic instability), TA (telomere attrition), EA (epigenetic alterations), LP (loss of proteostasis), DNS (deregulated nutrient sensing), MD (mitochondrial dysfunction), CS (cellular senescence), SCE (stem cell exhaustion), AIC (altered intercellular communication). Classifiers: SVM (AIC, CS, DNS, EA, LP), RF (GI), XGB (MD), ET (SCE, TA). Training: Class 1 (negative influencers), Class 0 (positive/neutral), no overlap with geroprediction data. Performance: AUC 0.85-1.00 (LP: 0.85, CS: 0.91, DNS: 0.96, MD: 0.97, AIC: 0.97, EA: 0.99, TA/SCE/GI: 1.00). Features: SIRT activators, NF-κB inhibitors, HSP90 inhibitors, macroautophagy activators, farnesyltransferase inhibitors, stem cell proliferators, telomerase activators. SHAP: AIC, DNS, EA key drivers. Friedman H-statistic: crosstalk analysis (AIC-CS, MD-LP, CS-GI positive correlations). Tanimoto similarity search to known bioactives."
      - name: Toxicity Module
        description: "15 ADMET models assessing absorption, distribution, metabolism, excretion, toxicity properties"
        technical_details: "14 binary classifiers: AMES (mutagenicity, AUC 0.86), MMP disruption (mitochondrial toxicity, 0.92), CYP450 inhibition (CYP1A2: 0.94, CYP2C19: 0.90, CYP2C9: 0.92, CYP2D6: 0.93, CYP3A4: 0.93), hepatotoxicity (0.89), HLM stability (0.85), hERG blockers (0.99), DILI (drug-induced liver injury, 0.83), BBB penetration (0.96), Pgp-inhibitors (0.92), Pgp-substrates (0.91). 1 regression model: MRTD (maximum recommended therapeutic dose, decision tree regressor). Data source: vNN-ADMET datasets. Validated metformin toxicity consistent with literature (failed AMES, DILI; passed others)."
      - name: Target Module
        description: "Ligand-based protein target prediction using structural similarity"
        technical_details: "Database: BindingDB v2022 (2,407,381 protein-ligand interactions). Species coverage: H.sapiens, R.norvegicus, M.musculus, S.cerevisiae (61.3% of BindingDB). Method: Tanimoto similarity search identifying top 3 structurally similar ligands. Output: Top 3 ligand-protein pairs with similarity scores. Validation examples: mTORC1 inhibitors (53% hit rate), HSP90 inhibitors (100%), JAK1 inhibitors (45%), HDAC6 inhibitors (59%) correctly identified in top 3. Example predictions: Metformin targets (DPP4 100%, 5-HT3a 72%, C1S 66%), Taurine targets (S36A1 100%/93%, GABR1 93%), N-acetyltaurine targets (NEP 85%/84%/83%)."
    capabilities:
      - High-confidence geroprotector prediction (stringent cut-off 0.904 minimizes false positives)
      - Mechanistic explainability linking compounds to 9 aging hallmarks
      - Comprehensive ADMET toxicity profiling (15 models covering mutagenicity, hepatotoxicity, CYP450, BBB, etc)
      - Protein target identification from 2.4M experimentally validated interactions
      - Structural similarity search to known bioactive compounds per aging process
      - Crosstalk analysis between aging processes (Friedman H-statistic)
      - Large-scale screening capability (pre-computed 1.1B+ compounds from 20 databases)
      - Python package for custom compound screening
      - Browser for rapid search in pre-computed databases
    applications:
      - Ultra-large-scale screening of chemical space for geroprotectors (1.1B+ compounds)
      - Drug repurposing for aging interventions (DrugBank screening)
      - Endogenous metabolite analysis for anti-aging potential (HMDB, YMDB, ECMDB)
      - Microbiome-derived metabolite evaluation (gutMGene, microbiota production mapping)
      - Senomodulator identification and validation
      - Phytochemical and natural product screening (IMPPAT, FooDB, CMNPD, AfroDb)
      - Metabolic pathway analysis in aging (Aging Atlas integration)
      - Mechanistic hypothesis generation for aging research
      - Gut microbiome age association analysis
      - Frailty-protective metabolite identification
    technical_details:
      ai_methods: "Support Vector Machines (SVM), Random Forest (RF), XGBoost (XGB), Extra Trees (ET), Signaturizer v1.1.11 bioactivity descriptors, SMOTE for class balancing, Boruta feature selection, SHAP explainability analysis, Friedman H-statistic for interaction analysis, Decision Tree Regressor (MRTD), t-SNE dimensionality reduction"
      architecture: "Four sequential interconnected modules operating independently but linked: Geroprediction (binary classification) → Explainability (9 binary classifiers) → Toxicity (15 ADMET models) → Target (similarity search). Two user interfaces: Predictor mode executes full pipeline on query compounds; Browser mode enables rapid search in pre-computed database (1.1B+ compounds, 20 databases). Python package available via pip."
      training_data: "Geroprediction: 972 compounds (583 GPs from DrugAge build 4 + Geroprotectors.org, 389 N from literature, manual curation, duplicate/conflict removal). Independent validation: 84 compounds (74 GPs + 10 N from 60 recent articles). Explainability: 9 aging-process-specific datasets (class 0/1, no overlap with geroprediction, includes SIRT activators, NF-κB inhibitors, HSP90 inhibitors, mTOR activators, senescence inducers, stem cell proliferators, telomerase activators, farnesyltransferase inhibitors, macroautophagy activators). Toxicity: vNN-ADMET datasets. Targets: BindingDB v2022 (2.4M interactions, 61.3% from H.sapiens/R.norvegicus/M.musculus/S.cerevisiae)."
      performance_metrics: "Geroprediction: 79.2% testing accuracy, 86.4% AUC-ROC (LOOCV), 94.6% precision/recall (independent dataset), 90.5% accuracy (74 new GPs + 10 N). Age-ChEMBL (SIRT1/3/6 activators, mTORC1/HSP90/JAK1/HDAC6 inhibitors): median 0.84 geroprediction probability. DarkChem (biologically inert compounds): median 0.58 vs Age-ChEMBL 0.84 (p<0.001, Kolmogorov-Smirnov test). Excluded-from-training validation: Metformin 0.65, Taurine 0.70, N-acetyltaurine 0.80. Explainability: AUC 0.85-1.00 per hallmark. Toxicity: AUC 0.83-0.99 across 15 models. Outperforms previously reported geroprotector models."
      validation: "Independent dataset: 90.5% accuracy (74 GPs + 10 N from recent literature). Yeast CLS assay: 24 endogenous metabolites tested over 25 days (days 1,3,5,10,15,20,25), significant pro-longevity effects for d-erythrose 4-phosphate (ERP), succinyl-CoA (SCoA), deoxycholic acid (DCA), d-ribulose 5-phosphate (DRLP), 3-phospho-d-glycerate (DGA), l-ascorbic acid (AAA), putrescine (PUT). Growth assay (16h): no growth effects except ERP/PUT/fucosterol. C. elegans N2 lifespan assay: Fadrozole 100μM (+10.8% maximum mean lifespan, p=0.01, log-rank test, n=90), Anastrozole 100μM (+8.4%, p=0.03), Amyl acetate (non-significant). Human dermal fibroblasts senescence: DCA/zymosterol (1μM) reduced SA-β-gal+ cells under CPT-induced senescence (25nM, 48h), validated by Sudan Black B staining; DHAP negative control (no effect); DCA non-toxic, ZST toxic at 10μM. Microbiome meta-analysis: 5,388 gut profiles (13 datasets), age-negative taxa (n=43) significantly higher geroprediction scores vs age-positive (n=52) (p=0.003, Mann-Whitney U), FIM-positive species higher scores (p=0.02), negative correlation with telomere attrition (TA) (r=-0.32, p=0.025, Pearson). Species validated: Roseburia hominis, Dorea longicatena, Catenibacterium mitsuokai, Coprococcus comes."
links:
  - url: "https://www.nature.com/articles/s43587-024-00763-4"
    type: research_publication
    title: "Discovering geroprotectors through the explainable artificial intelligence-based platform AgeXtend"
    relevance: primary
    category: source
    description: "Primary publication in Nature Aging describing the AgeXtend platform, methodology, and results"
    authors:
      - Sakshi Arora
      - Aayushi Mittal
      - Subhadeep Duari
      - Sonam Chauhan
      - Nilesh Kumar Dixit
      - Sanjay Kumar Mohanty
      - Arushi Sharma
      - Saveena Solanki
      - Anmol Kumar Sharma
      - Vishakha Gautam
      - Pushpendra Singh Gahlot
      - Shiva Satija
      - Jeet Nanshi
      - Nikita Kapoor
      - Lavanya CB
      - Debarka Sengupta
      - Parul Mehrotra
      - Tarini Shankar Ghosh
      - Gaurav Ahuja
    publisher: Nature Aging
    publication_date: 2024-12-03
    metadata:
      doi: "10.1038/s43587-024-00763-4"
      journal: "Nature Aging"
      volume: "5"
      pages: "144-161"
      issue: "January 2025"
      received: "2023-10-27"
      accepted: "2024-10-25"
      published_online: "2024-12-03"
      publication_type: "Technical Report"
  - url: "https://github.com/the-ahuja-lab/AgeXtend/"
    type: github
    title: "AgeXtend GitHub Repository"
    relevance: primary
    category: source
    description: "Open-source repository containing AgeXtend platform code, documentation, installation instructions, and requirements. Free for academic use, commercial license required."
  - url: "https://pypi.org/project/AgeXtend"
    type: documentation
    title: "AgeXtend Python Package on PyPI"
    relevance: primary
    category: source
    description: "Official Python package distribution for AgeXtend platform, installable via pip"
  - url: "https://doi.org/10.5281/zenodo.8378959"
    type: database
    title: "AgeXtend Training Datasets and Code (Zenodo)"
    relevance: primary
    category: source
    description: "Training datasets and source code repository on Zenodo"
    metadata:
      doi: "10.5281/zenodo.8378959"
  - url: "https://doi.org/10.5281/zenodo.8379479"
    type: database
    title: "AgeXtend Additional Data and Supplementary Tables (Zenodo)"
    relevance: primary
    category: source
    description: "Supplementary tables, additional training dataset information, and endogenous metabolites data for yeast chronological assay"
    metadata:
      doi: "10.5281/zenodo.8379479"
  - url: "https://codeocean.com/capsule/0693261/tree"
    type: documentation
    title: "AgeXtend Workflow on CodeOcean"
    relevance: primary
    category: source
    description: "Executable AgeXtend workflow capsule on CodeOcean platform"
  - url: "https://www.iiitd.ac.in/"
    type: website
    title: "IIIT-Delhi Official Website"
    relevance: secondary
    category: reference
    description: "Official website of Indraprastha Institute of Information Technology Delhi"
  - url: "https://ngdc.cncb.ac.cn/aging"
    type: database
    title: "Aging Atlas Database"
    relevance: secondary
    category: source
    description: "Multi-omics database for aging biology used for metabolite enrichment analysis"
  - url: "http://eldermet.ucc.ie"
    type: database
    title: "ELDERMET Gut Microbiome Cohort"
    relevance: secondary
    category: source
    description: "Gut microbiome cohort study (214 samples) used for frailty index (FIM) association analysis"
  - url: "https://www.ebi.ac.uk/chembl"
    type: database
    title: "ChEMBL Database"
    relevance: secondary
    category: source
    description: "Bioactive compounds database used for validation (Age-ChEMBL: SIRT1/3/6 activators, mTORC1/HSP90/JAK1/HDAC6 inhibitors)"
  - url: "https://hmdb.ca"
    type: database
    title: "Human Metabolome Database (HMDB v5.0)"
    relevance: secondary
    category: source
    description: "Human metabolome database (~88K compounds) screened for geroprotectors"
  - url: "https://www.ymdb.ca"
    type: database
    title: "Yeast Metabolome Database (YMDB v2.0)"
    relevance: secondary
    category: source
    description: "Yeast metabolome database (~9K compounds) screened for geroprotectors"
  - url: "https://www.bindingdb.org"
    type: database
    title: "BindingDB v2022"
    relevance: primary
    category: source
    description: "Protein-ligand interaction database (2.4M interactions) used for target prediction module"
  - url: "https://www.metaboage.info"
    type: database
    title: "MetaboAge Database"
    relevance: secondary
    category: source
    description: "Aging-associated metabolites database (45 compounds) screened"
  - url: "https://www.metaboanalyst.ca"
    type: documentation
    title: "Metaboanalyst v5.0"
    relevance: secondary
    category: source
    description: "Metabolic pathway enrichment analysis tool used for over-representation analysis"
  - url: "https://biotransformer.ca"
    type: documentation
    title: "Biotransformer 3.0"
    relevance: secondary
    category: source
    description: "Software suite used to predict phase I and phase II metabolism of tested metabolites"
  - url: "https://sbi.postech.ac.kr/oasis2"
    type: documentation
    title: "Oasis2 Python Package"
    relevance: secondary
    category: source
    description: "Survival analysis package used for C. elegans lifespan data analysis (Kaplan-Meier, log-rank test)"
  - url: "https://imagej.net/software/fiji"
    type: documentation
    title: "ImageJ/Fiji Software"
    relevance: secondary
    category: source
    description: "Image analysis software used for quantification of senescence assays (SA-β-gal, SBB staining)"
people:
  - name: Gaurav Ahuja
    title: PhD
    person_type: pi
    role: Principal Investigator, Corresponding Author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    email: gaurav.ahuja@iiitd.ac.in
    responsibilities:
      - Overall project leadership
      - Study conception and design
      - Experimental workflow design (yeast, C. elegans, human cells)
      - Manuscript writing
      - Illustrations
    contribution_description: Principal Investigator who conceived the study, designed computational and experimental workflows, and led manuscript preparation
    expertise: Computational biology, AI in aging research, geroprotector discovery
  - name: Sakshi Arora
    person_type: researcher
    role: First Author (equal contribution)
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
      - TCS Research Scholar Program
    responsibilities:
      - Computational analysis workflow design
      - Data analysis and model building
      - Yeast experimental design and execution
      - C. elegans experimental design and execution
      - Human cell culture experiments
      - Microbiome data analysis
      - Manuscript writing
      - Illustrations
    contribution_description: Co-first author who designed and performed computational analyses, executed all experimental validations (yeast, C. elegans, human cells), conducted microbiome analysis, and co-wrote manuscript
  - name: Aayushi Mittal
    person_type: researcher
    role: First Author (equal contribution)
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    responsibilities:
      - Computational analysis workflow design
      - Data analysis
      - Yeast experimental workflow design and execution
      - C. elegans experimental workflow design and execution
      - Manuscript illustrations
    contribution_description: Co-first author who designed computational workflows, performed data analysis, conducted yeast and C. elegans experiments, and created illustrations
  - name: Subhadeep Duari
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis, conducted yeast and C. elegans experiments
  - name: Sonam Chauhan
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Conducted C. elegans experiments
  - name: Nilesh Kumar Dixit
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Designed human cell culture experimental workflows
  - name: Sanjay Kumar Mohanty
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    responsibilities:
      - Data analysis
      - AgeXtend Python package development
    contribution_description: Performed data analysis and built AgeXtend Python package
  - name: Arushi Sharma
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Saveena Solanki
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Anmol Kumar Sharma
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Conducted yeast experiments
  - name: Vishakha Gautam
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Pushpendra Singh Gahlot
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Shiva Satija
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Jeet Nanshi
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Nikita Kapoor
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Performed data analysis
  - name: Lavanya CB
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    contribution_description: Conducted microbiome data analysis
  - name: Debarka Sengupta
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    responsibilities:
      - Statistical guidance
    contribution_description: Provided statistical guidance for data analysis
    expertise: Statistical analysis, computational biology
  - name: Parul Mehrotra
    person_type: researcher
    role: Co-author
    affiliations:
      - Kusuma School of Biological Sciences, Indian Institute of Technology, New Delhi
    responsibilities:
      - Experimental design guidance (C. elegans, human cells)
    contribution_description: Designed C. elegans and human cell culture experimental workflows
  - name: Tarini Shankar Ghosh
    person_type: researcher
    role: Co-author
    affiliations:
      - Department of Computational Biology, IIIT-Delhi
    responsibilities:
      - Microbiome data analysis
    contribution_description: Conducted microbiome data analysis
    expertise: Microbiome analysis, computational biology
financials:
  - category: grant
    source: Department of Biotechnology, Ministry of Science & Technology, Government of India
    funding_type: Grant
    description: Research grant supporting AgeXtend platform development
    note: Funds Gaurav Ahuja lab
  - category: grant
    source: Science and Engineering Research Board (SERB)
    funding_type: Start-Up Research Grant
    description: Start-Up Research Grant SRG/2020/000232
    details:
      grant_number: SRG/2020/000232
      recipient: Gaurav Ahuja
  - category: grant
    source: European Molecular Biology Organization (EMBO)
    funding_type: Young Investigator Programme
    description: EMBO Young Investigator Programme research grant
    details:
      recipient: Gaurav Ahuja
  - category: grant
    source: IHUB Anubhuti
    funding_type: Research Grant
    description: Research grant supporting AgeXtend development
    details:
      grant_number: project grant/23
  - category: grant
    source: Indraprastha Institute of Information Technology-Delhi (IIIT-Delhi)
    funding_type: Intramural Start-up Grant
    description: Intramural start-up grant
    details:
      recipient: Gaurav Ahuja
  - category: grant
    source: Department of Science and Technology (DST), India
    funding_type: INSPIRE Faculty Grant
    description: INSPIRE faculty grant funding D. Sengupta lab
    details:
      recipient: Debarka Sengupta
  - category: grant
    source: TCS Foundation
    funding_type: Fellowship
    description: TCS Research Scholar Program sponsorship
    details:
      recipient: Sakshi Arora
      type: Research Scholar Fellowship
events:
  - event_date: 2023-10-27
    event_type: milestone
    title: "Manuscript Received by Nature Aging"
    description: "Research manuscript submitted to Nature Aging for peer review"
  - event_date: 2024-10-25
    event_type: milestone
    title: "Manuscript Accepted by Nature Aging"
    description: "Research manuscript accepted for publication after peer review"
  - event_date: 2024-12-03
    event_type: publication
    title: "AgeXtend Publication in Nature Aging"
    description: "Publication of AgeXtend platform research in Nature Aging, Volume 5, January 2025, pages 144-161"
    details:
      journal: "Nature Aging"
      doi: "10.1038/s43587-024-00763-4"
      volume: "5"
      pages: "144-161"
      issue_date: "January 2025"
      publication_type: "Technical Report"
      received_date: "2023-10-27"
      accepted_date: "2024-10-25"
      published_online: "2024-12-03"
partnerships:
  - partnership_date: 2023-01-01
    partnership_type: research
    description: "Research collaboration between IIIT-Delhi and IIT Delhi for experimental validation workflows"
    focus: "C. elegans lifespan assays and human fibroblast senescence assays experimental design"
    organizations:
      - name: Indraprastha Institute of Information Technology Delhi
        role: initiator
        role_description: "Primary research institution leading AgeXtend development"
      - name: Indian Institute of Technology Delhi
        role: collaborator
        role_description: "Collaborating institution providing experimental design expertise through Kusuma School of Biological Sciences"
---

# AgeXtend - Explainable AI Platform for Geroprotector Discovery

## Description

AgeXtend is a multimodal, bioactivity-based, and biologically explainable AI-supported prediction platform developed by the Ahuja Lab at Indraprastha Institute of Information Technology Delhi (IIIT-Delhi) for discovering nontoxic geroprotectors. Published in Nature Aging (December 2024), AgeXtend addresses limitations of existing approaches that rely solely on chemical information and lack biological explainability.

### Four-Module Architecture

**1. Geroprediction Module**: Binary SVM classifier trained on 583 experimentally validated geroprotectors and 389 neutral compounds using Signaturizer bioactivity descriptors. Achieved 79.2% testing accuracy and 86.4% AUC-ROC in leave-one-out cross-validation. Uses stringent probability cut-off of 0.904 (vs default 0.5) to minimize false positives.

**2. Explainability Module**: Nine independent binary classifiers linking predictions to aging hallmarks (genomic instability, telomere attrition, epigenetic alterations, loss of proteostasis, deregulated nutrient sensing, mitochondrial dysfunction, cellular senescence, stem cell exhaustion, altered intercellular communication). Each classifier trained on hallmark-specific datasets with no overlap to geroprediction training data. Achieves AUC 0.85-1.00 across hallmarks. Includes structural similarity search to known bioactives (SIRT activators, NF-κB inhibitors, HSP90 inhibitors, etc).

**3. Toxicity Module**: Fifteen ADMET models (14 binary classifiers + 1 regression) assessing mutagenicity (AMES), mitochondrial toxicity (MMP), CYP450 inhibition (5 isoforms), hepatotoxicity, liver microsomal stability (HLM), hERG blockers, drug-induced liver injury (DILI), blood-brain barrier (BBB) penetration, P-glycoprotein interactions, and maximum recommended therapeutic dose (MRTD). AUC 0.83-0.99 across models.

**4. Target Module**: Identifies potential protein targets through Tanimoto similarity-based screening of BindingDB database (2.4 million experimentally validated protein-ligand interactions from H. sapiens, R. norvegicus, M. musculus, S. cerevisiae). Returns top 3 similar ligands with protein targets and similarity scores. Validated with 45-100% hit rates for known aging-related targets (mTORC1, HSP90, JAK1, HDAC6).

### Large-Scale Screening and Validation

Screened 1,139,718,575 (~1.1 billion) unique compounds from 20 databases including small molecules (DrugBank, PubChem, ChEMBL, ZINC12, GDB13), phytochemicals (IMPPAT, FooDB, CMNPD, AfroDb), and metabolites (HMDB, YMDB, ECMDB, Aging Atlas, MetaboAge, gutMGene). Successfully predicted excluded known geroprotectors: metformin (0.65 probability), taurine (0.70), N-acetyltaurine (0.80).

Comprehensive experimental validation across three model systems: **(1) Yeast chronological lifespan assays**: 24 endogenous metabolites tested over 25 days, significant pro-longevity effects for d-erythrose 4-phosphate, succinyl-CoA, deoxycholic acid, d-ribulose 5-phosphate, 3-phospho-d-glycerate, l-ascorbic acid, and putrescine. **(2) C. elegans longevity assays**: Fadrozole extended maximum mean lifespan +10.8% (p=0.01), anastrozole +8.4% (p=0.03). **(3) Human fibroblast senescence assays**: Deoxycholic acid and zymosterol reduced SA-β-gal+ cells under camptothecin-induced senescence, validated by Sudan Black B staining.

### Microbiome-Aging Connection

Meta-analysis of 5,388 gut microbiome profiles (13 datasets, 107 species) revealed age-negative gut taxa had significantly higher geroprediction scores than age-positive taxa (p=0.003). FIM-positive species (frailty-protective) showed higher scores (p=0.02) with negative correlation to telomere attrition (r=-0.32, p=0.025). Validated healthy-aging-associated species: Roseburia hominis, Dorea longicatena, Catenibacterium mitsuokai, Coprococcus comes.

### Key Innovation

AgeXtend's bioactivity-based descriptors (Signaturizer) outperformed chemistry-based (Mordred, ECFP) and graph-based (ConvMol) features by integrating both chemical structure and biological context (protein interactions, pathways, disease associations). Validated compounds showed minimal structural similarity (<0.38 Tanimoto) but high bioactivity similarity to training data, demonstrating platform identifies geroprotectors by biological function rather than chemical structure alone.

## Mission

To develop a multimodal, explainable AI platform that systematically identifies geroprotectors from vast chemical space, provides mechanistic insights into aging-related biological processes, assesses toxicity comprehensively, and predicts protein targets, enabling acceleration of aging research and development of healthspan-promoting interventions.

## Project Information

**Received**: October 27, 2023  
**Accepted**: October 25, 2024  
**Published Online**: December 3, 2024  
**Print Publication**: Nature Aging Volume 5, January 2025, pages 144-161  
**DOI**: 10.1038/s43587-024-00763-4  
**Publication Type**: Technical Report  
**Status**: Published  
**Research Category**: Academic Institution (Department of Computational Biology, IIIT-Delhi)

## Technical Details

```yaml
ai_methods:
  - Support Vector Machines (SVM)
  - Random Forest (RF)
  - XGBoost (XGB)
  - Extra Trees Classifier (ET)
  - Decision Tree Regressor
  - Bioactivity-based descriptors (Signaturizer v1.1.11)
  - SMOTE for class imbalance handling
  - Boruta feature selection
  - SHAP (SHapley Additive exPlanations) for interpretability
  - Friedman H-statistic for interaction analysis
  - t-SNE for dimensionality reduction
  - Tanimoto similarity for structural comparison

training_datasets:
  geroprediction_module:
    total_compounds: 972
    geroprotectors: 583
    neutral_compounds: 389
    sources:
      - "DrugAge database (build 4, release 2021-11-20)"
      - "Geroprotectors.org database"
      - "Literature curation from ~60 recent articles"
    preprocessing: "Rigorous duplicate/conflict/low-confidence removal, species-specific bias elimination"
    independent_validation: 84 compounds (74 GPs + 10 N from recent publications)
  explainability_module:
    hallmarks_covered: 9
    datasets:
      genomic_instability: "Farnesyltransferase inhibitors (class 1) vs controls (class 0)"
      telomere_attrition: "Telomerase activators, telomere preservation compounds (class 1) vs controls (class 0)"
      epigenetic_alterations: "SIRT activators, HDAC inhibitors (class 1) vs controls (class 0)"
      loss_of_proteostasis: "HSP90 inhibitors, macroautophagy activators (class 1) vs controls (class 0)"
      deregulated_nutrient_sensing: "mTOR inhibitors, caloric restriction mimetics (class 1) vs mTOR activators (class 0)"
      mitochondrial_dysfunction: "Mitochondrial enhancers, PINK1/parkin pathway modulators (class 1) vs controls (class 0)"
      cellular_senescence: "Senolytics, senomorphics (class 1) vs senescence inducers (class 0)"
      stem_cell_exhaustion: "Stem cell proliferators, differentiation modulators (class 1) vs controls (class 0)"
      altered_intercellular_communication: "NF-κB inhibitors, NLRP3 inflammasome inhibitors, SIRT activators, CD38 inhibitors (class 1) vs controls (class 0)"
    data_integrity: "No overlap with geroprediction training data to prevent information leakage"
    total_compounds: 100763
  toxicity_module:
    models: 15
    classifiers: 14
    regression_models: 1
    source: "vNN-ADMET datasets"
  target_module:
    database: "BindingDB v2022"
    total_interactions: 2407381
    species_coverage: "H.sapiens, R.norvegicus, M.musculus, S.cerevisiae (61.3%)"

model_performance:
  geroprediction:
    algorithm: "Support Vector Machine (SVM)"
    features: "Signaturizer v1.1.11 bioactivity descriptors"
    feature_selection: "Boruta algorithm"
    hyperparameter_tuning: "Random grid search"
    class_balancing: "SMOTE (proportion=0.8)"
    cross_validation: "5-fold, 10-fold, LOOCV"
    accuracy: 79.2%
    auc_roc: 86.4%
    precision: 94.6%
    recall: 94.6%
    f1_score: "Reported in LOOCV"
    mcc: "Matthews Correlation Coefficient reported"
    cohens_kappa: "Reported in validation"
    cut_off_threshold: 0.904
    cut_off_rationale: "Stringent threshold to minimize false positives (vs default 0.5)"
    independent_validation: "90.5% accuracy on 74 GPs + 10 N"
  explainability:
    classifiers_by_hallmark:
      GI: "Random Forest (RF), AUC 1.00"
      TA: "Extra Trees (ET), AUC 1.00"
      EA: "Support Vector Machine (SVM), AUC 0.99"
      LP: "Support Vector Machine (SVM), AUC 0.85"
      DNS: "Support Vector Machine (SVM), AUC 0.96"
      MD: "XGBoost (XGB), AUC 0.97"
      CS: "Support Vector Machine (SVM), AUC 0.91"
      SCE: "Extra Trees (ET), AUC 1.00"
      AIC: "Support Vector Machine (SVM), AUC 0.97"
    shap_key_drivers:
      - "AIC (Altered intercellular communication)"
      - "DNS (Deregulated nutrient sensing)"
      - "EA (Epigenetic alterations)"
    interaction_analysis:
      method: "Friedman H-statistic"
      key_interactions:
        - "AIC-CS positive correlation"
        - "MD-LP positive correlation"
        - "CS-GI positive correlation"
        - "MD-CS positive correlation"
      most_prevalent_process: "MD (Mitochondrial dysfunction)"
  toxicity:
    auc_scores:
      hERG_blockers: 0.99
      BBB_penetration: 0.96
      CYP1A2_inhibition: 0.94
      CYP2D6_inhibition: 0.93
      CYP3A4_inhibition: 0.93
      CYP2C9_inhibition: 0.92
      MMP_disruption: 0.92
      Pgp_inhibitor: 0.92
      Pgp_substrate: 0.91
      CYP2C19_inhibition: 0.90
      hepatotoxicity: 0.89
      AMES_mutagenicity: 0.86
      HLM_stability: 0.85
      DILI: 0.83
    regression_model:
      MRTD: "Decision tree regressor"
  target:
    hit_rates:
      mTORC1: 53%
      HSP90: 100%
      JAK1: 45%
      HDAC6: 59%
    method: "Tanimoto similarity, top 3 ligand-protein pairs"

databases_screened:
  total_compounds: 1139718575
  count: 20
  databases:
    - name: "AfroDb"
      compounds: 304
      description: "African medicinal plants"
    - name: "Aging Atlas v1.0"
      compounds: 70
      description: "Age-associated metabolites"
    - name: "ChEMBL"
      compounds: 51000
      description: "Bioactive compounds"
    - name: "ChemBridge"
      compounds: 14
      description: "Screening compounds"
    - name: "ChemDiv BBlocks"
      compounds: 1000
      description: "Building blocks"
    - name: "CMNPD v1.0"
      compounds: 5000
      description: "Comprehensive Marine Natural Products Database"
    - name: "DSSTox v2021"
      compounds: 63000
      description: "Toxicology database"
    - name: "DDPEDB"
      compounds: 802
      description: "Dr. Duke's Phytochemical and Ethnobotanical Databases"
    - name: "ECMDB v2.0"
      compounds: 1000
      description: "E. coli Metabolome Database"
    - name: "FooDB v1.0"
      compounds: 6000
      description: "Food metabolite database"
    - name: "GDB13"
      compounds: 16000000
      description: "Generated Database"
    - name: "gutMGene"
      compounds: 72
      description: "Gut microbe-derived metabolites"
    - name: "HMDB v5.0"
      compounds: 88000
      description: "Human Metabolome Database"
    - name: "IMPPAT 2.0"
      compounds: 4000
      description: "Indian Medicinal Plants, Phytochemistry And Therapeutics"
    - name: "MetaboAge"
      compounds: 45
      description: "Aging-associated metabolites"
    - name: "MolData v1.1.0"
      compounds: 13000
      description: "Molecular data"
    - name: "PubChem"
      compounds: 2500000
      description: "Public chemistry database (downloaded 2022-10-21)"
    - name: "RepoHub"
      compounds: 370
      description: "Drug Repurposing Hub (release 2020-03-24)"
    - name: "YMDB v2.0"
      compounds: 9000
      description: "Yeast Metabolome Database"
    - name: "ZINC12"
      compounds: 500000
      description: "ZINC database"

software_dependencies:
  python: "3.8+"
  core_libraries:
    - "Signaturizer v1.1.11 - bioactivity descriptors"
    - "RDKit v2022.3.1 - cheminformatics"
    - "OpenBabel v3.0.0 - SMILES conversion"
    - "scikit-learn v1.2.1 - machine learning"
    - "DeepChem v2.6.2 - graph descriptors"
    - "smote_variants v0.4.0 - SMOTE algorithm"
    - "Boruta v0.3 - feature selection"
    - "ChemmineR v3.46.0 - functional group analysis"
  analysis_tools:
    - "Metaboanalyst v5.0 - metabolic pathway enrichment"
    - "Biotransformer 3.0 - metabolism prediction"
    - "bayestestR v0.11.5 - AUC calculation"
    - "ImageJ/Fiji - microscopy quantification"
  package_distribution:
    - "PyPI: https://pypi.org/project/AgeXtend"
    - "GitHub: https://github.com/the-ahuja-lab/AgeXtend"
    - "Zenodo: https://doi.org/10.5281/zenodo.8378959"
    - "CodeOcean: https://codeocean.com/capsule/0693261/tree"

infrastructure:
  description: "Two-component architecture for flexible usage"
  components:
    - name: "Predictor"
      description: "Execute full AgeXtend pipeline (geroprediction → explainability → toxicity → target) on user-supplied compounds"
      functionality: "Custom compound screening, full SMILES-to-prediction workflow"
    - name: "Browser"
      description: "Rapid search in pre-computed AgeXtend results for 1.1B+ compounds from 20 databases or user-prescreened in-house databases"
      functionality: "Quick lookup of pre-computed predictions, comprehensive HTML reports"

system_architecture:
  overview: "Four-module sequential architecture with bioactivity-based feature representation"
  module_flow: "Query compound → Geroprediction → Explainability → Toxicity → Target"
  components:
    - name: "Module 1: Geroprediction"
      type: "Binary classifier"
      algorithm: "SVM"
      input: "Signaturizer bioactivity descriptors (926 features after Boruta selection)"
      output: "Geroprotection probability (0-1), binary classification (GP/N)"
      training: "583 GPs + 389 N, SMOTE balancing, 10-fold CV"
      performance: "79.2% accuracy, 86.4% AUC-ROC (LOOCV)"
    - name: "Module 2: Explainability"
      type: "9 independent binary classifiers"
      algorithms: "SVM (5 hallmarks), RF (1), XGB (1), ET (2)"
      input: "Geroprediction output + Signaturizer descriptors"
      output: "Probability scores for 9 aging hallmarks, structural similarity to known bioactives"
      training: "Hallmark-specific datasets (class 0/1), no geroprediction overlap"
      performance: "AUC 0.85-1.00 per hallmark"
    - name: "Module 3: Toxicity"
      type: "15 ADMET models (14 classifiers + 1 regressor)"
      algorithms: "Various classifiers per toxicity endpoint"
      input: "Explainability output + Signaturizer descriptors"
      output: "14 binary toxicity predictions + MRTD dose estimate"
      training: "vNN-ADMET datasets per endpoint"
      performance: "AUC 0.83-0.99 across 15 models"
    - name: "Module 4: Target"
      type: "Similarity-based search"
      algorithm: "Tanimoto similarity"
      database: "BindingDB v2022 (2.4M interactions)"
      input: "Query compound structure"
      output: "Top 3 similar ligands with protein targets and similarity scores"
      species_filter: "H.sapiens, R.norvegicus, M.musculus, S.cerevisiae"

technical_workflow:
  model_development:
    - step: "Data collection"
      description: "Compile GPs, N compounds, hallmark-specific datasets, ADMET datasets from authenticated sources"
      details: "Manual curation, cross-verification, duplicate/conflict/low-confidence removal"
    - step: "Feature extraction"
      description: "Convert compounds to Canonical SMILES (OpenBabel), compute descriptors"
      options_tested: "Chemistry (Mordred, ECFP 1024/2048), Graph (ConvMol, PMG, MolGraphConv), Bioactivity (Signaturizer)"
      best_performer: "Signaturizer bioactivity descriptors"
    - step: "Class balancing"
      description: "Handle imbalanced datasets using SMOTE algorithm (proportion=0.8)"
    - step: "Classifier selection"
      description: "Test 10 classifiers (LR, SVM, GBC, RF, GNB, KNN, ET, SGD, XGB, MLP) via 5-fold CV"
      best_performers: "SVM (geroprediction, 5 hallmarks), RF (GI), XGB (MD), ET (SCE, TA)"
    - step: "Feature selection"
      description: "Apply Boruta algorithm to identify most influential features"
      result: "Selected features per module documented in Extended Data Fig. 3c"
    - step: "Hyperparameter tuning"
      description: "Random grid search to optimize classifier hyperparameters"
    - step: "Model validation"
      description: "10-fold cross-validation + LOOCV for stability confirmation"
    - step: "Threshold optimization"
      description: "Calculate optimal cut-off (0.904) achieving zero false positives across 10 folds"
    - step: "Final training"
      description: "Train on complete dataset with best hyperparameters and selected features"
  prediction_workflow:
    - step: "Input compound"
      description: "User provides compound as SMILES string"
    - step: "Feature extraction"
      description: "Compute Signaturizer bioactivity descriptors (926 signatures)"
    - step: "Geroprediction"
      description: "SVM classifier predicts GP probability, binary classification if ≥0.904"
    - step: "Explainability"
      description: "9 classifiers predict probabilities for aging hallmarks, Tanimoto similarity to known bioactives"
    - step: "Toxicity assessment"
      description: "15 ADMET models evaluate mutagenicity, hepatotoxicity, CYP450 inhibition, BBB, etc"
    - step: "Target prediction"
      description: "Search BindingDB for top 3 structurally similar ligands, output protein targets"
    - step: "Report generation"
      description: "Comprehensive HTML report with predictions, explanations, toxicity profile, targets"

chemical_representation:
  format: "Canonical SMILES (OpenBabel v3.0.0)"
  bioactivity_descriptors:
    name: "Signaturizer v1.1.11"
    dimension: 926
    advantages:
      - "Integrates chemical information (functional groups, scaffolds, physicochemistry)"
      - "Integrates biological information (protein-protein interactions, chemical-protein interactions, signaling pathways, diseases, toxicology, therapeutic areas)"
      - "Holistic compound representation beyond chemistry alone"
      - "Outperformed chemistry-based (Mordred, ECFP) and graph-based (ConvMol) descriptors"
    comparison_chemistry_based:
      Mordred: "AUC 0.86"
      ECFP_2048: "AUC 0.86"
      ECFP_1024: "AUC 0.85"
      ConvMol_graph: "AUC 0.83"
      Signaturizer_bioactivity: "AUC 0.90"

data_types:
  - Bioactivity data from experimentally validated geroprotectors
  - Small molecule structures (SMILES)
  - Phytochemical data (IMPPAT, FooDB, CMNPD, AfroDb, DDPEDB)
  - Human metabolites (HMDB v5.0, Aging Atlas, MetaboAge)
  - Microbial metabolites (YMDB v2.0, ECMDB v2.0, gutMGene)
  - Drug databases (DrugBank, RepoHub, PubChem, ChEMBL)
  - Protein-ligand interaction data (BindingDB v2022)
  - ADMET toxicity data (vNN-ADMET)
  - Gut microbiome profiles (5,388 profiles, 13 datasets, 107 species)
  - Aging Atlas metabolite enrichment data
  - ELDERMET gut microbiome FIM associations

platforms:
  - Python 3.8+
  - Signaturizer v1.1.11
  - RDKit v2022.3.1
  - OpenBabel v3.0.0
  - scikit-learn v1.2.1
  - DeepChem v2.6.2
  - smote_variants v0.4.0
  - Boruta v0.3
  - ChemmineR v3.46.0

performance_metrics:
  scale:
    compounds_screened: 1139718575
    databases: 20
    training_compounds: 972
    validation_compounds: 84
    yeast_metabolites_tested: 24
    celegans_drugs_tested: 3
    human_fibroblast_metabolites: 3
  geroprediction_accuracy:
    loocv: "79.2% accuracy, 86.4% AUC-ROC"
    independent: "90.5% accuracy (74 GPs + 10 N)"
    precision_recall: "94.6% / 94.6%"
  validation_highlights:
    excluded_known_gps:
      metformin: 0.65
      taurine: 0.70
      n_acetyltaurine: 0.80
    age_chembl_median: 0.84
    darkchem_median: 0.58
    comparison_significance: "p<0.001 (Kolmogorov-Smirnov)"
  experimental_validation:
    yeast_cls:
      metabolites_tested: 24
      significant_effects: "ERP, SCoA, DCA, DRLP, DGA, AAA, PUT"
      assay_duration: "25 days"
      timepoints: "Days 1,3,5,10,15,20,25"
      replicates: 8
    celegans_lifespan:
      drugs_tested: 3
      significant:
        - drug: "Fadrozole 100μM"
          effect: "+10.8% maximum mean lifespan"
          p_value: 0.01
        - drug: "Anastrozole 100μM"
          effect: "+8.4% maximum mean lifespan"
          p_value: 0.03
      replicates: 90
      strain: "N2"
      test: "Log-rank test"
    human_fibroblasts:
      senescence_model: "CPT-induced (25nM, 48h)"
      metabolites_tested: 3
      positive_results:
        - "DCA (1μM): Reduced SA-β-gal+ cells, non-toxic"
        - "Zymosterol (1μM): Reduced SA-β-gal+ cells, toxic at 10μM"
      negative_control: "DHAP (no effect on senescence)"
      positive_control: "Azithromycin (100μM, senolytic)"
      assays: "SA-β-gal staining, Sudan Black B staining"
      cell_line: "Human dermal fibroblasts (Lonza NHDF-Ad, CC-2511)"
      replicates: 10
  microbiome_analysis:
    gut_profiles: 5388
    datasets: 13
    species_analyzed: 107
    age_threshold: "≥60 years"
    age_negative_taxa: 43
    age_positive_taxa: 52
    geroprediction_score_difference: "p=0.003 (Mann-Whitney U)"
    fim_analysis:
      cohort: "ELDERMET"
      samples: 214
      fim_positive_higher_scores: "p=0.02"
      ta_correlation: "r=-0.32, p=0.025 (Pearson)"
    validated_species:
      - "Roseburia hominis"
      - "Dorea longicatena"
      - "Catenibacterium mitsuokai"
      - "Coprococcus comes"

validation:
  method: "Multi-organism experimental validation: yeast CLS, C. elegans lifespan, human fibroblast senescence assays"
  results: "High validation rate across all experimental systems. Geroprediction module: 90.5% accuracy on independent 74 GPs. Yeast: 24 metabolites, majority showed pro-longevity effects. C. elegans: 2/3 drugs significantly extended lifespan. Human fibroblasts: 2/2 predicted senomodulators reduced senescence markers. Microbiome: Age-negative taxa significantly enriched for geroprotective metabolite producers."
```

## Scientific Background

```yaml
aging_biology:
  hallmarks_of_aging:
    count: 12
    established_hallmarks:
      - genomic_instability: "DNA damage, repair defects"
      - telomere_attrition: "Telomere shortening with cell division"
      - epigenetic_alterations: "Changes in DNA methylation, histone modifications"
      - loss_of_proteostasis: "Protein misfolding, aggregation, impaired quality control"
      - deregulated_nutrient_sensing: "Dysregulation of mTOR, AMPK, insulin/IGF-1 signaling"
      - mitochondrial_dysfunction: "Impaired oxidative phosphorylation, increased ROS"
      - cellular_senescence: "Accumulation of senescent cells with SASP"
      - stem_cell_exhaustion: "Decline in stem cell function and regenerative capacity"
      - altered_intercellular_communication: "Dysregulated cell-cell communication, inflammation"
      - disabled_macroautophagy: "Impaired autophagy and cellular recycling"
      - dysbiosis: "Altered microbiome composition"
      - chronic_inflammation: "Age-related chronic inflammatory state (inflammaging)"
    note: "AgeXtend explainability module covers 9 of 12 hallmarks (excludes dysbiosis due to unavailable training data, disabled macroautophagy/chronic inflammation due to tight association with other hallmarks)"
  metabolism_aging_connection:
    principle: "Cellular metabolism is intricately connected to nearly all aging hallmarks"
    metabolic_pathways: "Metabolic pathways and their byproducts influence aging processes"
    known_geroprotective_metabolites:
      - "Coenzyme Q10: Modulates mitochondrial function"
      - "Carnosine: Antioxidant, anti-glycation"
      - "Taurine: Multi-hallmark effects (identified by AgeXtend)"
      - "NAD+: Supports sirtuins, DNA repair, mitochondrial health"
    metabolite_cooperation: "Functional cooperation via metabolite exchanges among aging cells (Correia-Melo et al.)"

geroscience_context:
  definition: "Systematic analysis of multidimensional aging processes and their interconnections"
  omics_technologies:
    - "Genomics: Genetic factors in aging"
    - "Transcriptomics: Gene expression changes with age"
    - "Epigenomics: Epigenetic alterations"
    - "Metabolomics: Metabolic shifts and metabolite roles"
    - "Proteomics: Protein expression and modifications"
    - "Pharmacogenomics: Drug-gene interactions"
    - "Metagenomics: Microbiome composition and function"
  intervention_approaches:
    - "Genetic manipulation: Gene knockouts, overexpression"
    - "Epigenetic modification: DNA methylation, histone editing"
    - "Pharmacological intervention: Small molecules, geroprotectors"

geroprotectors:
  definition: "Compounds that slow aging processes, extend lifespan, and improve healthspan"
  known_examples:
    metformin:
      status: "Leading longevity drug candidate"
      clinical_trial: "Phase IV trials for anti-aging effects"
      agextend_prediction: 0.65
      predicted_mechanisms: "Loss of proteostasis (LP), Stem cell exhaustion (SCE), Telomere attrition (TA)"
      predicted_targets: "DPP4 (100%), 5-HT3a (72%), C1S (66%)"
      toxicity: "Failed AMES (mutagenicity), DILI; passed other 13 assessments (consistent with literature)"
    taurine:
      source: "Endogenous metabolite, dietary supplement"
      agextend_prediction: 0.70
      predicted_mechanisms: "Loss of proteostasis (LP), Stem cell exhaustion (SCE), Telomere attrition (TA)"
      predicted_targets: "S36A1 (100%, 93%), GABR1 (93%)"
      toxicity: "Passed all 15 ADMET assessments"
      experimental_evidence: "Shown to extend lifespan in multiple species"
  intervention_strategies:
    - "Enhancing genomic stability (DNA damage prevention, improved DNA repair)"
    - "Telomerase activation"
    - "Metabolic reprogramming for longevity"
    - "Multi-hallmark targeting for comprehensive intervention"

explainable_ai:
  challenge: "Traditional ML black-box approaches lack reasoning for predictions"
  agextend_solution:
    - "Explainability module links predictions to 9 aging hallmarks with probability scores"
    - "Structural similarity search to known bioactives per hallmark (e.g., SIRT activators, HSP90 inhibitors)"
    - "SHAP analysis identifies key feature contributions"
    - "Friedman H-statistic reveals crosstalk between aging processes"
  benefits:
    - "Transparent mechanism of action predictions"
    - "Identifiable protein targets from validated interactions"
    - "Interpretable toxicity assessments (15 ADMET properties)"
    - "Hypothesis generation for downstream research"
  biological_explainability:
    advantage: "Returns biologically relevant information (aging processes, protein targets) not just chemical features"
    validation: "CS module predictions (DCA, zymosterol as senomodulators) confirmed by SA-β-gal and SBB assays"

chemical_space_exploration:
  scale: "1,139,718,575 compounds (~1.1 billion)"
  diversity:
    - "Small molecules: DrugBank, RepoHub, ChEMBL, GDB13, ZINC12, PubChem"
    - "Phytochemicals: IMPPAT, FooDB, CMNPD, AfroDb, DDPEDB"
    - "Human metabolites: HMDB, Aging Atlas, MetaboAge"
    - "Microbial metabolites: YMDB, ECMDB, gutMGene"
    - "Toxicity-screened: DSSTox"
  challenge: "Limited experimentally validated GPs (DrugAge, Geroprotectors.org) make computational decoding challenging"
  agextend_contribution: "Enables ultra-large-scale screening to differentiate geroprotective chemical space"

microbiome_aging_connection:
  gut_microbiota_role: "Gut microbes and metabolites closely linked to aging trajectories"
  fecal_transplant_evidence: "FMT from young to aged improves aging phenotypes, promotes longevity (multiple species)"
  agextend_microbiome_analysis:
    approach: "Two-stage investigation linking gut microbial alterations to metabolic aging effects"
    stage_1: "Age association (5,388 profiles, 13 datasets, ≥60 years)"
    stage_2: "Frailty association (ELDERMET cohort, FIM scores)"
    results:
      - "Age-negative taxa (n=43) significantly higher geroprediction scores (p=0.003)"
      - "FIM-positive species higher scores (p=0.02)"
      - "Negative correlation with telomere attrition (r=-0.32, p=0.025)"
      - "Validated healthy-aging species: R. hominis, D. longicatena, C. mitsuokai, C. comes"

metabolomics_aging:
  metabolic_plasticity: "Metabolic networks highly plastic, dynamics tightly linked with aging"
  age_associated_pathways:
    enriched_in_young:
      - "Taurine and hypotaurine metabolism"
      - "Sphingolipid metabolism"
      - "Biosynthesis of unsaturated fatty acids"
      - "Arginine biosynthesis"
      - "Pentose phosphate pathway"
      - "TCA cycle"
      - "Vitamin B6 metabolism"
    statistical_significance: "Amino acids (p=0.0014) and lipids (p=0.0001) enriched in young for predicted GPs"
  metabolite_classes:
    poorly_understood: "Lipids, amino acids increasingly recognized but functional significance unclear"
    agextend_contribution: "Functional and mechanistic exploration of aging-associated metabolites"

validation_models:
  yeast_cls:
    strain: "BY4741 (MATa his3Δ1 leu2Δ0 met15Δ0 ura3Δ0)"
    assay: "Chronological lifespan (CLS) assay"
    duration: "25 days"
    medium: "SC medium (2% glucose + amino acids)"
    staining: "Propidium iodide (PI) for cell survival"
    measurement: "Fluorescence (Ex 530/25nm, Em 590/25nm)"
    controls: "Untreated, vehicle, metformin (positive), heat-killed (PI control)"
    concentrations: "3 per metabolite (log scale: 0.1, 1, 10 μM or 0.01, 0.1, 1 mM)"
    timepoints: "Days 1,3,5,10,15,20,25"
    replicates: 8
    growth_control: "16h growth assay to rule out growth effects"
  celegans_lifespan:
    strain: "N2 (wild-type)"
    synchronization: "Egg-laying for 4h, L4 stage transfer"
    fUdr_treatment: "100 μg/ml for 18h (sterility)"
    drug_concentration: "100 μM"
    vehicle: "DMSO"
    scoring_frequency: "Every 2 days (day 0-10), days 13, 18, then alternate days to day 34"
    transfer_frequency: "Every 2 days until day 10, then days 13, 18"
    replicates: 90
    temperature: "20°C"
    medium: "NGM + Amp, PFA-treated OP50 bacteria"
    analysis: "Kaplan-Meier estimator, log-rank test (Oasis2 Python package)"
  human_fibroblasts:
    cell_line: "Primary human dermal fibroblasts (Lonza NHDF-Ad, CC-2511)"
    culture: "DMEM + 10% FBS"
    seeding: "0.5-0.7×10⁴ cells/well (12-well) for SA-β-gal, 1.5-3.5×10⁴ cells/well (96-well) for SBB/toxicity"
    senescence_induction: "Camptothecin (CPT) 25nM for 48h"
    metabolite_concentration: "1 μM"
    controls: "Vehicle (ethanol/water), untreated, azithromycin 100μM (positive)"
    assays:
      sa_beta_gal: "X-gal staining, 16-18h at 37°C, ×5 magnification"
      sudan_black_b: "Lipofuscin detection, 8min staining, ×10 magnification"
      fda_pi: "Fluorescein diacetate/propidium iodide viability"
      mtt: "MTT viability assay"
    quantification: "ImageJ/Fiji software"
    replicates: "10 micrographs for senescence, 4-12 biological replicates for toxicity"
```

## Lessons Learned

```yaml
achievements:
  platform_development:
    - "Developed first multimodal, bioactivity-based, explainable AI platform for geroprotector discovery"
    - "Four-module architecture (geroprediction, explainability, toxicity, target) with independent but interconnected operation"
    - "Outperformed previous geroprotector models in comparative analysis"
    - "Created publicly available Python package (PyPI) with Predictor and Browser functionalities"
  model_performance:
    - "Geroprediction: 79.2% accuracy, 86.4% AUC-ROC (LOOCV), 90.5% on independent 74 GPs"
    - "Explainability: AUC 0.85-1.00 across 9 aging hallmarks"
    - "Toxicity: AUC 0.83-0.99 across 15 ADMET models"
    - "Target: 45-100% hit rates for validated aging-related targets"
  bioactivity_descriptor_advantage:
    - "Signaturizer bioactivity descriptors outperformed chemistry-based (Mordred, ECFP) and graph-based (ConvMol) features"
    - "Demonstrated minimal structural similarity but high bioactivity similarity between training and validated compounds"
    - "Holistic representation integrating chemical and biological information"
  large_scale_screening:
    - "Screened 1,139,718,575 compounds (~1.1B) from 20 databases"
    - "Identified high-confidence GPs (probability ≥0.904) across diverse chemical space"
    - "Mapped geroprotective chemical space including drugs, metabolites, phytochemicals"
  experimental_validation:
    - "Successfully predicted excluded known GPs: metformin (0.65), taurine (0.70), N-acetyltaurine (0.80)"
    - "Yeast CLS: 24 metabolites tested, majority showed pro-longevity effects (ERP, SCoA, DCA, DRLP, DGA, AAA, PUT)"
    - "C. elegans: Fadrozole +10.8% lifespan (p=0.01), Anastrozole +8.4% (p=0.03)"
    - "Human fibroblasts: DCA and zymosterol reduced senescence markers (SA-β-gal, SBB)"
  metabolite_discoveries:
    - "Identified endogenous metabolites with geroprotective potential conserved in yeast-human networks"
    - "Pentose phosphate pathway metabolites (ERP, DRLP): Produce NADPH reducing agents, NADPH decreases with age"
    - "3-phospho-d-glycerate (DGA): Activates mitochondrial energy metabolism, increases NADP+:NADPH ratio"
    - "Deoxycholic acid (DCA): Senomodulator validated in human fibroblasts"
    - "Pathway enrichment: Taurine metabolism, sphingolipid metabolism, unsaturated fatty acid biosynthesis"
  microbiome_insights:
    - "Age-negative gut taxa significantly higher geroprediction scores (p=0.003)"
    - "FIM-positive species (frailty-protective) higher scores (p=0.02)"
    - "Identified healthy-aging-associated species: Roseburia hominis, Dorea longicatena, Catenibacterium mitsuokai, Coprococcus comes"
    - "Metabolite-driven associations with healthy aging and frailty protection"
    - "Negative correlation between FIM association and telomere attrition probability (r=-0.32, p=0.025)"
  explainability_insights:
    - "MD (mitochondrial dysfunction) most prevalent biological process for geroprotection"
    - "AIC, DNS, EA identified as key drivers (SHAP analysis)"
    - "Positive correlations: AIC-CS, MD-LP, CS-GI, MD-CS (Friedman H-statistic)"
    - "LP, SCE, TA critical for endogenous metabolite-driven pro-longevity responses"
  drug_repurposing:
    - "Validated 3 bioactive drugs from DrugBank with minimal structural similarity to training (<0.38 Tanimoto)"
    - "Fadrozole (aromatase inhibitor): Extended C. elegans lifespan"
    - "Anastrozole (aromatase inhibitor): Extended C. elegans lifespan"
    - "Demonstrates drug repurposing potential beyond structural similarity"

implications:
  ai_drug_discovery:
    - "Bioactivity-based descriptors superior to chemistry-based for geroprotector prediction"
    - "Explainability crucial for building trust and generating mechanistic hypotheses"
    - "Multi-module approach (prediction + explanation + toxicity + target) provides comprehensive assessment"
  aging_research:
    - "Systematic exploration of geroprotective chemical space now feasible at billion-compound scale"
    - "Endogenous metabolites represent underexplored source of geroprotectors"
    - "Microbiome-derived metabolites mediate beneficial/detrimental aging effects"
    - "Multi-hallmark targeting strategies enabled by explainability module"
  metabolic_aging:
    - "Metabolite-defined cellular microenvironment facilitates pro-longevity responses"
    - "Amino acids and lipids enriched in young samples for predicted GPs (p=0.0014, p=0.0001)"
    - "Age-negative gut taxa produce metabolites with higher geroprotective potential"
    - "Metabolic reprogramming pathway to promote longevity and cellular health"
  healthspan_vs_lifespan:
    - "Human life expectancy increased substantially, but healthspan improvements lag"
    - "Aging is predominant risk factor for comorbidities"
    - "Small molecule interventions practical means to suppress aging-associated changes"
    - "AgeXtend enables discovery of healthspan-promoting interventions"

challenges:
  training_data_limitations:
    - "Restricted training datasets for all modules"
    - "Performance bias toward diversity of training data"
    - "Limited experimentally validated GPs available (DrugAge, Geroprotectors.org)"
    - "Explainability module lacks representation of 3 newer hallmarks (dysbiosis - no training data; disabled macroautophagy, chronic inflammation - tight association with other hallmarks)"
  computational:
    - "Ultra-large-scale screening computationally intensive (1.1B compounds)"
    - "Bioactivity descriptor calculation resource-intensive (Signaturizer)"
  experimental:
    - "Need for validation across multiple model organisms"
    - "Species-specific responses may not generalize"
    - "Yeast CLS validation needed for replicative lifespan (SCE proxy)"
    - "Phase I/II metabolism prediction accuracy (Biotransformer 3.0)"
  data_quality:
    - "DarkChem dataset may contain false positives (limited bioassay coverage)"
    - "Potential for incorrectly classified bioactive compounds as inert"
  methodological:
    - "Machine learning inherent limitations (black-box elements despite explainability efforts)"
    - "Tanimoto similarity assumes structural similarity implies target similarity (ligand-based drug design assumption)"

impact_on_field:
  paradigm_shift:
    - "From chemistry-centric QSAR to bioactivity-based multimodal AI"
    - "From structural similarity to biological function similarity"
    - "From black-box predictions to mechanistically explainable insights"
  research_acceleration:
    - "Enables screening chemical space orders of magnitude beyond manual capacity"
    - "Compresses geroprotector discovery timeline through computational pre-screening"
    - "Prioritizes experimental validation resources on high-confidence predictions"
  open_science:
    - "Publicly available Python package (pip install AgeXtend)"
    - "Free for academic institutions (commercial license for commercial use)"
    - "Code and data on Zenodo, GitHub, CodeOcean"
    - "Pre-computed results for 1.1B compounds accessible via Browser"
  therapeutic_development:
    - "Drug repurposing: Screened DrugBank identifying candidates with longevity potential"
    - "Natural products: Systematic screening of phytochemicals from multiple databases"
    - "Endogenous metabolites: Revealed cellular metabolites as geroprotection targets"
    - "Microbiome: Metabolite-based approach to pro-longevity microbiome interventions"
  mechanistic_understanding:
    - "Links compounds to specific aging hallmarks providing research hypotheses"
    - "Reveals crosstalk between aging processes (AIC-CS, MD-LP correlations)"
    - "Identifies key aging processes (MD most prevalent, AIC/DNS/EA key drivers)"
    - "Senomodulator discovery pathway validated (CS module → experimental confirmation)"
  future_directions:
    - "Platform for ongoing geroprotector discovery as new compounds emerge"
    - "Framework extensible to additional aging hallmarks as training data becomes available"
    - "Integration with other aging databases and biobanks"
    - "Potential for personalized geroprotector recommendations based on individual aging profiles"

comparison_to_existing_approaches:
  advantages_over_previous_models:
    - "Bioactivity-based vs chemistry-only descriptors"
    - "Explainability module linking to aging hallmarks"
    - "Comprehensive toxicity assessment (15 ADMET models)"
    - "Target prediction from validated interactions (BindingDB)"
    - "Public availability and user-friendly interface"
    - "Superior performance metrics (theoretical comparison in Supplementary Table 10)"
  advantages_over_drug_repurposing:
    - "Not limited to approved drugs - explores full chemical space"
    - "Includes metabolites, phytochemicals, natural products"
    - "Mechanistic explainability beyond empirical drug effects"
  advantages_over_qsar:
    - "Multimodal bioactivity data vs chemical structure alone"
    - "Addresses chemically similar compounds with distinct bioactivities"
    - "Lower false positive/negative rates"
    - "Not limited by multifactorial nature of aging"
  advantages_over_virtual_screening:
    - "Bioactivity-based surrogates more potent than traditional virtual screening"
    - "Human-relevant predictions (not limited to non-human organism testing)"
    - "Direct aging hallmark associations vs pathway similarity proxies"
```

## Organizations

### Indraprastha Institute of Information Technology Delhi (IIIT-Delhi)

**Role in Project**: Primary research institution  
**Organization Type**: Institution  
**Status**: Operational  
**Location**: New Delhi, India  
**Website**: https://www.iiitd.ac.in/

**Contribution**: 

The Ahuja Lab in the Department of Computational Biology at IIIT-Delhi developed the complete AgeXtend platform including all four modules (geroprediction, explainability, toxicity, target). The team designed and executed comprehensive computational analysis workflows, built machine learning models, performed large-scale screening of 1.1 billion compounds, and conducted experimental validations in yeast, C. elegans, and human fibroblasts. The institution provided research infrastructure, computational resources, and IT support from the IT-HelpDesk team. All 17 authors except one collaborator are from IIIT-Delhi.

**Research Team**: Led by PI Gaurav Ahuja with 16 team members including co-first authors Sakshi Arora (TCS Research Scholar) and Aayushi Mittal, performing computational analysis, software development, yeast experiments, C. elegans experiments, human cell culture, microbiome analysis, and manuscript preparation.

**Description**: Public research university in New Delhi, India, established as an institute of eminence focused on information technology and interdisciplinary research. The Department of Computational Biology houses the Ahuja Lab specializing in AI applications for aging research, computational biology, and geroprotector discovery.

**Focus**: Information technology, artificial intelligence, machine learning, computational biology, aging research, bioinformatics

### Indian Institute of Technology Delhi (IIT Delhi)

**Role in Project**: Collaborating institution  
**Organization Type**: Institution  
**Status**: Operational  
**Location**: New Delhi, India  
**Website**: https://www.iitd.ac.in/

**Contribution**: Parul Mehrotra from the Kusuma School of Biological Sciences at IIT Delhi contributed to designing experimental workflows for C. elegans lifespan assays and human fibroblast senescence assays.

**Description**: Premier engineering and technology institute in New Delhi, India, one of the oldest and most prestigious IITs. The Kusuma School of Biological Sciences conducts interdisciplinary research at the intersection of biology, engineering, and technology.

**Focus**: Engineering, technology, biological sciences, interdisciplinary research

## Experimental Validation Results

### Yeast Chronological Lifespan (CLS) Assays

**24 Endogenous Metabolites Tested** (conserved in yeast-human metabolic networks):

Significant pro-longevity effects observed for:
- **d-Erythrose 4-phosphate (ERP)**: Strong geroprotective effect, 0.88 geroprediction probability
- **Succinyl-coenzyme A (SCoA)**: Strong geroprotective effect, 0.85 probability
- **Deoxycholic acid (DCA)**: Strong geroprotective effect, 0.83 probability, also validated as senomodulator in human cells
- **d-Ribulose 5-phosphate (DRLP)**: Strong geroprotective effect, 0.89 probability
- **3-Phospho-d-glycerate (DGA)**: Strong geroprotective effect, 0.78 probability
- **l-Ascorbic acid (AAA)**: Known geroprotector confirmed, 0.89 probability
- **Putrescine (PUT)**: Known geroprotector confirmed, 0.87 probability

**Protocol Details**:
- **Strain**: BY4741 (MATa his3Δ1 leu2Δ0 met15Δ0 ura3Δ0)
- **Duration**: 25 days
- **Timepoints**: Days 1, 3, 5, 10, 15, 20, 25
- **Concentrations**: 3 per metabolite (log scale: 0.1, 1, 10 μM or 0.01, 0.1, 1 mM)
- **Replicates**: 8 biological replicates
- **Staining**: Propidium iodide (PI) for cell survival measurement
- **Controls**: Untreated, vehicle, metformin (positive), heat-killed (PI control)
- **Growth control**: 16h growth assay confirmed no growth effects (except ERP, PUT, fucosterol)

**Pathway Enrichment**: Pentose phosphate pathway, glycolysis/gluconeogenesis, TCA cycle, vitamin B6 metabolism, taurine/hypotaurine metabolism, sphingolipid metabolism

### C. elegans Lifespan Assays

**3 Bioactive Drugs from DrugBank**:

- **Fadrozole (aromatase inhibitor)**: +10.8% maximum mean lifespan extension, p=0.01 (log-rank test), 0.74 geroprediction probability
- **Anastrozole (aromatase inhibitor)**: +8.4% maximum mean lifespan extension, p=0.03, 0.85 probability  
- **Amyl acetate**: Promising trend but non-significant at 95% confidence, 0.96 probability

**Selection Criteria**: Minimal Tanimoto similarity to training GPs (<0.38), high/diverse geroprediction scores (>0.7), novelty

**Protocol Details**:
- **Strain**: N2 (wild-type)
- **Synchronization**: Egg-laying 4h, L4 stage transfer
- **FUdR Treatment**: 100 μg/ml for 18h (maintains sterility throughout assay)
- **Drug Concentration**: 100 μM
- **Vehicle**: DMSO
- **Replicates**: 90 animals per condition
- **Scoring**: Every 2 days (day 0-10), days 13, 18, then alternate days to day 34
- **Temperature**: 20°C
- **Medium**: NGM + ampicillin, PFA-treated OP50 bacteria
- **Analysis**: Kaplan-Meier estimator, log-rank test (Oasis2 Python package)

### Human Fibroblast Senescence Assays

**2 Endogenous Metabolites Validated as Senomodulators**:

- **Deoxycholic acid (DCA, 1 μM)**: Reduced SA-β-gal+ cells under CPT-induced senescence, non-toxic to non-senescent cells, passed all ADMET assessments
- **Zymosterol (ZST, 1 μM)**: Reduced SA-β-gal+ cells, selective toxicity only under senescence conditions (toxic at 10 μM), validated by Sudan Black B staining

**Negative Control**: Dihydroxyacetone phosphate (DHAP) - pro-survival in yeast but no senomodulator activity (as predicted)

**Positive Control**: Azithromycin (100 μM) - validated senolytic

**Protocol Details**:
- **Cell Line**: Primary human dermal fibroblasts (Lonza NHDF-Ad, CC-2511)
- **Culture**: DMEM + 10% FBS
- **Senescence Induction**: Camptothecin (CPT) 25 nM for 48h
- **Metabolite Concentration**: 1 μM
- **Assays**: SA-β-galactosidase staining (X-gal, 16-18h at 37°C), Sudan Black B staining (lipofuscin detection)
- **Toxicity Assessment**: FDA/PI assay, MTT viability assay
- **Quantification**: ImageJ/Fiji software
- **Replicates**: 10 micrographs for senescence quantification

## Key Discoveries

### Validated Geroprotective Metabolites

**Pentose Phosphate Pathway Metabolites**:
- d-Erythrose 4-phosphate (ERP) and d-ribulose 5-phosphate (DRLP) directly involved in producing reducing agents (NADPH)
- NADPH levels decrease with age; augmentation of NADPH-powered redox networks enhances longevity
- Strong experimental validation in yeast CLS assays

**Energy Metabolism Modulators**:
- 3-Phospho-d-glycerate (DGA) activates mitochondrial energy metabolism
- Increases plasma concentration ratio [NADP+]:[NADPH]
- Results in decreased inflammation and enhanced cellular membrane integrity

**Bile Acid**:
- Deoxycholic acid (DCA) validated as senomodulator in human fibroblasts
- Predicted by explainability module's cellular senescence (CS) classifier
- Selective effect on senescent cells, non-toxic to normal cells

**Known Geroprotectors Confirmed**:
- l-Ascorbic acid (vitamin C) and putrescine showed pro-longevity effects in yeast

### Microbiome-Aging Connections

**Age-Negative Taxa** (decline with age, n=43 species):
- Significantly higher geroprediction scores vs age-positive taxa (p=0.003, Mann-Whitney U)
- Produce metabolites with geroprotective potential
- Include healthy-aging-associated species: Roseburia hominis, Dorea longicatena, Catenibacterium mitsuokai, Coprococcus comes
- Most metabolites predicted to inhibit loss of proteostasis (LP) and telomere attrition (TA)

**Frailty Index (FIM) Analysis** (ELDERMET cohort, 214 samples):
- FIM-positive species (negatively associated with frailty) had higher geroprediction scores (p=0.02)
- Negative correlation with telomere attrition probability (r=-0.32, p=0.025, Pearson)
- Demonstrates metabolite-driven associations with frailty protection

### Aging Atlas Metabolite Analysis

- Young samples significantly enriched for predicted geroprotective metabolites
- **Amino acids**: p=0.0014 (χ² test)
- **Lipids**: p=0.0001 (χ² test)
- Suggests metabolite-defined cellular microenvironment facilitates pro-longevity responses
- Key pathways: Taurine/hypotaurine metabolism, sphingolipid metabolism, biosynthesis of unsaturated fatty acids

### Drug Repurposing Discoveries

**Validated from DrugBank**:
- **Fadrozole** (aromatase inhibitor): Extended C. elegans lifespan +10.8% (p=0.01)
- **Anastrozole** (aromatase inhibitor): Extended C. elegans lifespan +8.4% (p=0.03)
- Both drugs had <0.38 Tanimoto similarity to training GPs, demonstrating bioactivity-based prediction beyond structural similarity

## Acknowledgments

Research supported by Department of Biotechnology (Ministry of Science & Technology, Government of India), SERB Start-Up Research Grant (SRG/2020/000232), EMBO Young Investigator Programme, IHUB Anubhuti (project grant/23), IIIT-Delhi intramural start-up grant, DST INSPIRE Faculty Grant (D. Sengupta), and TCS Foundation TCS Research Scholar Program (S. Arora).

Thanks to: IT-HelpDesk team IIIT-Delhi (computational resources), Ahuja Lab members (intellectual contributions), K. Sriram (mathematical calculations), V. K. Yenamandra (human fibroblasts), J. Tayal and A. Mehta (cell culture facility access), A. Mukhopadhyay (C. elegans strains).


