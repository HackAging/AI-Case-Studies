# YAML Frontmatter - Required and Recommended Fields

Documentation based on the actual structure of cases from the database.

## Required Fields

These fields must be present in every case:

```yaml
id: case-slug              # Unique case identifier (usually matches slug)
slug: case-slug           # URL-friendly identifier
entity_type: commercial    # Type: "commercial" or "research"
status: operational       # Status (see below)
name: Case Name           # Case name
```

## Status Values

Status values depend on case type:

**For commercial:**
- `operational` - company is operating
- `liquidated` - company is closed

**For research:**
- `published` - research is published
- `ongoing` - research is ongoing

## Metadata

```yaml
data_completeness: high   # "exceptional", "very_high", "high", "moderate", "low"
last_researched: 2025-12-29  # Date of last research (YYYY-MM-DD)
researcher: AI Assistant  # Researcher who collected the data
version: 4.2              # Data version
```

**For research cases:**
```yaml
research_category: collaboration  # "collaboration", "academic_institution", "internal"
```

## Basic Information

```yaml
description: "Full case description. Can be long text with details."
mission: Mission statement  # Project/company mission
```

## Entity Data

### For Commercial Cases

```yaml
entity_data:
  name: Company Legal Name
  status: operational
  legal_name: Full Legal Name
  founded: 2014
  headquarters:
    city: Cambridge
    state: Massachusetts
    country: USA
  ticker: INS  # If public company
  exchange: NASDAQ  # Stock exchange
  employees: 500
  industry: Biotechnology
  focus: AI-driven drug discovery
  website: https://example.com
  parent_company: Parent Company Name  # Optional
```

### For Research Cases

```yaml
entity_data:
  name: Research Project Name
  status: published
  objectives:
    - Objective 1
    - Objective 2
  start_date: 2024-01-01
  completion_date: 2025-09-03  # Optional
  publication_date: 2025-09-03
  description: "Research project description"
  methodology: "Research methodology description"
  results: "Research results summary"
  collaboration_period:
    start: 2024
    publication_date: 2025-09-03
  author_contributions:
    methodology:
      - Researcher Name
    supervision:
      - PI Name
    investigation:
      - Researcher Name
    visualization:
      - Researcher Name
    conceptualization:
      - Researcher Name
    writing_original_draft:
      - Researcher Name
    writing_review_editing:
      - Researcher Name
  competing_interests:
    no_conflicts:
      - Researcher Name
    declared_conflicts:
      - company: Scipher Medicine, Inc.
        persons:
          - Person Name
        relationship: Founders
        company_focus: Description
  supplementary_data:
    data_availability: Description
    github_repository: "https://github.com/user/repo"
    supplementary_tables:
      - "Table S5: Description"
```

## Taxonomy (Categorization)

```yaml
taxonomy:
  primary_focus:          # Array: ["AI-Driven Drug Discovery", "Aging Clocks", ...]
    - "AI-Driven Drug Discovery"
  ai_technology:          # Array: Short names for UI ["Generative AI", "LLMs", "Graph Neural Networks", ...]
    - "Generative AI"
    - "Diffusion Models"
    - "Graph Neural Networks"
    - "Predictive ML/DL"  # Legacy (only in ~13 cases)
  ai_approach:            # Array: Broad learning approaches (NEW)
    - "Generative AI"
    - "Supervised Learning"
    - "Unsupervised Learning"
    - "Reinforcement Learning"
    - "Active Learning"
  ai_architecture:        # Array: Specific model architectures (NEW)
    - "LLMs"
    - "Protein LMs"
    - "Diffusion Models"
    - "Graph Neural Networks"
    - "Transformers"
    - "Autoencoders"
    - "Computer Vision (CNNs/ViTs)"
    - "Kolmogorov-Arnold Networks"
  ai_specialization:      # Array: Specialized techniques (NEW)
    - "Multi-Agent AI"
    - "Federated Learning"
    - "Ensemble Methods"
    - "Transfer Learning"
    - "Bayesian Optimization"
    - "RAG"
  aging_approach:         # Array: ["Target Discovery", "Drug Repurposing", ...]
    - "Target Discovery"
  target_biology:         # Array: ["General Aging/Longevity", "Senescence", ...]
    - "General Aging/Longevity"
    - "Neurodegenerative"
    - "Metabolic Diseases"
    - "Cancer/Oncology"
    - "Eye Diseases"
    - "Fibrosis"
  development_stage: Research / Preclinical  # "operational", "published", "Research / Preclinical", "Clinical Trials", "Discontinued"
  geography: USA          # Geography (countries/regions)
  organization_type: research  # "research", "company"
  organization_subtype: collaboration  # For research: "collaboration", "academic_institution", "internal"
  therapeutic_modality: []  # Array: ["Small Molecules", "Therapeutic Proteins", "Gene Therapy", "Cell Therapy", "RNA Therapeutics", "PROTAC"]
```

