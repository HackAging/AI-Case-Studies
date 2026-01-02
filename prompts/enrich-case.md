# Prompt: Enrich Case

## Instructions for AI Agent

You are an expert in collecting and structuring information about AI applications in longevity research. Your task is to gather maximum comprehensive information about a specific case and save it in the correct format.

## Project Context

This is a community-based repository of AI longevity case studies:
- Format: Markdown files with YAML frontmatter
- Structure: `cases/commercial/` or `cases/research/`
- See `YAML_FIELDS.md` for complete field structure

## Preparation

Before starting:

1. **Study case structure**
   - Open `YAML_FIELDS.md`
   - Understand required fields and complete structure
   - Learn format differences for commercial vs research cases

2. **Check existing case list**
   - Open `memory-bank/projectbrief.md`
   - Verify case name/slug is correct
   - Check if case already exists

## Case to Enrich

**Case name/company:** `[INSERT CASE NAME HERE]`

**Examples:**
- "Insilico Medicine"
- "Barabási Network Medicine"
- "NewLimit"
- "ESM3 esmGFP"

## Task

Gather maximum comprehensive information about the case and create/update the corresponding file in the project.

## Information Collection

### 1. Basic Information
- Full name
- Detailed description (2-3 paragraphs, clear and comprehensive)
- Mission/objectives
- Current status (operational, published, liquidated, ongoing)

### 2. For Commercial Cases
- Founded year
- Headquarters (city, state, country)
- Legal company name
- Website
- Industry
- Employee count (if available)
- Ticker and exchange (if public company)

### 3. For Research Cases
- Project start date
- Publication date
- Research objectives
- Methodology
- Results
- Collaboration period
- Author contributions
- Competing interests

### 4. Taxonomy (Categorization)
- Primary focus (AI-Driven Drug Discovery, Aging Clocks, etc.)
- AI technology (Generative AI, LLMs, Graph Neural Networks, etc.)
- Aging approach (Target Discovery, Drug Repurposing, etc.)
- Target biology (General Aging/Longevity, Senescence, etc.)
- Development stage
- Geography

### 5. Organizations
- All related organizations
- Organization roles
- Organization types
- Websites
- Contribution descriptions

### 6. Products
- Product/platform/methodology names
- Product types
- Development statuses
- Descriptions

### 7. People
- Key people (PIs, researchers, founders)
- Titles
- Affiliations
- Expertise
- Biographies
- Profiles (Google Scholar, ORCID, etc.)

### 8. Links
- Websites
- Scientific publications
- GitHub repositories
- Databases
- Reference materials

### 9. Finances
- Funding rounds
- Grants
- Amounts and dates
- Funding sources

### 10. Events
- Important events (publications, launches, partnerships)
- Dates
- Descriptions

### 11. Partnerships
- Partnerships with other organizations
- Partnership types
- Dates
- Descriptions

### 12. Technical Details
- AI methods (detailed explanation of what and how)
- System architecture
- Technical workflow
- Scientific background
- Performance metrics
- Infrastructure

### 13. Lessons Learned
- Achievements
- Implications
- Challenges
- Impact on field

## Research Sources

Use multiple sources:

1. **Company/research websites**
2. **Scientific publications** (PubMed, arXiv, bioRxiv, Google Scholar)
3. **Press releases and news**
4. **Company databases** (Crunchbase, PitchBook)
5. **GitHub repositories**
6. **LinkedIn profiles**
7. **Financial reports** (if public company)
8. **Patent databases**

## Quality Standards

The case must be:
- **Clear** - Easy to understand what the case is about
- **Comprehensive** - All available details collected
- **Accurate** - Verified facts, correct dates and numbers
- **Well-structured** - Follows `YAML_FIELDS.md` exactly
- **Complete** - No obvious gaps in information

## Validation and Verification

### 1. Data Completeness Check

After collecting information, evaluate:

- **Required fields present?** (id, slug, entity_type, status, name, description, taxonomy)
- **Entity data complete?** (all fields for commercial/research type)
- **Organizations listed?** (at least primary organization)
- **Products documented?** (if applicable)
- **People included?** (key researchers, founders, PIs)
- **Links diverse?** (websites, publications, GitHub, etc.)
- **Technical details comprehensive?** (AI methods, architecture, workflow)
- **Scientific background included?** (for research cases)

### 2. Identify Gaps and Inconsistencies

Check for:
- **Missing critical information** (founded date, headquarters, publication date)
- **Incomplete descriptions** (too short, lacks detail)
- **Missing related entities** (organizations, people, products)
- **Outdated information** (old status, missing recent developments)
- **Inconsistent data** (conflicting dates, contradictory information)
- **Unclear explanations** (what/how not clearly described)

### 3. Verify Accuracy

- **Cross-check facts** across multiple sources
- **Verify dates** are logical and consistent
- **Check names** are spelled correctly
- **Validate links** are working
- **Confirm status** reflects current state

### 4. Ask User When Uncertain

**Always ask user to verify when:**
- Information is contradictory across sources
- You're unsure about classification (commercial vs research)
- Critical data is missing and you can't find it
- Dates or facts seem incorrect
- You need clarification on technical details
- Status is unclear

**Format for questions:**
```
I found conflicting information about [specific issue]. 
Source 1 says: [X]
Source 2 says: [Y]
Could you please verify which is correct?
```

## Output Format

1. **Find or create case file**
   - Check `cases/commercial/` or `cases/research/`
   - If exists: read and enhance
   - If not: create new with proper slug

2. **Update/create YAML frontmatter**
   - Follow `YAML_FIELDS.md` structure exactly
   - All required fields filled
   - Entity data matches entity type

3. **Enhance Markdown content**
   - Clear, comprehensive descriptions
   - Well-organized sections
   - Use YAML blocks (not JSON) for structured data
   - Explain what happens and how it works

4. **File structure:**
```markdown
---
id: case-slug
slug: case-slug
entity_type: commercial/research
status: operational/published
# ... all YAML frontmatter fields
---

# Case Name

## Description
[Clear, detailed description explaining what the case is about and how it works]

## Mission
[Mission statement]

## Technical Details

```yaml
# Structured data in YAML
ai_methods: [detailed list]
system_architecture: [clear explanation]
technical_workflow: [step-by-step process]
```

## Organizations
[Description of organizations]

# ... other sections
```

## Important Rules

1. **Check existing file first** - If exists, enhance it, don't overwrite completely
2. **Preserve structure** - Follow format of existing cases
3. **Use YAML blocks** for structured data (not JSON)
4. **Validate YAML** - All blocks must be valid
5. **Add sources** - Include links to all found materials
6. **Be accurate** - Verify facts, especially dates and numbers
7. **Be clear** - Explain what happens and how it works
8. **Be comprehensive** - Collect all available details
9. **Ask when uncertain** - Always verify with user if information is unclear or conflicting
10. **Check completeness** - Evaluate data completeness and identify gaps

## Workflow

1. **Read case structure** from `YAML_FIELDS.md`
2. **Find or locate case file** in `cases/` directory
3. **Research comprehensively** using multiple sources
4. **Collect all available information** following the checklist above
5. **Evaluate completeness** - identify gaps and missing information
6. **Check for inconsistencies** - verify facts across sources
7. **Ask user** if information is unclear or conflicting
8. **Create/update file** with proper structure
9. **Validate YAML** - ensure all blocks are valid
10. **Present to user** for review and validation

**Start by researching the case `[INSERT CASE NAME]` and gathering comprehensive information.**
