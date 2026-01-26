# Claude Guidelines for dubplanner-issues

## Release Notes

When asked to create release notes, **always prepend** new entries to `RELEASE_NOTES.md`.

### Format

Use this exact format for each release:

```markdown
---

## Week of [Start Date] - [End Date], [Year]

### New Features

#### [Feature Name]
- **[Sub-feature]** - Description

### Improvements

#### [Category]
- **[Improvement]** - Description

### Bug Fixes

- **[Fix title]** - Description

---
```

### Rules

1. **Prepend, don't append** - New releases go at the top, right after the `# DubPlanner Release Notes` heading
2. **Use horizontal rules** - Each release section is wrapped with `---` separators
3. **Week-based grouping** - Group changes by week, using the Sunday-Saturday range
4. **User-facing language** - Write for end users, not developers. Avoid technical jargon
5. **Bold feature names** - Use `**bold**` for feature/fix names followed by a description
6. **Categorize appropriately**:
   - **New Features** - Brand new functionality
   - **Improvements** - Enhancements to existing features
   - **Bug Fixes** - Issues that were resolved
7. **Skip internal changes** - Don't include deployment, CI/CD, or infrastructure changes unless they affect users
