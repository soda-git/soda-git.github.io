# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## ⚠️ IMPORTANT: Read AI_ASSISTANT_RULES.md First

**Before doing any work in this repository, you MUST read and follow the comprehensive guidelines in `AI_ASSISTANT_RULES.md`.**

This file contains detailed rules for:
- Code style and design standards
- Development workflow and best practices
- Content management and file organization
- Testing and deployment procedures
- AI collaboration guidelines

## Project Overview

This is a GitHub Pages static website repository for a personal homepage called "Soda Code". It's a Chinese-language personal portfolio platform featuring travel planning, blogs, tools, and creative works.

## Development Commands

### Basic Git Workflow
```bash
# Check status
git status

# Add changes
git add .

# Commit (follow AI_ASSISTANT_RULES.md for commit message format)
git commit -m "feat: 添加新功能描述"

# Deploy to GitHub Pages (push = immediate live deployment)
git push origin master
```

### No Build Process Required
- Static files served directly by GitHub Pages
- Open `index.html` in browser for local testing
- Push to master branch = immediate deployment
- 1-2 minutes deployment time

## Architecture Overview

### File Structure
```
soda-git/
├── index.html                  # Main homepage
├── travel/                     # Travel planning pages
├── blog/                       # Tech blog (reserved)
├── tools/                      # Utility tools (reserved)  
├── creative/                   # Creative works (reserved)
├── assets/                     # Static resources
├── README.md                   # Project documentation
└── AI_ASSISTANT_RULES.md      # ⭐ AI development guidelines
```

### Key Technical Details
- **No external dependencies**: Vanilla HTML, CSS, JavaScript only
- **Inline styles**: CSS embedded in HTML files for GitHub Pages compatibility
- **Chinese language**: All content in Chinese with `lang="zh-CN"`
- **Responsive design**: Mobile-first approach
- **Direct deployment**: Push to master = live site

## Working with This Repository

1. **Always read `AI_ASSISTANT_RULES.md` first** for complete guidelines
2. **Follow the design system** defined in the rules file
3. **Test thoroughly** before pushing (push = immediate deployment)
4. **Use Chinese language** for all content
5. **Maintain responsive design** across all devices
6. **Follow git commit conventions** specified in the rules

## Reference Files

- `AI_ASSISTANT_RULES.md` - Complete development guidelines (READ THIS FIRST)
- `hulunbeier_travel_guide.html` - Design reference template
- `index.html` - Main homepage structure
- `README.md` - Project documentation