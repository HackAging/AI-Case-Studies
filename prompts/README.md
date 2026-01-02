# Prompts for Case Management

This directory contains ready-to-use prompts for AI agents in Cursor to work with AI longevity case studies.

## Available Prompts

### 1. `find-new-cases.md`
Prompt for finding new cases that are not yet in the database.

**Usage:**
- Copy the prompt into Cursor
- AI agent will analyze existing cases and find new ones
- Results will be proposed for addition to the project

### 2. `add-new-case.md`
Prompt for adding a completely new case study to the repository.

**Usage:**
- Insert the case name or company name in the prompt
- AI agent will verify the case doesn't exist, conduct deep research, and create a complete case file
- The new case will be saved in the appropriate directory (`cases/commercial/` or `cases/research/`)

### 3. `enrich-case.md`
Prompt for enriching an existing case with additional information.

**Usage:**
- Insert the case name or company name in the prompt
- AI agent will gather additional information and validate completeness
- Results will be saved to the corresponding file

## How to Use

1. Open the desired prompt file in this directory
2. Copy the contents
3. Paste into Cursor Chat
4. If needed, insert specific values (case name, company, etc.)
5. Follow the AI agent's instructions

## Project Structure

Before using prompts, make sure you understand the project structure:

- `cases/commercial/` - Commercial companies (32 cases)
- `cases/research/` - Research projects (28 cases)
- Format: Markdown with YAML frontmatter
- See `YAML_FIELDS.md` for field structure
