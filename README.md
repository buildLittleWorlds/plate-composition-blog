# AI, Writing, and Work

This is the instructor example blog for ENGL 170 (Composition II) at Lindenwood University, Spring 2026.

## What's Here

- **Blog posts** exploring AI, writing, and intellectual work
- **`_template.html`** — starter file for new posts
- **`transcripts/`** — source transcripts used for writing posts
- **`drafts/`** — work in progress

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

You can use `_template.html` as a starting point for your own posts. The key structural elements:

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
