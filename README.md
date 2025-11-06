# Bakaliee Security Blog - Dracula Theme for Tistory

*Automatically synced with your [v0.app](https://v0.app) deployments*

[![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=for-the-badge&logo=vercel)](https://vercel.com/ciaovos2-9600s-projects/v0-tistory-theme)
[![Built with v0](https://img.shields.io/badge/Built%20with-v0.app-black?style=for-the-badge)](https://v0.app/chat/q3pTmzXv4gJ)

A complete, production-ready Tistory blog theme with Dracula dark color scheme, optimized for blockchain security content.

## Features

- **Pure HTML + CSS** - No JavaScript required, works everywhere
- **Dracula Color Palette** - Beautiful dark theme with purple, cyan, and green accents
- **Responsive Design** - Mobile-first approach, works on all devices
- **Security-Focused** - Optimized for smart contract security content
- **Code Highlighting** - Solidity syntax support with line numbers
- **Semantic HTML** - Proper structure for SEO and accessibility
- **Ready for Tistory** - Drop-in components with exact class names

## Color Palette

\`\`\`css
--bg: #282A36          /* Main background */
--surface: #1E1F29     /* Card/panel background */
--text: #F8F8F2        /* Primary text */
--accent: #BD93F9      /* Purple accent */
--accent-2: #8BE9FD    /* Cyan accent */
--success: #50FA7B     /* Green for success */
--warning: #F1FA8C     /* Yellow for warnings */
--danger: #FF5555      /* Red for errors */
\`\`\`

## File Structure

\`\`\`
tistory-theme/
├── styles.css                      # Complete CSS with all components
├── header.html                     # Site header with navigation
├── post-cards.html                 # Post card grid layout
├── article-with-toc.html          # Article with table of contents
├── code-sample-solidity.html      # Code blocks with Solidity
├── sidebar.html                    # Sidebar widgets
├── footer.html                     # Site footer
├── logo.svg                        # Logo/favicon SVG
├── favicon-usage.html             # Favicon implementation guide
├── smart-contract-security-diary.md # Markdown template
└── preview.html                    # Full page preview
\`\`\`

## Components

### A) Header / Navigation
- Logo with shield icon
- Navigation menu (Home, Tutorials, Audits, Tools, About)
- Responsive mobile layout

### B) Post Cards
- 2-column grid (1 column on mobile)
- Title, date, tags, excerpt
- "Read" button with hover effects

### C) Article Layout
- Main content area with TOC sidebar
- Headings (h1-h3) with proper hierarchy
- Callouts (tip, warning, danger, info)
- Tables, blockquotes, figures
- Tag list

### D) Code Blocks
- Filename header with copy button
- Line numbers (pure CSS)
- Solidity syntax highlighting
- Dark background with proper contrast

### E) Sidebar Widgets
- Search box
- Popular posts list
- Tag cloud with size variations

### F) Footer
- Copyright notice
- Social links (Github, X, RSS)
- Centered layout

### G) Logo/Favicon
- Shield with chain link design
- SVG format for scalability
- Purple and cyan colors

### H) Security Diary Template
- Markdown template for vulnerability reports
- Sections: Overview, Findings, PoC, Impact, Mitigation
- Code blocks for Solidity examples
- Vulnerability checklist table

## Quick Start

### Preview

Open `tistory-theme/preview.html` in your browser to see all components in action.

### For Tistory

1. **Upload CSS**
   - Go to Tistory Admin → Skin → Edit HTML
   - Copy contents of `tistory-theme/styles.css` into the CSS section

2. **Update HTML**
   - Copy components from individual HTML files
   - Paste into appropriate sections of your Tistory skin

3. **Add Logo**
   - Upload `tistory-theme/logo.svg` to your Tistory file manager
   - Update the `<link rel="icon">` tag in your HTML

## Usage

### Writing Posts

Use the `smart-contract-security-diary.md` template for security articles:

\`\`\`markdown
# Smart Contract Security Diary: [Vulnerability Name]

**Date:** 2025-01-XX
**Severity:** 🔴 Critical
**CWE:** [CWE-XXX]

## Overview
...
\`\`\`

### Code Blocks

Wrap Solidity code in the codebox structure:

\`\`\`html
<div class="codebox with-lines">
  <div class="code-header">
    <span class="code-filename">Contract.sol</span>
    <span class="code-copy">Copy</span>
  </div>
  <div class="code-content">
    <pre><code class="language-solidity">
      <!-- Your Solidity code here -->
    </code></pre>
  </div>
</div>
\`\`\`

### Callouts

Use callouts for important information:

\`\`\`html
<div class="callout tip">
  <div class="callout-title">💡 Key Takeaway</div>
  <p>Your important message here</p>
</div>
\`\`\`

Available types: `tip`, `warning`, `danger`, `info`

## Customization

### Colors

Edit the `:root` variables in `styles.css`:

\`\`\`css
:root {
  --accent: #BD93F9;  /* Change primary accent color */
  --accent-2: #8BE9FD; /* Change secondary accent */
  /* ... other colors ... */
}
\`\`\`

### Typography

Change fonts in the `html, body` rule:

\`\`\`css
html, body {
  font-family: Pretendard, "Noto Sans KR", system-ui, sans-serif;
}
\`\`\`

### Layout Width

Adjust max-width in `.container`:

\`\`\`css
.container {
  max-width: 980px; /* Change to your preferred width */
}
\`\`\`

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Deployment

Your project is live at:

**[https://vercel.com/ciaovos2-9600s-projects/v0-tistory-theme](https://vercel.com/ciaovos2-9600s-projects/v0-tistory-theme)**

## Build your app

Continue building your app on:

**[https://v0.app/chat/q3pTmzXv4gJ](https://v0.app/chat/q3pTmzXv4gJ)**

## How It Works

1. Create and modify your project using [v0.app](https://v0.app)
2. Deploy your chats from the v0 interface
3. Changes are automatically pushed to this repository
4. Vercel deploys the latest version from this repository

## License

MIT License - Free to use and modify

## Credits

- **Theme:** Dracula (https://draculatheme.com/)
- **Design:** Bakaliee Security
- **Platform:** Tistory

---

**Made with 🦇 by Bakaliee Security**
