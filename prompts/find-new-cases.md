# Prompt: Find New Cases

## Instructions for AI Agent

You are an expert in AI applications for longevity research. Your task is to find new cases of AI use in aging research and intervention that are not yet in the database.

## Project Context

This is a community-based repository of AI longevity case studies:
- **60 existing cases** (32 commercial companies, 28 research projects)
- Format: Markdown files with YAML frontmatter
- Structure: `cases/commercial/` and `cases/research/`

## Preparation

Before starting your search:

1. **Read the existing case list**
   - Open `memory-bank/projectbrief.md`
   - Study the complete list of existing cases (commercial and research)
   - Understand what cases are already documented

2. **Study case structure**
   - Open `YAML_FIELDS.md`
   - Understand required fields and structure
   - Learn the format for commercial vs research cases

3. **Understand project goals**
   - Read `memory-bank/productContext.md` for workflow details
   - Understand what makes a valid case

## Task

Find **new cases** that are not in the existing list. Cases must:

1. **Use AI/ML** to address aging or longevity challenges
2. **Be current** (2020-2025, prioritize 2024-2025)
3. **Have public information** (publications, websites, press releases)
4. **Relate to longevity research** or aging intervention

## Search Criteria

**Commercial cases:**
- Companies developing AI solutions for aging research
- Longevity/biotech startups with AI components
- Platforms using AI for drug discovery in aging context
- Companies with published results or products

**Research cases:**
- Scientific publications using AI/ML for aging research
- Research projects with AI components
- Collaborations applying AI methods
- New methodologies using AI to study aging

## Research Process

1. **Deep research**
   - Use web search for recent companies and projects
   - Check scientific databases (PubMed, arXiv, bioRxiv, Google Scholar)
   - Review news sources and press releases
   - Check company databases (Crunchbase, PitchBook)
   - Look for recent funding announcements

2. **Verify uniqueness**
   - Cross-reference with existing case list from `projectbrief.md`
   - Ensure case is not already documented
   - Check if it's a sub-project of existing case

3. **Validate relevance**
   - Confirm AI/ML is central to the approach
   - Verify connection to longevity/aging research
   - Ensure sufficient public information exists

## Output Format

For each new case found, provide:

1. **Name** - Case/company/project name
2. **Type** - commercial or research
3. **Description** - Brief description (2-3 sentences)
4. **Sources** - Links to publications, websites, press releases
5. **Justification** - Why this is a new case (not in existing list)

**Example:**
```
New Case #1:
- Name: [Company/Project Name]
- Type: commercial/research
- Description: [Brief description of what they do and how AI is used]
- Sources:
  - [URL 1 - website/publication]
  - [URL 2 - additional source]
- Justification: [Why this is new - not found in projectbrief.md list]
```

## Important Rules

- **Check existing list first** - Always verify against `memory-bank/projectbrief.md`
- **Prioritize recent cases** - Focus on 2024-2025 cases
- **Quality over quantity** - Better to find 3-5 high-quality cases than 20 weak ones
- **AI must be central** - Case must use AI/ML as core approach, not just mention it
- **Sufficient information** - Case must have enough public data to create full case study

## Start Search

Begin by:
1. Reading `memory-bank/projectbrief.md` for existing cases
2. Reviewing `YAML_FIELDS.md` for case structure
3. Conducting deep research using multiple sources
4. Finding minimum 3-5 new cases not in existing list
