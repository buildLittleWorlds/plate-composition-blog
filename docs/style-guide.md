# Plate Blog: AI, Writing, and Work — Style Guide

This style guide adapts the Canvas course design to an HTML/CSS blog deployed on GitHub Pages. The aesthetic is intentionally bookish and understated—ink, cream, and sepia tones evoke a thoughtful, academic sensibility without being stuffy.

## Color Palette

| Color | Hex | CSS Variable | Usage |
|-------|-----|--------------|-------|
| Deep Ink | `#2C3E50` | `--ink-deep` | Headers, primary emphasis |
| Ink Medium | `#4A6785` | `--ink-medium` | Secondary headers, nav links |
| Warm Cream | `#F5F0E6` | `--cream` | Backgrounds, containers |
| Aged Paper | `#EDE4D3` | `--paper` | Alternate backgrounds, code blocks |
| Sepia Brown | `#8B5A2B` | `--sepia` | Accents, decorative borders |
| Soft Rust | `#A0522D` | `--rust` | Warm accent, link hover |
| Near Black | `#333333` | `--text` | Body text |
| Muted Teal | `#17A2B8` | `--teal` | Links, info callouts |

## Typography

- **Body text**: Georgia, "Times New Roman", serif
- **Headings**: Georgia, serif (same family, larger sizes)
- **Line height**: 1.7 for body text
- **Font sizes**:
  - Body: 18px
  - H1 (site title): 1.5em
  - H2 (post titles): 1.6em
  - H3 (section headings): 1.2em
  - Meta/footer: 0.85em

## Page Structure

### Header
Site header contains the blog title and navigation. Uses a subtle bottom border in warm cream tones.

```html
<header>
  <h1>AI, Writing, and Work</h1>
  <nav>
    <a href="index.html">Posts</a>
    <a href="about.html">About</a>
  </nav>
</header>
```

### Article/Post
Each post is wrapped in `<article>` with:
- H2 for the post title
- Meta line with date and source attribution
- H3 for section headings within the post
- Blockquotes for source material

```html
<article>
  <h2>Post Title</h2>
  <p class="meta">January 8, 2026 · Response to: <a href="#">Source Title</a></p>

  <p>Introduction paragraph...</p>

  <h3>Section Heading</h3>
  <p>Content...</p>

  <blockquote>
    <p>Quoted material from source.</p>
    <cite>— Speaker Name, Source Title</cite>
  </blockquote>
</article>
```

### Footer
Simple footer with site description. Uses subtle top border.

```html
<footer>
  <p>A blog about AI in writing and intellectual work.</p>
</footer>
```

## Component Styles

### Links
- Default: Muted teal (`#17A2B8`)
- Hover: Underline (no color change)
- Nav links: Ink medium (`#4A6785`)

### Blockquotes
For quoting source material:
- Background: Aged paper (`#EDE4D3`)
- Left border: 3px solid sepia (`#8B5A2B`)
- Padding: 15px 20px
- Italic text
- Citation block below quote

### Post List (Index Page)
```html
<ul class="post-list">
  <li>
    <a href="post.html">Post Title</a>
    <span class="date">January 8, 2026</span>
  </li>
</ul>
```

### Callout Boxes (Optional)
For highlighting important information within posts:

**Info (teal):**
```html
<div class="callout info">
  <p>Content here</p>
</div>
```

**Warning (amber):**
```html
<div class="callout warning">
  <p>Content here</p>
</div>
```

**Insight (sepia):**
```html
<div class="callout insight">
  <p>Content here</p>
</div>
```

## Design Principles

### No Images
This blog intentionally uses no images. All visual interest comes from:
- The color palette (ink, cream, sepia tones)
- Typography (Georgia serif at varied sizes)
- CSS-based decorative elements (borders, backgrounds)
- Whitespace and layout

This avoids complications around AI-generated imagery and keeps pages lightweight.

### Readability First
- Maximum width: 700px (optimal line length)
- Generous line height: 1.7
- Ample spacing between elements
- High contrast text on light backgrounds

### Understated Elegance
- Borders are subtle, not heavy
- Colors are muted, not bright
- Decorative elements are minimal
- Focus stays on the writing

## File Organization

```
plate-blog/
├── posts/
│   ├── index.html          # Homepage with post list
│   ├── about.html          # About page
│   ├── style.css           # Stylesheet
│   ├── _template.html      # Template for new posts
│   └── [post-name].html    # Individual posts
├── drafts/                 # Work in progress
├── transcripts/            # Source transcripts
├── style-guide.md          # This file
└── blog-rubric.md          # Evaluation criteria
```

## CSS Variables Reference

Include at the top of `style.css`:

```css
:root {
  --ink-deep: #2C3E50;
  --ink-medium: #4A6785;
  --cream: #F5F0E6;
  --paper: #EDE4D3;
  --sepia: #8B5A2B;
  --rust: #A0522D;
  --text: #333333;
  --teal: #17A2B8;
}
```

## Sample Post Structure

See `_template.html` for the standard post structure, which includes:
1. Introduction (what is this source, why engage with it)
2. Fair representation of source's argument with direct quote
3. Your response/critique
4. Development of counter-argument
5. Connection to broader themes
6. Conclusion