**Primary Focus Values (12 possible):**
- `AI-Driven Drug Discovery`
- `Aging Clocks`
- `Senescent Cells & Senolytics`
- `Protein Design & Engineering`
- `Gene Editing & Therapy`
- `Cellular Rejuvenation`
- `Clinical Trials Optimization`
- `Autonomous AI Scientists`
- `Robotic Lab Automation`
- `Diagnostics & Preventive Health`
- `Multi-Omics & Biomarkers`
- `Virtual Cells & Digital Twins`

**Aging Approach Values (6 possible):**
- `Target Discovery`
- `Molecule Design`
- `Therapeutic Development`
- `Diagnostics/Age Assessment`
- `Cellular Rejuvenation`
- `Senescent Cell Elimination`

## Organizations

```yaml
organizations:
  - name: Organization Name
    legal_name: Full Legal Name  # Optional
    role: primary         # "primary", "partner", "institution", "lab", "collaborator"
    org_type: company     # "company", "research_center", "institution", "spinoff", "lab"
    website: "https://example.com"
    status: operational   # "operational", "closed", "liquidated", "acquired", "active", "merged"
    role_description: Description of organization's role
    contribution_description: Detailed description of contribution
    description: Organization description
    focus: Organization focus area
    founded: 2014  # For companies
    parent_organization_id: parent-org-id  # If lab belongs to institution
    director:  # For labs
      name: Director Name
      title: Director Title
      expertise: Expertise area
      background: Background description
    research_focus:  # For labs
      - Research area 1
      - Research area 2
    key_achievements:  # For labs
      - Achievement 1
      - Achievement 2
    logo_url: "https://example.com/logo.png"  # For companies
    social_media:  # For companies
      twitter: "https://twitter.com/..."
      linkedin: "https://linkedin.com/company/..."
      facebook: "https://facebook.com/..."
      youtube: "https://youtube.com/..."
    media_links:  # For companies
      press_kit: "https://example.com/press"
      media_contact: "contact@example.com"
      newsroom: "https://example.com/news"
      blog: "https://example.com/blog"
      careers: "https://example.com/careers"
      investor_relations: "https://example.com/investors"
    involvement_period:  # Period of involvement in this case
      start: "2024-01"
      end: "2025-12"
      status: "active"  # "active", "completed", "ongoing"
```

## Products

```yaml
products:
  - name: Product Name
    alternative_names:  # Optional
      - Alternative Name 1
      - Alternative Name 2
    type: AI Software Platform  # "AI Software Platform", "research_methodology", "therapeutic", "ai_model", "platform", "drug", "therapy"
    status: published  # "published", "operational", "development", "discontinued"
    development_stage: Research / Preclinical  # "Research / Preclinical", "Clinical Trials", "Operational", "Discontinued"
    description: Product description
    mechanism: Mechanism of action
    target: Target molecule/pathway
    target_pathway: Target pathway description
    capabilities:  # Array
      - Capability 1
      - Capability 2
    applications:  # Array
      - Application 1
      - Application 2
    indications:  # Array of objects
      - primary: Primary indication
        secondary: Secondary indication  # Optional
        status: Status  # Optional
    clinical_trials:  # Array of objects
      - phase: Phase number
        status: Trial status
        results: Results summary
        dates:
          start: 2024-01-01
          end: 2025-12-31
    components:  # Array of objects
      - name: Component Name
        description: Component description
        technical_details: Component technical details
    infrastructure:  # Object
      description: Infrastructure description
      details: Additional infrastructure details
    technical_details:  # Object
      ai_methods: AI methods used
      architecture: System architecture
      training_data: Training data description
      performance_metrics: Performance metrics
      validation: Validation details
```

