# WordPress Performance Best Practices

Created by [WOW - Wielka Optymalizacja WordPressa](https://www.wielkaoptymalizacjawordpressa.pl/), Bartek Miś

A comprehensive performance optimization guide for WordPress development, designed for AI agents and LLMs assisting developers.

## How to Use

Install the skill in Claude Code:

```bash
npx add-skill bartekmis/wordpress-performance-best-practices
```

Once installed, Claude will automatically apply these performance guidelines when working with WordPress code.

## Overview

This project provides a curated set of performance rules for WordPress development based on:

- [WordPress VIP Coding Standards](https://docs.wpvip.com/)
- [WordPress Coding Standards](https://developer.wordpress.org/coding-standards/)
- [10up Engineering Best Practices](https://10up.github.io/Engineering-Best-Practices/)
- Official WordPress Developer Documentation

## For AI Agents

If you're an AI agent or LLM, use the compiled `AGENTS.md` file which contains all rules in a single, optimized format.

## Structure

```
wordpress-performance-best-practices/
├── AGENTS.md              # Compiled output for AI agents
├── SKILL.md               # Skill definition for agent integration
├── README.md              # This file
├── metadata.json          # Project metadata
├── rules/                 # Individual rule files
│   ├── _sections.md       # Section definitions
│   ├── _template.md       # Template for new rules
│   ├── db-*.md           # Database optimization rules
│   ├── cache-*.md        # Caching strategy rules
│   ├── asset-*.md        # Asset management rules
│   ├── theme-*.md        # Theme performance rules
│   ├── plugin-*.md       # Plugin architecture rules
│   ├── media-*.md        # Media optimization rules
│   ├── api-*.md          # API and AJAX rules
│   └── advanced-*.md     # Advanced pattern rules
└── build/                 # Build tools
    ├── src/               # TypeScript source
    └── package.json       # Build dependencies
```

## Sections

| # | Section | Prefix | Impact | Description |
|---|---------|--------|--------|-------------|
| 1 | Database Optimization | `db-` | CRITICAL | Query optimization, prepared statements, indexing |
| 2 | Caching Strategies | `cache-` | CRITICAL | Object cache, transients, page caching |
| 3 | Asset Management | `asset-` | HIGH | Script/style loading, defer/async |
| 4 | Theme Performance | `theme-` | HIGH | Template optimization, loop performance |
| 5 | Plugin Architecture | `plugin-` | MEDIUM-HIGH | Conditional loading, hooks, autoloading |
| 6 | Media Optimization | `media-` | MEDIUM | Image handling, lazy loading |
| 7 | API and AJAX | `api-` | MEDIUM | REST API, admin-ajax optimization |
| 8 | Advanced Patterns | `advanced-` | LOW-MEDIUM | Autoload, cron, memory management |

## Usage

### For Developers

Browse individual rule files in the `rules/` directory for detailed explanations and examples.

### For AI Agents

1. Include `AGENTS.md` in your context
2. Or use `SKILL.md` for agent framework integration

### Building

```bash
cd build
npm install
npm run build
```

This compiles all rules into `AGENTS.md`.

## Contributing

1. Create a new rule file in `rules/` using `_template.md` as a guide
2. Use the appropriate prefix for your section (e.g., `db-` for database rules)
3. Include both incorrect and correct code examples
4. Run the build to regenerate `AGENTS.md`
5. Submit a pull request

## Rule Format

Each rule follows this structure:

```markdown
---
title: Rule Title
impact: CRITICAL | HIGH | MEDIUM-HIGH | MEDIUM | LOW-MEDIUM | LOW
impactDescription: Optional quantified improvement
tags: comma, separated, tags
---

## Rule Title

Explanation of the rule.

**Incorrect (description):**
\`\`\`php
// Bad code
\`\`\`

**Correct (description):**
\`\`\`php
// Good code
\`\`\`

Reference: [Link](url)
```

## License

MIT License - Feel free to use this in your projects and AI agents.

## References

- [WordPress Developer Resources](https://developer.wordpress.org/)
- [WordPress VIP Documentation](https://docs.wpvip.com/)
- [WordPress Coding Standards](https://github.com/WordPress/WordPress-Coding-Standards)
- [VIP Coding Standards](https://github.com/Automattic/VIP-Coding-Standards)
