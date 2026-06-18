# ULI - Useful Links and Information

A curated collection of useful links, articles, cheatsheets, and reference materials for developers and tech enthusiasts.

## About

ULI (Useful Links and Information) is a knowledge base repository designed to store and organize:
- Copied articles and blog posts
- Curated link collections
- Quick reference cheatsheets
- Reusable templates

This repository helps preserve valuable information and makes it easily accessible.

## Repository Structure

```
uli/
├── README.md                    # This file - main overview
├── AGENT.md                     # Instructions for AI agents
├── articles/                    # Copied articles with metadata
│   ├── programming/             # Programming languages, frameworks
│   ├── devops/                  # DevOps, infrastructure, cloud
│   └── misc/                    # Other technical articles
├── links/                       # Curated link collections
│   ├── programming.md           # Programming resources
│   ├── tools.md                 # Useful tools and utilities
│   ├── learning.md              # Tutorials, courses, books
│   └── communities.md           # Forums, newsletters, communities
├── cheatsheets/                 # Quick reference guides
│   ├── git.md
│   ├── docker.md
│   └── ...
└── templates/                   # Reusable templates
    └── entry-template.md        # Template for new entries
```

## Quick Navigation

### 📚 Articles
- [Programming Articles](./articles/programming/)
- [DevOps Articles](./articles/devops/)
- [Miscellaneous Articles](./articles/misc/)

### 🔗 Links
- [Programming Resources](./links/programming.md)
- [Tools & Utilities](./links/tools.md)
- [Learning Resources](./links/learning.md)
- [Communities](./links/communities.md)

### 📋 Cheatsheets
- [Git Cheatsheet](./cheatsheets/git.md)
- [Docker Cheatsheet](./cheatsheets/docker.md)

### 📝 Templates
- [Entry Template](./templates/entry-template.md)

## How to Use This Repository

### Adding New Content

#### 1. Adding an Article
1. Place the file in the appropriate `articles/<category>/` directory
2. Use the filename format: `YYYY-MM-DD-slug.md`
3. Include frontmatter with metadata (see [AGENT.md](./AGENT.md))
4. Always credit the original source

Example filename: `2024-06-18-react-performance-optimization.md`

#### 2. Adding a Link
1. Open the appropriate file in the `links/` directory
2. Add your link using the format:
   ```markdown
   - [Link Title](https://url.com) - Brief description. *Added: YYYY-MM-DD*
   ```
3. Group related links under category headings

#### 3. Adding a Cheatsheet
1. Create a new file in `cheatsheets/` directory
2. Use a descriptive name (e.g., `kubernetes.md`)
3. Include frontmatter with creation date and tags
4. Use clear headings and code examples

### Contribution Guidelines

- ✅ **Do**: Add useful, referenceable information
- ✅ **Do**: Include dates and sources
- ✅ **Do**: Organize content logically
- ✅ **Do**: Verify links work before adding
- ❌ **Don't**: Add personal notes (use a separate `notes/` directory if needed)
- ❌ **Don't**: Copy content that prohibits redistribution
- ❌ **Don't**: Add duplicate entries

## Metadata Standards

Every content file should include:

| Field | Required | Description |
|-------|----------|-------------|
| `date_added` | Yes | When the content was added to this repo |
| `source` | If copied | Original URL or author |
| `category` | Yes | Primary category |
| `tags` | Yes | Keywords for searchability |

## Searching the Repository

Use `grep` or GitHub's search to find content:

```bash
# Search for all files containing "react"
grep -r "react" --include="*.md" .

# Search for files added in June 2024
find . -name "2024-06-*.md"
```

## Maintenance

This repository is maintained by:
- Human contributors
- AI agents (see [AGENT.md](./AGENT.md) for agent instructions)

### Regular Tasks
- Monthly: Verify all external links
- Quarterly: Archive outdated content
- As needed: Reorganize and refactor structure

## License

This repository contains:
- Original content: MIT License (or as specified)
- Copied content: Respects original copyright and licensing

Always check the original source for licensing information when copying content.

## Getting Started

1. Clone the repository
2. Browse the structure to find what you need
3. Add new content following the guidelines
4. Submit a pull request with your changes

---

**Last Updated:** 2024-06-18  
**Repository Created:** 2024-06-18

For detailed agent instructions, see [AGENT.md](./AGENT.md)
