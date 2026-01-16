# WordPress Performance Best Practices Skill

## Metadata

- **Name:** wordpress-performance-best-practices
- **Version:** 1.0.0
- **Description:** Performance optimization guidelines for WordPress development
- **Author:** WordPress Performance Community

## Trigger Conditions

This skill should be activated when:

1. Writing or reviewing WordPress PHP code
2. Working with WordPress themes or plugins
3. Optimizing WordPress database queries
4. Implementing caching in WordPress
5. Working with WordPress REST API or AJAX
6. Handling media uploads in WordPress
7. Reviewing WordPress code for performance issues

## Keywords

- WordPress
- WP_Query
- wpdb
- transients
- object cache
- wp_enqueue_script
- wp_enqueue_style
- add_action
- add_filter
- plugin development
- theme development
- REST API
- admin-ajax
- wp-cron

## Instructions for Agents

When this skill is active:

1. **Review code against rules**: Check code for violations of the performance rules in AGENTS.md
2. **Suggest improvements**: When violations are found, suggest the correct implementation
3. **Explain impact**: Communicate the performance impact of violations
4. **Prioritize by impact**: Address CRITICAL and HIGH impact issues first
5. **Consider context**: Some rules may not apply in all situations

## Rule Categories

| Priority | Section | When to Check |
|----------|---------|---------------|
| 1 | Database Optimization | Any `$wpdb` usage, WP_Query, get_posts() |
| 2 | Caching Strategies | Data fetching, API calls, expensive computations |
| 3 | Asset Management | wp_enqueue_script/style, frontend code |
| 4 | Theme Performance | Template files, theme functions |
| 5 | Plugin Architecture | Plugin code, hooks, activation |
| 6 | Media Optimization | Image handling, uploads, galleries |
| 7 | API and AJAX | REST endpoints, admin-ajax handlers |
| 8 | Advanced Patterns | High-traffic optimizations, cron, autoload |

## Integration

### Claude Code

Add to your project's `CLAUDE.md`:

```markdown
When working with WordPress code, follow the rules in:
/path/to/wordpress-performance-best-practices/AGENTS.md
```

### Other AI Agents

Include the contents of `AGENTS.md` in your system prompt or context when working with WordPress projects.

## Example Usage

### Code Review Prompt

```
Review this WordPress code for performance issues using the WordPress Performance Best Practices rules:

[code here]
```

### Implementation Prompt

```
Implement [feature] in WordPress following the WordPress Performance Best Practices, particularly the caching and database optimization rules.
```
