# How to edit your website

## The tool you need

Download **Visual Studio Code** (free): https://code.visualstudio.com

To edit the site:
1. Open VS Code
2. File → Open File → select `index.html`
3. Press **Ctrl+F** (Windows) or **Cmd+F** (Mac) to search for anything
4. Make your changes, then File → Save
5. Go to your GitHub repository → click `index.html` → click the pencil (edit) icon → paste your updated content → Commit changes

---

## All the things to update

### 1. Your email address
**Search for:** `your@email.com`  
**Replace with:** your actual email, e.g. `sherry.xu@manchester.ac.uk`

---

### 2. Your Substack URL
**Search for:** `YOUR-SUBSTACK-URL.substack.com`  
**Replace all 2 occurrences with** your actual Substack URL, e.g. `sherryxu.substack.com`

---

### 3. Your photo
**Search for:** `EDIT: Replace this placeholder with your photo`  
**What to do:**
- Add a file called `photo.jpg` to your GitHub repository (your headshot, cropped to portrait)
- Delete the entire `<div class="about-photo-placeholder">...</div>` block
- Replace it with: `<img src="photo.jpg" alt="Sherry Xu" style="width:100%;aspect-ratio:3/4;object-fit:cover;border-radius:12px;">`

---

### 4. Routledge book links
**Search for:** `EDIT: Replace with the direct book URL from Routledge`  
**Replace with** the actual URL from the Routledge website product page for your book.

Also search for `EDIT: Replace href with direct book URL` in the hero card and update that too.

---

### 5. Your LinkedIn URL
**Search for:** `YOUR-LINKEDIN-HANDLE`  
**Replace with** your actual LinkedIn URL, e.g. `https://www.linkedin.com/in/yishuang-sherry-xu`

---

### 6. Gumroad product links
**Search for:** `YOUR-GUMROAD-LINK`  
There are 4 occurrences — one per product. Replace each with the correct Gumroad URL once products are live:
- Token Ready → your Gumroad Token Ready URL
- AI Prompts for Property → your Gumroad prompt library URL
- Deal Tester → your Gumroad Deal Tester URL
- PropTech AI Radar → your Gumroad subscription URL

---

### 7. Research / publications
**Search for:** `Add your journal paper title here`  
There are 2 placeholder rows. Replace each one with a real publication using this pattern:

```html
<div class="research-row">
  <div class="research-year">2023</div>
  <div class="research-body">
    <div class="research-title">Your Paper Title Here</div>
    <div class="research-venue">Journal of Real Estate Research · Vol 45, pp. 123–145</div>
  </div>
</div>
```

Copy and paste this block as many times as you need for all your papers.

---

### 8. When an article goes live
When you publish a cornerstone article, find its "Coming soon" badge:

**Search for:** the article title, then look for `Coming soon` nearby  
**Replace:**
```html
<span class="article-status">Coming soon</span>
```
**With:**
```html
<a href="/articles/your-article-slug/" class="article-status live">Read article →</a>
```

Also create the article file at `articles/your-article-slug/index.html`.

---

### 9. Adding a new KDP book in the future
Find the correct group (AI & Technology, ESG & Sustainability, or Digital Assets).  
Copy one existing book card and paste it at the end of that group:

```html
<a href="https://www.amazon.co.uk/dp/YOUR-ASIN" target="_blank" class="book-card">
  <div class="book-card-thumb" style="background:#YOUR-COLOUR;aspect-ratio:2/3;display:flex;align-items:center;justify-content:center;padding:1rem;text-align:center;">
    <div class="book-card-thumb-text">Your Book Title</div>
  </div>
  <div class="book-card-body">
    <div class="book-card-title">Your Full Book Title Here</div>
    <div class="book-card-tag">For your target reader</div>
  </div>
</a>
```

Replace `YOUR-ASIN` with the Amazon ASIN (found on your KDP bookshelf).  
Replace `YOUR-COLOUR` with a hex colour code — pick from these:
- Dark navy: `#0a3d5e`
- Teal: `#0a6b5e`
- Deep green: `#1a4d2e`
- Dark purple: `#2a1a5c`
- Deep blue: `#134e7a`

---

## Tip: use Ctrl+F / Cmd+F

The fastest way to find anything in the file is to search for the exact text shown above. VS Code will highlight every match instantly.

If you ever want Claude to make a bigger change (redesign a section, add a new page, update the layout), just share the current `index.html` file and ask.
