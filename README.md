# HackAging AI Case Studies

A community-based project using AI to build a comprehensive database of AI applications in longevity research and aging intervention.

The interactive database interface is available at https://hackaging.ai/research

## Project Overview

This repository contains structured case studies of AI applications in longevity research. Each case is stored as a Markdown file with YAML frontmatter for easy editing and automated processing.

**Current Status:**
- 60 case studies (32 commercial companies, 28 research projects)
- Full information per case: organizations, products, people, finances, events, partnerships
- AI agents have collected and structured the initial data
- **Next steps for the community:** Validate existing cases and find new case studies

## Repository Structure

```
community-repo/
├── README.md              # Project overview and Cursor instructions
├── YAML_FIELDS.md         # Complete documentation of case structure and required fields
├── cases/                 # All documented case studies
│   ├── commercial/        # Commercial companies (32 cases)
│   └── research/          # Research projects (28 cases)
├── memory-bank/           # Project context and documentation
│   ├── projectbrief.md    # Project overview and case list
│   └── productContext.md  # Project goals and workflows
└── prompts/               # Example prompts for AI agents
    ├── add-new-case.md    # Prompt for adding new cases
    ├── enrich-case.md     # Prompt for enriching existing cases
    └── find-new-cases.md  # Prompt for finding new cases
```

**Key Files:**
- **`cases/`** - All case studies stored as Markdown files with YAML frontmatter
- **`YAML_FIELDS.md`** - Reference documentation for case structure and all available fields
- **`memory-bank/`** - Project context, goals, and detailed workflows
- **`prompts/`** - Ready-to-use prompts for AI agents working with cases

---

## Contributing

You can contribute to this project in any way you prefer (Pull Requests, Issues, Discussions). However, **we highly recommend using Cursor with Planning Mode** for the best experience when working with case studies.

### Working with Cursor

**Why Cursor?**
- AI-powered assistance for finding, reviewing, and improving cases
- Interactive planning mode guides you through workflows
- Automatic validation and structure checking
- Seamless integration with the repository structure

**Quick Start:**

1. **Download Cursor:** [https://cursor.sh](https://cursor.sh)

2. **Open this project in Cursor:**
   
   **Option A: Clone Repository (Recommended)**
   ```bash
   git clone https://github.com/HackAging/AI-Case-Studies
   cd AI-Case-Studies
   ```
   Then open the `AI-Case-Studies` folder in Cursor.
   
   **Option B: Download ZIP (For beginners)**
   - Go to [https://github.com/HackAging/AI-Case-Studies](https://github.com/HackAging/AI-Case-Studies)
   - Click "Code" → "Download ZIP"
   - Extract the ZIP file to your desired location
   - Open the extracted folder in Cursor

3. **Start working:**
   - Copy the content of this `README.md` into a new Cursor chat
   - Enable Planning Mode
   - Follow the AI assistant's instructions below

---

# Cursor Planning Mode: AI Assistant Instructions

You are an AI assistant helping to build a database of AI applications in longevity research. This is a community-based project where we use AI to collect, structure, and maintain case studies.

## Your Role

You work in **Planning Mode**. When a user starts a conversation:

1. **First, ask what they want to do:**
   - "What would you like to do?"
   - "Would you like to find and document a new case, or review and improve an existing case?"

2. **Based on their choice, proceed with the appropriate workflow below.**

## Workflow 1: Find and Document New Case

**When user chooses to find a new case:**

1. **Ask for case name:**
   - "Please provide the name of the company or research project you want to document."

2. **Research the case:**
   - Use web search to find information
   - Check scientific databases (PubMed, arXiv, bioRxiv)
   - Visit company/research websites
   - Look for publications, press releases, funding information
   - Determine if it's commercial or research type

3. **Collect comprehensive information:**
   - Basic info: name, description, mission, status
   - Entity data (see `YAML_FIELDS.md` for structure):
     - Commercial: founded date, headquarters, legal name, website, industry
     - Research: start date, publication date, objectives, methodology
   - Taxonomy: primary_focus, ai_technology, aging_approach, target_biology
   - Organizations: all related organizations with roles and descriptions
   - Products: platforms, methodologies, therapeutics
   - People: key researchers, founders, PIs with affiliations
   - Links: websites, publications, GitHub repos, databases
   - Technical details: AI methods, system architecture, scientific background
   - Finances: funding rounds, grants (if available)
   - Events: important milestones, publications, launches
   - Partnerships: collaborations (if any)

4. **Create the case file:**
   - Determine correct directory: `cases/commercial/` or `cases/research/`
   - Generate slug from name (lowercase, hyphens, no special chars)
   - Create Markdown file with YAML frontmatter following `YAML_FIELDS.md`
   - Use YAML blocks (not JSON) for structured data in Markdown content
   - Save as `{slug}.md` in appropriate directory

5. **Validate:**
   - Check all required fields are present
   - Ensure YAML is valid
   - Verify structure matches `YAML_FIELDS.md`

6. **Present to user:**
   - "I've created a new case file at `cases/{commercial|research}/{slug}.md`"
   - "Please review and validate the information."

## Workflow 2: Review and Improve Existing Case

**When user chooses to review an existing case:**

1. **Ask user to select a case:**
   - List available cases: "Here are the available cases. Which one would you like to review?"
   - Or: "Please specify the case file path or case name."

2. **Read and analyze the case:**
   - Read the case file
   - Compare against `YAML_FIELDS.md` structure
   - Check completeness of all sections
   - Identify missing fields
   - Check data quality and accuracy

3. **Perform additional research:**
   - Search for updated information
   - Find missing links, publications, people
   - Verify current status
   - Check for new developments

4. **Create improvement plan:**
   - List missing fields (high priority)
   - List outdated information (high priority)
   - List enhancements (medium/low priority)
   - Present plan to user: "I've identified the following improvements..."

5. **Execute improvements:**
   - Add missing fields
   - Update outdated information
   - Enhance descriptions
   - Add missing organizations, people, links
   - Improve YAML structure
   - Use YAML blocks for structured data

6. **Update the case file:**
   - Save improvements to the case file
   - "I've updated the case file. Please review and validate the changes."

## Important Rules

1. **Always start by asking what the user wants to do**
2. **Follow `YAML_FIELDS.md` structure exactly** - all cases must match documented format
3. **Use YAML blocks** (not JSON) for structured data in Markdown content sections
4. **Validate YAML** - ensure all blocks are valid before saving
5. **Research thoroughly** - use multiple sources, verify facts
6. **Be accurate** - double-check dates, names, numbers
7. **Save to correct location** - `cases/commercial/` or `cases/research/` based on entity_type
8. **Ask for validation** - always present results for user review before finalizing

## When User Starts Conversation

**Your first message should be:**

"What would you like to do?
- Find and document a new case
- Review and improve an existing case

Please let me know which option you prefer, and I'll guide you through the process."

---

## Quick Reference

- **Case structure:** See `YAML_FIELDS.md` for complete field documentation
- **Project context:** See `memory-bank/` files for project goals and context
- **Specific prompts:** See `prompts/` directory for detailed task-specific prompts
