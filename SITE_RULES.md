# PulsePoint Site Rules

These rules apply to **every article** — new and existing. Check every article against these before publishing.

---

## 1. Header — PulsePoint Must Link Home
The site name in the header **MUST** be a clickable link to `index.html` with the full branding:
```html
<h1><a href="index.html" style="color:white;text-decoration:none">PulsePoint</a> <span>Daily Trends</span></h1>
```
**Rule:** "PulsePoint" is always clickable → home. "Daily Trends" always appears next to it.

---

## 2. Article Header (top of every article page)
After the nav bar, the article must open with:
- Category tag (color-coded)
- Article title
- Date + read time
- **Author byline** ← REQUIRED

Byline format (insert after the meta line, before the hero image):
```html
<p style="color:#888;font-size:0.9rem;margin-bottom:0.5rem;">
  By <strong>Puckwudgie 🐸</strong> &middot; Updated [Date]
</p>
```
**Every article must have this exact byline.** Use today's date. The date in the byline must match the date shown in the article's meta line.

---

## 3. Bottom of Every Article (required elements, in order)
After the article text ends, before the footer:

**A) Back button:**
```html
<div style="text-align:center;padding:2rem">
  <a href="index.html" style="display:inline-flex;align-items:center;gap:0.5rem;background:#1d3557;color:white;padding:0.75rem 1.5rem;border-radius:8px;text-decoration:none;font-weight:600;">← Go Back</a>
</div>
```

**B) Share buttons:**
```html
<div style="max-width:900px;margin:0 auto 2rem;padding:0 2rem;text-align:center">
  <p style="font-size:0.85rem;color:#888;margin-bottom:0.75rem;">Share this article</p>
  <div style="display:flex;gap:0.75rem;justify-content:center;flex-wrap:wrap">
    <a href="https://twitter.com/intent/tweet?text=[TITLE]&url=[URL]" target="_blank" style="display:inline-flex;align-items:center;gap:0.4rem;background:#1a1a2e;color:white;padding:0.5rem 1rem;border-radius:6px;text-decoration:none;font-size:0.85rem;font-weight:600;">𝕏 Post</a>
    <a href="https://www.facebook.com/sharer/sharer.php?u=[URL]" target="_blank" style="display:inline-flex;align-items:center;gap:0.4rem;background:#1d3557;color:white;padding:0.5rem 1rem;border-radius:6px;text-decoration:none;font-size:0.85rem;font-weight:600;">f Facebook</a>
    <button onclick="navigator.clipboard.writeText(window.location.href);this.textContent='✓ Copied!';setTimeout(()=>this.textContent='🔗 Copy Link',2000)" style="background:[CATEGORY_COLOR];color:white;padding:0.5rem 1rem;border:none;border-radius:6px;font-size:0.85rem;font-weight:600;cursor:pointer;">🔗 Copy Link</button>
  </div>
</div>
```

---

## 4. Internal Links (SEO + Engagement)
When one article mentions a topic that has its own dedicated article on the site, link to it inline. Examples:
- Article mentioning AI coding → link to `article-claude-apps.html`
- Article mentioning robots/AI replacing jobs → link to `article-robot-jobs.html`
- Article about data centers → link to `article-datacenters.html`
- Article about GTA VI → link to `article-gta-vi.html`
- Article about streaming/music → link to `article-chappell-roan.html`
- Article about Boston/NYC marathon → link to `article-marathon-underdog.html` or `article-nyc-half.html`
- Article about TikTok trends → link to `article-tiktok.html`

Link style: `<a href="[slug].html" style="color:[category-color];text-decoration:underline;">[anchor text]</a>`
Aim for 2–3 internal links per article, naturally woven into the text.

| Category | Author | Role |
|----------|--------|------|
| Tech | Morgan Vale | Tech & Science Editor |
| Sports | Derek Sloane | Sports & Outdoors Editor |
| Culture | Jade Reyes | Culture & Entertainment Editor |
| Viral | Casey Quinn | Viral & Internet Editor |
| Music | Ryan Cho | Music & Gaming Editor |
| Sci-Fi/Unexplained | Alex Mercer | Sci-Fi & Unexplained Editor |

---

## Category Colors (for share button accent)
- Tech: #457b9d
- Sports: #2a9d8f
- Culture: #e9c46a
- Viral: #f4a261
- Music: #9b5de5
