# Contributing to GoMining Agent Skills

Thank you for your interest in contributing to the GoMining Agent Skills repository!

## How to Contribute

### Reporting Issues

- Check existing issues before creating a new one
- Provide clear descriptions and context
- Include relevant skill names and file paths

### Suggesting Improvements

- Open an issue describing the improvement
- Explain the use case and benefits
- Reference official GoMining documentation when possible

### Submitting Changes

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement-name`)
3. Make your changes following the guidelines below
4. Test your changes
5. Commit with clear messages
6. Push to your fork
7. Open a Pull Request

## Skill Structure Guidelines

### SKILL.md Format

Every skill must have a `SKILL.md` file with:

```yaml
---
name: skill-name
description: "Clear, comprehensive description of the skill's scope"
license: Apache-2.0
compatibility: "Compatible with Claude Code, Codex, and all Agent Skills spec tools."
metadata:
  author: gomining
  version: "1.0"
  tags: ["relevant", "tags"]
  triggers: ["trigger phrase 1", "trigger phrase 2"]
---
```

### skill.json Format

Every skill must also have a `skill.json` file with:

```json
{
  "name": "skill-name",
  "description": "Concise description of the skill's scope",
  "triggers": ["trigger phrase 1", "trigger phrase 2"],
  "enabled": true,
  "type": "knowledge"
}
```

### Content Guidelines

1. **Accuracy**: All information must align with official GoMining documentation
2. **Structure**: Use clear headings, tables, and lists
3. **Links**: Reference official resources with full URLs
4. **FAQs**: Include commonly asked questions
5. **References**: Link to supporting files in `references/`

### Reference Files

- Place detailed documentation in `references/` subdirectory
- Use descriptive, uppercase filenames with standard prefixes:
  - `FAQ-TOPIC.md` — Frequently asked questions
  - `INSTRUCTION-ACTION.md` — Step-by-step guides
  - `TOPIC.md` — Deep-dive reference material
- Cross-reference from main SKILL.md file

## Writing Style

- Use clear, concise language
- Prefer tables for structured data
- Include code blocks for diagrams using ASCII art
- Avoid marketing language; focus on factual information
- Keep descriptions neutral and informative

## Testing Changes

Before submitting:

1. Verify all internal links work
2. Check YAML frontmatter is valid
3. Ensure tables render correctly
4. Validate URLs are accessible
5. Review for spelling and grammar

## Code of Conduct

- Be respectful and constructive
- Focus on improving the documentation
- Cite sources for new information
- Acknowledge others' contributions

## Questions?

Open an issue for any questions about contributing.