## People

```yaml
people:
  - name: Person Name
    title: PhD  # "PhD", "MD", "Professor", etc.
    person_type: founder  # "founder", "leadership", "researcher", "advisor", "pi"
    role: CEO  # "CEO", "Lead Researcher", "Principal Investigator", etc.
    background: Background description
    expertise: Expertise area
    previous_role: Previous role description
    bio: Full biography
    profile_url: "https://example.com/profile"
    email: person@example.com
    phone: +1-234-567-8900
    orcid_id: "0000-0000-0000-0000"  # For researchers
    google_scholar_id: "scholar-id"
    researchgate_url: "https://www.researchgate.net/profile/..."
    affiliations:  # Array
      - Affiliation 1
      - Affiliation 2
    organization_id: org-id  # Organization in context of this case
    period: "2015-present"  # Period of involvement
    involvement_period:  # Detailed period
      start: "2024-01"
      end: "2025-12"
      status: "active"  # "active", "completed", "ongoing"
    responsibilities:  # Array
      - Responsibility 1
      - Responsibility 2
    contribution_description: Description of contribution to this case
```

## Links

```yaml
links:
  - url: "https://example.com"
    type: website  # "website", "research_publication", "github", "database", "reference", "news_article", "article", "blog_post", "press_release", "video", "case_study", "social_media", "documentation", "patent"
    title: Link Title
    description: Link description
    authors:  # Array
      - Author Name 1
      - Author Name 2
    publisher: Publisher Name
    publication_date: 2025-01-01
    language: en  # "en", "ru", etc.
    excerpt: Brief excerpt/description
    thumbnail_url: "https://example.com/thumbnail.jpg"
    word_count: 5000
    full_text: Full text content (for full-text search)
    is_active: true
    last_checked_at: 2025-12-29T12:00:00Z
    tags:  # Array
      - Tag 1
      - Tag 2
    metadata:  # Object
      doi: "10.1234/example"
      arxiv_id: "2509.03330"
      journal: Journal Name
      volume: "123"
      pages: "45-67"
      citations: 100
      video_duration: 3600
      references_in_article:  # Array
        - Reference 1
        - Reference 2
    relevance: primary  # "primary", "secondary", "tertiary" (in context of case)
    category: source  # "source", "publication", "reference", "related"
    description: Description of link's relevance to case
    display_order: 1  # For sorting
```

**Link Types:**
- `website` - Website
- `research_publication` - Scientific publication
- `github` - GitHub repository
- `database` - Database
- `reference` - Reference material
- `news_article` - News article
- `article` - Article
- `blog_post` - Blog post
- `press_release` - Press release
- `video` - Video
- `case_study` - Case study
- `social_media` - Social media
- `documentation` - Documentation
- `patent` - Patent

## Financials

```yaml
financials:
  - category: funding  # "funding", "grant", "investment", "ipo", "partnership_deal"
    amount: "$100M"  # "$100M", "€50M", "Not disclosed"
    amount_numeric: 100000000  # Numeric value for sorting/filtering
    currency: USD  # "USD", "EUR", "GBP"
    funding_date: 2024-01-01
    period: "2020-2024"  # Optional
    source: "Venture Capital"  # "NIH", "Venture Capital", "Microsoft"
    funding_type: "Series A"  # "Series A", "Grant", "Partnership"
    description: Funding description
    note: Additional note
    details:  # Object
      investors:  # Array
        - Investor Name 1
        - Investor Name 2
      grant_number: "R01-12345"
      allocation:  # Array
        - category: Research
          amount: "$50M"
      conditions: Funding conditions
```

## Events

```yaml
events:
  - event_date: 2024-01-01
    event_type: foundation  # "foundation", "launch", "publication", "ipo", "acquisition", "partnership", "milestone", etc.
    title: Event Title
    description: Event description
    details:  # Object
      location: Event location
      participants:  # Array
        - Participant Name
      outcomes: Event outcomes
      related_links:  # Array
        - "https://example.com/related"
```

## Partnerships

