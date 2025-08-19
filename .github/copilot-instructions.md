# GitHub Profile Repository - AshabaJasper/AshabaJasper

This is a GitHub profile repository that displays on Ashaba Joshua Jasper's GitHub profile page. The repository contains a README.md file that serves as the profile introduction and showcase.

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively

### Repository Overview
- This is a special GitHub profile repository (username/username format)
- Contains only README.md file that displays on the GitHub profile page
- No build processes, dependencies, or runnable applications
- Focus is on content management, markdown formatting, and profile optimization

### Basic Repository Operations
- Check repository status: `git status` -- completes in under 1 second
- View recent commits: `git log --oneline -10` -- completes in under 1 second  
- View file contents: `cat README.md` -- completes in under 1 second
- Count lines in README: `wc -l README.md` -- completes in under 1 second

### Working with the README.md
- Always make backup before major changes: `cp README.md README.md.backup`
- Edit using text editor: `nano README.md` or `vim README.md`
- Preview changes with: `git diff README.md`
- Stage changes: `git add README.md`
- Commit changes: `git commit -m "Update profile README with [description]"`

## Validation

### Content Validation Steps
- ALWAYS validate markdown syntax after making changes
- Check line count to ensure reasonable length: `wc -l README.md` (current: ~91 lines)
- **CRITICAL**: Check for trailing whitespace: `grep -n ' $' README.md` (WARNING: Current README has trailing whitespace on lines 1-3, 5, 7-8)
- Check for broken markdown formatting: manually review in editor

### Manual Testing Scenarios
- After making any changes to README.md:
  1. Run `git diff README.md` to review all changes
  2. Check that badges and links follow consistent formatting
  3. Verify all sections maintain proper markdown structure
  4. Ensure contact information and social links are current
  5. Validate that tech stack badges are properly formatted
  6. Review GitHub stats section for accuracy

### Link Validation (Limited)
- GitHub API access is blocked in this environment
- External badge services (shields.io) may have connectivity issues
- Focus on structural validation rather than live link checking
- Use `grep -E 'https?://' README.md` to find all URLs for manual review

## Common Tasks

### Profile Content Updates
- Tech stack updates: Modify badges in the "💻 Tech Stack" section
- Contact info updates: Update links in "🌐 Connect With Me" section  
- Goals updates: Modify checklist in "🎯 2025 Goals" section
- Featured projects: Update "🚀 Featured Projects" section

### Markdown Structure Maintenance
- Section headers use `##` (h2) format consistently
- Subsections use `###` (h3) format for tech categories
- Badge images use consistent `![Name](URL)` format
- Links use `[Text](URL)` format consistently

### Common Issues and Fixes
- **Trailing whitespace cleanup**: `sed -i 's/[ \t]*$//' README.md` (removes trailing whitespace)
- **Line ending normalization**: `dos2unix README.md` (if available, converts CRLF to LF)
- **Markdown formatting**: Ensure consistent spacing between sections
- Check for uncommitted changes: `git status`
- View repository history: `git log --oneline -10`
- Create branches for major updates: `git checkout -b update/profile-2025`
- Always commit with descriptive messages

## File Structure Reference

### Repository Root
```
.
├── .git/           # Git repository metadata
├── .github/        # GitHub-specific files (workflows, templates)
└── README.md       # Profile README displayed on GitHub profile
```

### Current README.md Structure
- Line 1-7: Profile header with name, title, and coding GIF
- Line 8-16: About Me section with current focus areas
- Line 17-32: Connect With Me social links
- Line 34-57: Tech Stack with categorized badges
- Line 58-63: GitHub Stats widgets
- Line 65-74: Featured Projects section
- Line 75-81: 2025 Goals checklist
- Line 83-91: Collaboration info and contact

## Important Notes
- This repository has no build, test, or deployment processes
- All changes are content-focused (README.md updates)
- Repository serves as GitHub profile showcase only
- No dependencies, package managers, or external tools required
- Git operations are fast (all complete in under 1 second)
- Focus on content quality, markdown structure, and profile optimization

## Validation Checklist
Before committing any changes:
- [ ] Run `git status` to see what files changed
- [ ] Run `git diff README.md` to review all modifications  
- [ ] Check line count hasn't grown excessively: `wc -l README.md`
- [ ] Verify markdown syntax is correct
- [ ] Ensure all sections maintain consistent formatting
- [ ] Confirm badges and links follow established patterns
- [ ] Test that contact information is current and accurate