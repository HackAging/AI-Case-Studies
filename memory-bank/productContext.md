# Product Context: HackAging AI Case Studies

## Project Purpose

Create an open knowledge base of AI applications in longevity research. This community-based project uses AI to collect, structure, and maintain comprehensive case studies of how artificial intelligence is applied to aging research and intervention.

## Problems We Solve

1. **Information Fragmentation** - Case information is scattered across publications, press releases, news articles, and product documentation
2. **Data Obsolescence** - Information quickly becomes outdated (company status changes, new products launch, metrics update)
3. **Lack of Structure** - Need structured format for AI agents to analyze, compare, and generate insights

## Target Audience

- **Researchers** - Quick access to AI longevity applications, understanding current state of the field
- **Contributors** - Improve existing cases, add new ones, validate data
- **AI Agents** - Structured data for analysis, context for content generation
- **Developers** - Use data in applications, create visualizations and analytics

## How the Project Works

### Workflow 1: Review and Improve Existing Case

**Purpose:** Improve completeness, accuracy, and quality of existing case studies through comprehensive review and validation.

**Steps:**

1. **Select a case to review**
   - Choose from `cases/commercial/` or `cases/research/`
   - Or specify case name/slug

2. **Read and analyze the case**
   - Read the case file completely
   - Compare against `YAML_FIELDS.md` structure
   - Check for missing required fields (id, slug, entity_type, status, name)
   - Verify entity_data matches entity type (commercial vs research)
   - Check taxonomy fields are arrays with at least one value
   - Identify gaps in information

3. **Validate YAML structure**
   - Ensure all YAML frontmatter parses correctly
   - Verify all YAML blocks in content are valid
   - Check dates are in YYYY-MM-DD format
   - Ensure no null/undefined values in frontmatter
   - Verify structure matches `YAML_FIELDS.md` exactly

4. **Validate data accuracy**
   - Verify company/research status is current
   - Check links are working (no 404s)
   - Verify dates are logical (founded < current year, publication dates make sense)
   - Check names are spelled correctly
   - Confirm facts are accurate

5. **Check completeness**
   - Descriptions are detailed (not just one sentence)
   - Organizations have role descriptions and contribution descriptions
   - Products have types and statuses
   - People have affiliations, roles, and expertise
   - Links are diverse (websites, publications, GitHub, databases)
   - Technical details are comprehensive

6. **Check currency**
   - Information is up-to-date (check last_researched date)
   - Status reflects current state
   - No outdated information
   - Recent developments included (if any)

7. **Perform additional research**
   - Search for updated information (company website, recent publications)
   - Find missing links, organizations, people
   - Verify current status (operational, published, liquidated)
   - Check for new developments (products, partnerships, funding)
   - Look for new publications or press releases

8. **Create improvement plan**
   - List missing required fields (high priority)
   - List outdated information (high priority)
   - List missing related entities (organizations, people, products, links) - high priority
   - List incomplete descriptions (medium priority)
   - List enhancements and additional details (low priority)
   - Prioritize improvements

9. **Execute improvements**
   - Add missing YAML frontmatter fields
   - Update outdated information
   - Enhance descriptions with new details
   - Add missing organizations, people, products, links
   - Improve YAML structure and formatting
   - Use YAML blocks (not JSON) for structured data in Markdown content
   - Fix any YAML validation errors
   - Update last_researched date

10. **Final validation**
    - Ensure all YAML is valid (can be parsed)
    - Check structure matches `YAML_FIELDS.md`
    - Verify all links are working
    - Confirm dates and facts are accurate
    - Ensure all required fields are present
    - Check data completeness meets quality standards

11. **Save and present**
    - Update the case file
    - Present changes to user: "I've reviewed and improved the case. Changes include: [list]"
    - User reviews and validates
    - User approves or requests adjustments

**Output:** Improved case file ready for commit/PR

### Workflow 2: Add New Case

**Purpose:** Document a new company or research project that uses AI in longevity research.

**Steps:**

1. **Get case information**
   - Ask user for company/project name
   - Or user provides case name directly

2. **Research the case**
   - Use web search to find information
   - Check scientific databases (PubMed, arXiv, bioRxiv, Google Scholar)
   - Visit company/research websites
   - Look for publications, press releases, funding information
   - Check Crunchbase, PitchBook for company data
   - Determine entity type: commercial or research

3. **Collect comprehensive information**

   **Required fields:**
   - `id`, `slug`, `entity_type`, `status`, `name`
   - `description` (detailed, 2-3 paragraphs)
   - `taxonomy.primary_focus` (at least one)
   - `taxonomy.ai_technology` (at least one)

   **For commercial cases:**
   - Entity data: founded date, headquarters, legal name, website, industry
   - Organizations: primary company with full details
   - Products: platforms, therapeutics, services
   - People: founders, key executives, researchers
   - Finances: funding rounds, amounts, dates (if available)

   **For research cases:**
   - Entity data: start date, publication date, objectives, methodology
   - Organizations: participating institutions, labs
   - People: PIs, researchers, authors with affiliations
   - Publications: links to papers, preprints
   - GitHub repos: code repositories (if available)

   **Common to both:**
   - Links: websites, publications, databases, references
   - Technical details: AI methods, system architecture, scientific background
   - Events: important milestones, launches, publications
   - Partnerships: collaborations (if any)

4. **Create case file**
   - Determine directory: `cases/commercial/` or `cases/research/`
   - Generate slug: lowercase, hyphens, no special chars (e.g., "company-name")
   - Create file: `{slug}.md`

5. **Structure the file**
   - YAML frontmatter following `YAML_FIELDS.md` exactly
   - All required fields filled
   - Markdown content with proper sections
   - YAML blocks (not JSON) for structured data in content sections
   - Valid YAML syntax throughout

6. **Validate before saving**
   - All required fields present
   - YAML is valid (can be parsed)
   - Structure matches `YAML_FIELDS.md`
   - No null/undefined values in frontmatter
   - Proper file location

7. **Save and present**
   - Save file to correct directory
   - Present to user: "Created new case at `cases/{commercial|research}/{slug}.md`"
   - User reviews and validates

**Output:** New case file ready for commit/PR


## File Format

- **Format:** Markdown with YAML frontmatter
- **Structure:** See `YAML_FIELDS.md` for complete field documentation
- **Structured data:** Use YAML blocks (not JSON) in Markdown content sections
- **Location:** `cases/commercial/` or `cases/research/` based on entity_type

## Quality Standards

1. **Completeness** - All required fields present, detailed descriptions
2. **Accuracy** - Verified facts, working links, correct dates
3. **Currency** - Up-to-date information, recent research dates
4. **Structure** - Follows `YAML_FIELDS.md` exactly
5. **Validity** - All YAML parses correctly

## Success Criteria

Project is successful when:
- ✅ All cases have complete descriptions
- ✅ Data is regularly updated and validated
- ✅ Format is convenient for both humans and AI
- ✅ Repository is actively used by community
- ✅ Contribution process works efficiently
