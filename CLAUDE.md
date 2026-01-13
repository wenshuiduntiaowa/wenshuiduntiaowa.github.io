# CLAUDE.md - AI Assistant Guide for wenshuiduntiaowa.github.io

## Repository Overview

This is a simple **GitHub Pages** static website repository featuring Beijing tourist attractions. The site serves as a personal landing page with links to popular Beijing destinations.

**Repository Type**: GitHub Pages Static Website
**Primary Language**: HTML, CSS, JavaScript
**Target Audience**: Visitors looking for Beijing tourist information
**Deployment**: Automatically deployed via GitHub Pages

---

## Codebase Structure

```
wenshuiduntiaowa.github.io/
├── index.html          # Main landing page (Chinese/English hybrid)
├── styles.css          # External stylesheet with responsive design
├── scripts.js          # JavaScript file with basic DOM interactions
└── CLAUDE.md          # This file - AI assistant documentation
```

### File Descriptions

#### `index.html` (70 lines)
- **Purpose**: Main entry point for the website
- **Content**:
  - Header with navigation menu (Home, About, Contact)
  - Home section featuring 5 Beijing tourist attraction buttons
  - About section (placeholder content)
  - Contact section with email link
  - Footer with copyright notice
- **Special Features**:
  - Inline `<style>` block for button styling (lines 8-29)
  - External stylesheet link
  - Chinese language content for attraction names
  - Responsive button design (200px width, block display)
- **External Links**:
  - 北京野生动物园 (Beijing Wildlife Park)
  - 北京动物园 (Beijing Zoo)
  - 北京环球度假区 (Universal Beijing Resort)
  - 故宫博物院 (Palace Museum)
  - 天安门广场 (Tiananmen Square)

