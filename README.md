# AI, Writing, and Work

This is the instructor example blog for ENGL 170 (Composition II) at Lindenwood University, Spring 2026.

## What's Here

```
plate-blog/
├── index.html              # Post list
├── about.html
├── style.css
├── posts.json              # Manifest for dashboard scraper
├── _template/              # Template for new posts
│   └── index.html
├── posts/                  # All posts in individual folders
│   └── [slug]/
│       ├── index.html      # The post
│       └── transcript.md   # Source transcript (if applicable)
├── drafts/                 # Work in progress
│   └── adaptation-plans/   # Plans from CAH 205 newsletters
├── archive/                # Unused materials
│   └── unused-transcripts/
├── docs/                   # Documentation
│   ├── style-guide.md
│   └── blog-rubric.md
└── README.md
```

## Live Site

**Blog:** https://buildlittleworlds.github.io/plate-composition-blog/

**Course Dashboard:** https://buildlittleworlds.github.io/engl170-spring2026-dashboard/

The dashboard aggregates posts from all student blogs in the course network. This blog feeds into that dashboard alongside student work.

## For Students

This blog demonstrates the format and approach expected in ENGL 170. Each post:

1. Responds to a specific source (video, article, or another blog)
2. Represents the source's argument fairly before critiquing it
3. Develops an original position with evidence
4. Links to the source in the post metadata

You can use `_template/index.html` as a starting point for your own posts. The key structural elements:

- Title in `<h2>`
- Meta line with date and source link
- "The Argument" section summarizing the source
- "The Problem" or similar section with your critique
- "Why This Matters" section connecting to broader themes

## Post Structure for Dashboard

For your posts to appear on the course dashboard, your `index.html` must include:

```html
<ul class="post-list">
  <li>
    <a href="your-post.html">Post Title</a>
    <span class="date">Month Day, Year</span>
  </li>
</ul>
```

The dashboard scraper looks for this exact structure.

## Instructor Notes

This blog uses a `posts.json` manifest that the dashboard scraper reads directly (instead of parsing HTML). When adding a new post:

1. Create `posts/[slug]/index.html` (copy from `_template/`)
2. Add transcript to `posts/[slug]/transcript.md` if applicable
3. Add entry to `posts.json`
4. Add entry to `index.html`

See the main `CLAUDE.md` for detailed instructions.