```yaml
partnerships:
  - partnership_date: 2024-01-01
    partnership_type: research  # "research", "strategic", "technology", "commercial"
    description: Partnership description
    focus: Partnership focus area
    deal_value: "$100M"  # "$100M", "Undisclosed"
    deal_structure: Deal structure description
    details:  # Object
      duration: Partnership duration
      goals: Partnership goals
      outcomes: Partnership outcomes
    organizations:  # Array of organization objects
      - name: Organization Name
        role: partner  # "partner", "initiator", "collaborator", "sponsor"
        role_description: Description of organization's role in partnership
```

## Locations

Locations are accessed through organizations. Each organization can have multiple locations:

```yaml
locations:  # Within organization context
  - location_type: headquarters  # "headquarters", "office", "lab", "facility", "institution"
    name: "Main Office"  # "Main Office", "Research Lab", "Cambridge HQ"
    city: Cambridge
    state: Massachusetts
    country: USA
    address: Full address
    postal_code: "02139"
    coordinates:  # Object
      lat: 42.3656
      lng: -71.0809
    website: "https://example.com"
    phone: "+1-234-567-8900"
    email: "contact@example.com"
    is_primary: true
    notes: Additional notes
    location_role: headquarters  # "headquarters", "office", "lab", "facility"
    start_date: 2024-01-01
    end_date: null  # null = current
```

## Technical Details (YAML blocks in Markdown content)

Technical details are stored as YAML blocks within the Markdown content (not in frontmatter):

```markdown
## Technical Details

```yaml
ai_methods:
  - Method 1
  - Method 2
data_types:
  - Data type 1
  - Data type 2
platforms:
  - Platform 1
  - Platform 2
infrastructure:
  description: Infrastructure description
  components:
    - Component 1
    - Component 2
system_architecture:
  overview: Architecture overview
  components:
    - name: Component Name
      description: Component description
technical_workflow:
  steps:
    - step: Step 1
      description: Description
scientific_background:
  overview: Scientific background
  key_concepts:
    - Concept 1
    - Concept 2
governance_structure:
  description: Governance structure
performance_metrics:
  accuracy: 95%
  precision: 92%
validation:
  method: Validation method
  results: Validation results
```

## Lessons Learned (YAML blocks in Markdown content)

Lessons learned are stored as YAML blocks within the Markdown content:

```markdown
## Lessons Learned

```yaml
achievements:
  - Achievement 1
  - Achievement 2
implications:
  - Implication 1
  - Implication 2
challenges:
  - Challenge 1
  - Challenge 2
impact_on_field: Impact description
```

## YAML Blocks in Markdown Content

Within the Markdown file body (after frontmatter), use YAML blocks for structured data:

```markdown
## Technical Details

```yaml
overview: Description
components:
  - name: Component 1
    description: Description...
```

## Scientific Background

```yaml
network_medicine:
  definition: Definition...
  key_principles:
    - Principle 1
```

These blocks contain structured data that can be easily converted back to JSON for loading into Supabase.

## Complete Example: Research Case

```yaml
---
id: barabasi-network-medicine
slug: barabasi-network-medicine
entity_type: research
status: published
data_completeness: exceptional
last_researched: 2025-12-29
research_category: collaboration
researcher: AI Assistant
version: 4.2
name: Barabási–Gladyshev–Loscalzo Network Medicine for Hallmarks of Aging
description: "SHARP (Systematic Hallmark-based Aging Repurposing Pipeline): Network medicine framework..."
mission: Network medicine approach for drug repurposing targeting hallmarks of aging using SHARP pipeline

entity_data:
  name: Barabási–Gladyshev–Loscalzo Network Medicine
  status: published
  objectives:
    - Identify drug repurposing candidates targeting hallmarks of aging
    - Develop network medicine framework for systematic drug discovery
  start_date: 2024-01-01
  publication_date: 2025-09-03
  collaboration_period:
    start: 2024
    publication_date: 2025-09-03
  author_contributions:
    methodology:
      - Bnaya Gross
    supervision:
      - Vadim N. Gladyshev
      - Albert-László Barabási
  competing_interests:
    no_conflicts:
      - Bnaya Gross
    declared_conflicts:
      - company: Scipher Medicine, Inc.
        persons:
          - Albert-László Barabási
        relationship: Founders

