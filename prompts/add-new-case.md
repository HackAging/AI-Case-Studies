# Prompt: Add New Case

## Instructions for AI Agent

You are an expert in AI longevity research. Your task is to add a new case study to the repository by conducting comprehensive research and creating a complete case file.

## Case to Add

**Case name/company:** `[INSERT CASE NAME HERE]`

**Important:** If the case name is missing or unclear, ask the user to provide it before proceeding.

## Preparation

Before starting research:

1. **Check existing cases**
   - Open `memory-bank/projectbrief.md`
   - Review the complete list of existing cases
   - **Verify this case does NOT already exist**
   - If case exists, inform user and stop

2. **Study case structure**
   - Open `YAML_FIELDS.md`
   - Study the complete structure and all required fields
   - Understand format differences for commercial vs research cases
   - Note all entity types and relationships

## Methodology

### Step 1: Planning

Create a comprehensive plan using to-do items. Break down the research into specific tasks:

- [ ] Verify case doesn't exist in `memory-bank/projectbrief.md`
- [ ] Determine entity type (commercial/research)
- [ ] Study `YAML_FIELDS.md` structure
- [ ] Research basic information (name, description, status)
- [ ] Collect entity_data fields
- [ ] Research taxonomy (primary_focus, ai_technology, etc.)
- [ ] Find organizations
- [ ] Find products (if applicable)
- [ ] Find key people
- [ ] Collect links (websites, publications, GitHub)
- [ ] Research financials
- [ ] Find events and milestones
- [ ] Research partnerships
- [ ] Collect technical details
- [ ] Gather lessons learned
- [ ] Create case file with complete structure

### Step 2: Research Execution

For each to-do item, conduct thorough research:

1. **Use multiple sources:**
   - Company/research project websites
   - Scientific publications (PubMed, arXiv, bioRxiv, Google Scholar)
   - Press releases and news articles
   - Company databases (Crunchbase, PitchBook)
   - GitHub repositories
   - LinkedIn profiles
   - Funding announcements
   - Patent databases

2. **Mark to-do items as complete** as you find information:
   - Check off items when data is collected
   - Note sources for each piece of information
   - Document any gaps or missing information

3. **Track progress:**
   - Update to-do list regularly
   - Report findings to user
   - Ask for clarification if information is unclear or conflicting

### Step 3: Information Collection

Collect ALL available information according to `YAML_FIELDS.md`:

- Basic info (id, slug, name, description, status)
- Entity data (commercial: founded, headquarters, etc. / research: start_date, publication_date, etc.)
- Taxonomy (primary_focus, ai_technology, aging_approach, etc.)
- Organizations (all related organizations with full details)
- Products (if applicable)
- People (key researchers, founders, PIs)
- Links (websites, publications, GitHub, databases)
- Financials (funding rounds, grants)
- Events (important milestones)
- Partnerships (if any)
- Technical details (AI methods, architecture, workflow)
- Lessons learned (achievements, implications, challenges)

### Step 4: File Creation

1. **Determine file location:**
   - `cases/commercial/` for commercial entities
   - `cases/research/` for research entities
   - Filename: `{case-slug}.md` (lowercase, hyphens)

2. **Create case file:**
   - Follow structure from `YAML_FIELDS.md` exactly
   - Populate YAML frontmatter with all collected data
   - Write clear, comprehensive Markdown content
   - Use YAML blocks (not JSON) for structured data
   - Explain what the case is and how it works

3. **Validate:**
   - Check YAML syntax is valid
   - Verify all required fields are present
   - Ensure structure matches `YAML_FIELDS.md`

## Important Rules

1. **Ask for case name** if it's missing
2. **Verify uniqueness** - Check `memory-bank/projectbrief.md` first
3. **Use to-do list** - Plan and track progress systematically
4. **Study structure** - Read `YAML_FIELDS.md` thoroughly before collecting data
5. **Deep research** - Use multiple sources, be thorough
6. **Collect everything** - Gather all available details
7. **Use YAML blocks** - Not JSON for structured data
8. **Validate YAML** - All blocks must be valid
9. **Be accurate** - Verify facts, especially dates and numbers
10. **Be clear** - Explain what happens and how it works
11. **Document sources** - Include all URLs and references

## Workflow

1. **Check if case name provided** → If not, ask user
2. **Check existing cases** in `memory-bank/projectbrief.md`
3. **If case exists** → Inform user and stop
4. **Create to-do list** with all research tasks
5. **Study structure** in `YAML_FIELDS.md`
6. **Execute research plan** - check off items as you find information
7. **Collect all information** following the structure
8. **Determine entity type** (commercial/research)
9. **Create case file** in appropriate directory
10. **Populate YAML frontmatter** with all collected data
11. **Write Markdown content** with clear descriptions
12. **Validate YAML** - ensure all blocks are valid
13. **Present to user** for review

**Start by checking if the case name is provided, then verify it doesn't exist, create a research plan with to-do items, and execute it systematically.**