#### `styles.css` (78 lines)
- **Purpose**: Main stylesheet for visual design
- **Key Styles**:
  - CSS reset (lines 1-7)
  - Body styling with Arial font and light gray background
  - Dark header/navigation (#333 background)
  - White content sections with padding
  - Fixed footer at bottom of page
  - Image container with centering
  - Hover effects for navigation and buttons
- **Responsive Features**:
  - `max-width: 50%` for images
  - Auto height for images
  - Border and shadow effects

#### `scripts.js` (11 lines)
- **Purpose**: JavaScript functionality (currently minimal)
- **Current Function**:
  - DOMContentLoaded event listener
  - Console log for debugging
- **Note**: Contains Python-style comment header (author metadata)
- **Future Potential**: Can be expanded for interactive features

---

## Development Workflow

### Making Changes

1. **Always work on feature branches** starting with `claude/` prefix
2. **Test changes locally** before committing
3. **Use descriptive commit messages** in English or Chinese
4. **Push to the designated branch** (e.g., `claude/add-claude-documentation-MWGGs`)

### Git Operations

```bash
# Check current branch
git branch

# Create new feature branch
git checkout -b claude/feature-name-<session-id>

# Stage changes
git add <files>

# Commit with descriptive message
git commit -m "Descriptive message"

# Push to origin
git push -u origin claude/feature-name-<session-id>
```

### Commit Message Patterns

Looking at recent history, commits follow this pattern:
- Simple, direct messages: "Update index.html"
- Chinese messages occasionally used: "Update index.html 跳转北京动物园"

**Recommended**: Use descriptive messages that explain WHY changes were made, not just WHAT file changed.

---

## Key Conventions & Patterns

### HTML Conventions

1. **Language**: Hybrid English/Chinese content
   - HTML structure uses English (`<header>`, `<nav>`, etc.)
   - User-facing content often in Chinese (北京景点)

2. **Styling Approach**:
   - Mix of inline styles and external CSS
   - Inline styles used for button-specific customization
   - External CSS for global layout and theme

3. **Link Format**:
   - External links use `target="_blank"` to open in new tabs
   - Links styled as buttons with `.button` class
   - 200px width buttons, block display for vertical stacking

### CSS Conventions

1. **Color Scheme**:
   - Primary dark: `#333` (header, nav, footer)
   - Primary accent: `#007bff` (buttons)
   - Hover state: `#0056b3` (darker blue)
   - Background: `#f4f4f4` (light gray)
   - Content: `white` (sections)

2. **Layout**:
   - Fixed footer at bottom
   - Centered content
   - 20px padding for sections
   - Consistent spacing

3. **Reset Pattern**: CSS reset at top of file removes default browser styling

### JavaScript Conventions

1. **Event Handling**: Use `addEventListener` for DOM events
2. **Logging**: Console logging present for debugging
3. **File Header**: Python-style docstring with author/date info

---

## Important Rules for AI Assistants

### DO's ✓

1. **Preserve Chinese Content**: Keep all Chinese text intact unless explicitly asked to translate
2. **Maintain Simplicity**: This is a simple static site - don't over-engineer
3. **Test Links**: Verify external links are working before committing
4. **Responsive Design**: Ensure changes work on mobile and desktop
5. **Read Files First**: Always read existing files before suggesting modifications
6. **Use Feature Branches**: Work on `claude/` prefixed branches only
7. **Preserve External Links**: Don't modify URLs to tourist attractions without verification
8. **Keep Footer Updated**: If year changes, update copyright in footer

### DON'Ts ✗

1. **Don't Remove Chinese**: Don't translate or remove Chinese text without permission
2. **Don't Break Links**: Don't modify external URLs without testing
3. **Don't Add Complexity**: Avoid adding frameworks, build tools, or dependencies
4. **Don't Change Structure**: Maintain the simple three-section layout
5. **Don't Commit to Main**: Never push directly to main/master branch
6. **Don't Add Tracking**: No analytics or tracking scripts without explicit request
7. **Don't Create Unnecessary Files**: Keep the minimal file structure

### Security Considerations

1. **External Links**: All tourist attraction links should use HTTPS where possible
2. **Email Protection**: Contact email is displayed but consider spam protection
3. **No User Input**: Site currently has no forms - if adding, sanitize inputs
4. **HTTPS**: Ensure GitHub Pages HTTPS is enabled

---

## Common Tasks Guide

### Adding a New Tourist Attraction

1. Read `index.html` to see current structure
2. Add new `<p><a>` tag in the `#home` section (around lines 48-52)
3. Use `.button` class for consistency
4. Ensure `target="_blank"` for external links
5. Test the link before committing
6. Update spacing if needed

**Example**:
```html
<p><a href="https://example.com" target="_blank" class="button">新景点名称</a></p>
```

### Modifying Button Styles

1. Read both `index.html` (inline styles) and `styles.css`
2. Decide if change should be inline or in external CSS
3. For button-specific changes: modify inline `<style>` block (lines 8-29)
4. For global changes: modify `styles.css`
5. Test across different screen sizes

### Updating Color Scheme

1. Read `styles.css` fully
2. Identify all color values (`#333`, `#007bff`, etc.)
3. Use find/replace for consistency
4. Update both normal and hover states
5. Verify contrast ratios for accessibility

### Adding JavaScript Functionality

1. Read `scripts.js` to understand current setup
2. Add new functions inside or after `DOMContentLoaded` listener
3. Keep code simple and well-commented
4. Test in browser console before committing
5. Consider mobile compatibility

---

## Testing Checklist

Before committing changes, verify:

- [ ] All external links open correctly
- [ ] Buttons are properly styled and aligned
- [ ] Navigation menu works (hash links)
- [ ] Footer is fixed at bottom
- [ ] Page loads without console errors
- [ ] Chinese characters display correctly
- [ ] Mobile responsive design intact
- [ ] Hover effects work on buttons and nav
- [ ] No broken images or missing resources

---

## Deployment Information

- **Platform**: GitHub Pages
- **URL Format**: `https://wenshuiduntiaowa.github.io`
- **Auto-Deploy**: Pushes to main branch trigger automatic deployment
- **Build Time**: Usually 1-5 minutes
- **Cache**: Browser caching may delay visible changes

---

## Recent Activity Summary

**Last 10 Commits**: All focused on updating `index.html`
- Multiple iterative updates to the main page
- One commit specifically mentions "跳转北京动物园" (Beijing Zoo link)

**Development Pattern**:
- Frequent, small iterations
- Direct updates to index.html
- Simple, incremental improvements

---

## Future Enhancement Opportunities

If asked to improve the site, consider:

1. **SEO Optimization**: Meta tags, descriptions, Open Graph tags
2. **Accessibility**: ARIA labels, alt text, keyboard navigation
3. **Performance**: Minify CSS/JS, optimize images
4. **Interactivity**: Photo galleries, interactive maps
5. **Localization**: Full English/Chinese language toggle
6. **Mobile Menu**: Hamburger menu for better mobile UX
7. **Dark Mode**: Toggle for light/dark theme
8. **Form Validation**: If contact form is added
9. **PWA Features**: Service worker for offline access
10. **Analytics**: Privacy-respecting analytics (if requested)

---

## Questions to Ask Users

When receiving requests, clarify:

1. **Language Preference**: Should new content be in Chinese, English, or both?
2. **Target Audience**: Locals or international tourists?
3. **Link Verification**: Should AI verify links are current/working?
4. **Design Scope**: Simple changes or full redesign?
5. **Browser Support**: Which browsers/devices to test?

---

## Helpful Commands

```bash
# View git history
git log --oneline -10

# Check current status
git status

# View file contents
cat index.html

# Search for text
grep -r "北京" .

# Count lines of code
wc -l *.html *.css *.js
```

---

## Contact & Metadata

- **Author**: 34572 (from scripts.js header)
- **Created**: June 13, 2024 (from scripts.js header)
- **License**: Not specified (consider adding LICENSE file)
- **Contributing**: Not specified (consider adding CONTRIBUTING.md)

---

## Version History

- **Current Version**: CLAUDE.md v1.0
- **Last Updated**: 2026-01-13
- **Maintained By**: AI Assistant (Claude)

---

*This documentation is intended for AI assistants working on this codebase. Keep it updated as the project evolves.*
