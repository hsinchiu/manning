# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple static website for a 6-year-old child named 辛曼宁 (Xin Manning). It's a single-page website built with HTML, CSS, and JavaScript, designed as a colorful, child-friendly personal portfolio.

## Architecture

- **Single Page Application**: Everything is contained in `index.html`
- **No Build Process**: Pure HTML/CSS/JS with no compilation step
- **Static Hosting**: Designed for GitHub Pages (see `CNAME` file)
- **Responsive Design**: Uses Tailwind CSS via CDN with custom CSS
- **Language**: Chinese content (simplified)

## Key Technologies

- **HTML5**: Semantic markup
- **Tailwind CSS**: Utility-first CSS framework (via CDN)
- **Google Fonts**: Nunito and Fredoka One typefaces
- **Font Awesome**: Icons
- **Vanilla JavaScript**: Interactive features

## Development

### Local Development
Since this is a static site, you can:
1. Open `index.html` directly in a browser
2. Use any local server (e.g., `python -m http.server` or `npx serve`)
3. Use Live Server extensions in code editors

### Making Changes
- All content is in `index.html`
- CSS custom properties are defined in `:root` for easy theming
- JavaScript is embedded at the bottom of the HTML file
- The site uses smooth scrolling and interactive animations

### Content Sections
1. **Header**: Welcome area with name and age
2. **Navigation**: Smooth scroll navigation to sections
3. **About Me**: Introduction with placeholder avatar
4. **Hobbies**: Six hobby cards with icons and descriptions
5. **Gallery**: Portfolio showcase (currently placeholder)
6. **Contact**: Contact form (non-functional, display only)
7. **Footer**: Copyright information

## Common Tasks

### Updating Age
Change the age number in the HTML (line 317 and line 360):
```html
<span id="age" class="age-animation text-primary-green">6</span>
```

### Adding New Content
- New sections should follow the fade-in-up animation pattern
- Use existing CSS custom properties for consistent styling
- Maintain the responsive grid layouts

### Color Scheme
All colors use CSS custom properties defined in `:root`:
- Primary colors: purple, pink, blue, yellow, green
- Accent colors: orange, teal
- Text colors: dark, medium, light

## Deployment
- This is configured for GitHub Pages deployment
- The `CNAME` file shows the custom domain
- No build process required - just commit and push changes