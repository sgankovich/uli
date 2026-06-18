# Agent Guide for ULI Repository

## Purpose
This repository serves as a curated collection of useful links, articles, cheatsheets, and reference materials. As an AI agent, your role is to help maintain and organize this knowledge base.

## Repository Structure
```
uli/
├── README.md                    # Main overview and navigation
├── AGENT.md                     # This file - agent instructions
├── articles/                    # Copied articles and long-form content
│   ├── ai/                      # AI, ML, and agent-related articles
│   ├── programming/             # Programming-related articles
│   ├── devops/                  # DevOps and infrastructure articles
│   └── misc/                    # Other articles
├── links/                       # Curated link collections
│   ├── programming.md           # Programming resources
│   ├── tools.md                 # Useful tools and utilities
│   ├── learning.md              # Learning resources and tutorials
│   └── communities.md           # Communities and forums
├── cheatsheets/                 # Quick reference guides
│   ├── git.md
│   ├── docker.md
│   └── ...
└── templates/                   # Reusable templates
    └── entry-template.md        # Template for new entries
```

## Adding New Content

### 1. For Articles (copied content)
- Save in appropriate `articles/<category>/` directory
- Use filename format: `YYYY-MM-DD-slug.md` (e.g., `2024-01-15-react-hooks-guide.md`)
- Include frontmatter with metadata:
  ```markdown
  ---
  title: "Article Title"
  date_added: YYYY-MM-DD
  source: "https://original-source-url.com"
  author: "Original Author"
  category: "programming"
  tags: [react, hooks, frontend]
  ---
  ```
- Always include the original source URL at the top of the file
- Preserve original formatting when possible
- Add `[Source](url)` link at the bottom

### 2. For Links (curated collections)
- Add to appropriate file in `links/` directory
- Use this format:
  ```markdown
  ### Category Name
  - [Link Title](https://url.com) - Brief description. *Added: YYYY-MM-DD*
  ```
- Group related links under category headings
- Keep descriptions concise (1 line)
- Always include the date added

### 3. For Cheatsheets
- Save in `cheatsheets/` directory
- Use filename: `topic.md` (e.g., `git.md`, `docker.md`)
- Include frontmatter:
  ```markdown
  ---
  title: "Git Cheatsheet"
  date_created: YYYY-MM-DD
  date_updated: YYYY-MM-DD
  tags: [git, vcs, version-control]
  ---
  ```
- Use clear headings and code blocks
- Keep it practical and example-driven

## File Naming Conventions
- Use lowercase letters
- Use hyphens for spaces
- Include date prefix for time-sensitive content
- Be descriptive but concise

## Metadata Requirements
Every content file MUST include:
- **Date added/created** - When the information was added to this repo
- **Source** (if applicable) - Original URL or author
- **Category** - Primary category
- **Tags** - Relevant keywords for searchability

## Formatting Guidelines
- Use consistent Markdown formatting
- Prefer ATX-style headings (`# Heading`)
- Use fenced code blocks with language specification
- Wrap lines at 80-100 characters for readability
- Use lists for multiple items
- Include a table of contents for files > 100 lines

## Quality Standards
- Verify links are working before adding
- Check for duplicates before adding new content
- Ensure proper attribution for copied content
- Keep descriptions clear and useful
- Update dates when modifying existing content

## Workflow for Adding Content
1. Check if content already exists in the repo
2. Determine the appropriate category
3. Create or update the file following the format guidelines
4. Add metadata (date, source, tags)
5. Verify the file renders correctly
6. Commit with a descriptive message

## Example Workflow
```bash
# Adding a new article
cd /workspace/sgankovich__uli
# Copy content, add frontmatter, save to articles/programming/2024-01-15-react-hooks.md

# Adding a new link
echo "- [React Docs](https://react.dev) - Official React documentation. *Added: 2024-01-15*" \
  >> links/programming.md

# Commit changes
git add .
git commit -m "Add React hooks article and docs link"
```

## Maintenance Tasks
- Monthly: Verify all links are still valid
- Quarterly: Review and archive outdated content
- As needed: Reorganize categories when they grow too large
- Always: Keep AGENT.md updated with new conventions

## Important Notes
- Respect copyright: Only copy content that allows redistribution
- When in doubt, link to the original source rather than copying
- For personal notes, use a separate `notes/` directory
- Keep the repository focused on useful, referenceable information