taxonomy:
  geography: USA
  ai_technology:
    - Graph Neural Networks
    - Predictive ML/DL
  primary_focus:
    - AI-Driven Drug Discovery
  aging_approach:
    - Target Discovery
  target_biology:
    - General Aging/Longevity
  development_stage: Research / Preclinical
  organization_type: research
  organization_subtype: collaboration

organizations:
  - name: Network Science Institute, Northeastern University
    role: primary
    org_type: research_center
    website: "https://www.networkscienceinstitute.org/"
    status: operational
    role_description: Primary development institution
    contribution_description: Network Science Institute hosts Barabási Lab...

products:
  - name: SHARP: Systematic Hallmark-based Aging Repurposing Pipeline
    type: research_methodology
    status: published

links:
  - url: "https://arxiv.org/abs/2509.03330"
    type: research_publication
    title: Network-driven discovery of repurposable drugs targeting hallmarks of aging
  - url: "https://github.com/BnayaGross/Longevity-module"
    type: github
    title: SHARP Pipeline GitHub Repository
---
```

## Complete Example: Commercial Case

```yaml
---
id: insilico-pharma-ai
slug: insilico-pharma-ai
entity_type: commercial
status: operational
data_completeness: high
last_researched: 2025-12-23
researcher: AI Assistant
version: 4.2
name: Insilico Medicine Pharma.AI Platform
description: End-to-end AI-driven drug discovery and development platform
mission: To extend healthy and productive longevity for all

entity_data:
  name: Insilico Medicine
  legal_name: Insilico Medicine, Inc.
  status: operational
  founded: 2014
  headquarters:
    city: Cambridge
    state: Massachusetts
    country: USA
  website: https://insilico.com/
  industry: Biotechnology
  focus: AI-driven drug discovery

taxonomy:
  primary_focus:
    - "AI-Driven Drug Discovery"
  ai_technology:
    - "Generative AI"
    - "Diffusion Models"
  development_stage: operational
  geography: USA

organizations:
  - name: Insilico Medicine
    role: primary
    org_type: company
    website: "https://insilico.com/"
    status: operational

products:
  - name: Pharma.AI Platform
    type: AI Software Platform
    status: operational

links:
  - url: https://insilico.com/
    type: website
    title: Insilico Medicine - Official Website
---
```

## Validation Rules

1. **id and slug** must match and be unique
2. **entity_type** must be either "commercial" or "research"
3. **status** must match the type:
   - commercial: "operational", "liquidated"
   - research: "published", "ongoing"
4. **taxonomy.primary_focus** must be an array with at least one element
5. **taxonomy.ai_technology** must be an array with at least one element
6. All dates in format YYYY-MM-DD
7. **entity_data** structure depends on `entity_type`:
   - commercial: contains `founded`, `headquarters`, `legal_name`, etc.
   - research: contains `objectives`, `start_date`, `publication_date`, `author_contributions`, etc.
8. **URLs** must start with `http://` or `https://`
9. **Email addresses** must be valid format if provided

## Notes

- Fields with `null` or `undefined` values should not be included in YAML frontmatter
- Arrays can be empty (`[]`), but it's better not to include them if empty
- Nested objects are formatted with proper indentation (2 spaces)
- Strings with special characters are automatically escaped in quotes
- YAML blocks in Markdown content (not in frontmatter) are used for structured data that converts to JSON for Supabase

## Connection to Supabase

Data from YAML frontmatter and YAML blocks in Markdown content automatically converts to JSON for loading into Supabase:

- YAML frontmatter → main fields in `cases` table
- YAML blocks in content → JSONB fields (`technical_details`, `scientific_background`, `lessons_learned`)
- Related entities (organizations, people, products, links, financials, events, partnerships) → respective tables with relationships

For reverse conversion (YAML → JSON), use the `js-yaml` library:

```typescript
import yaml from 'js-yaml';

// Parse YAML block
const yamlContent = `...`;
const jsonData = yaml.load(yamlContent);

// Load into Supabase
await supabase.from('cases').update({
  technical_details: jsonData
}).eq('id', 'case-id');
```
