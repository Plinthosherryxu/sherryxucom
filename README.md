# sherryxu.com — Personal Website

Personal website for Yishuang (Sherry) Xu — researcher, author, and founder working at the intersection of AI, ESG, and real estate.

## Structure

```
/
├── index.html        # Main single-page site
├── README.md         # This file
├── _config.yml       # GitHub Pages configuration
└── articles/         # Add individual article pages here as you write them
    └── ...
```

## Sections

- **Hero** — positioning and credentials
- **About** — bio and advisory enquiries
- **Book** — PropTech Innovations in Real Estate Investment and Finance (Routledge, 2026)
- **Books** — KDP titles by theme (AI & Finance · ESG · Digital Assets)
- **Tools** — Gumroad digital products
- **Articles** — 10 GEO cornerstone articles (add as written)
- **Newsletter** — Substack (AI and ESG)
- **Research** — academic publications

## Before Publishing — Update These

Open `index.html` and replace the following placeholders:

| Placeholder | Replace with |
|---|---|
| `your@email.com` | Your actual email address |
| `https://substack.com` | Your actual Substack URL |
| `https://www.routledge.com` | Direct Routledge book buy link |
| `https://www.amazon.co.uk` | Direct Amazon UK book link |
| `https://www.linkedin.com/in/yishuang-sherry-xu` | Your LinkedIn URL |
| `href="#"` on book cards | Amazon/KDP links for each title |
| `href="#"` on tool cards | Gumroad product links |
| Photo placeholder | `<img src="photo.jpg" alt="Sherry Xu">` |
| Research rows | Your actual publications |

## Hosting on GitHub Pages

1. Push this repository to `yourusername.github.io`
2. Go to **Settings → Pages → Source: main branch**
3. Site is live at `https://yourusername.github.io`

## Connecting a Custom Domain (sherryxu.com)

1. Buy domain on Namecheap
2. In Namecheap DNS, add a CNAME record: `www` → `yourusername.github.io`
3. Add A records pointing to GitHub Pages IPs:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
4. In GitHub: **Settings → Pages → Custom domain** → enter `sherryxu.com`
5. Check **Enforce HTTPS** once the certificate is issued (~10 minutes)

## Adding Article Pages

When you write a cornerstone article, create a folder and HTML file:

```
articles/
└── how-ai-is-used-in-real-estate/
    └── index.html
```

Each article page needs:
- `Article` schema markup
- `FAQPage` schema for the FAQ section
- Link back to homepage in the nav
- Cross-post summary on Quora and Medium with a link to the full article
- Submit URL to Bing via IndexNow (topify.ai)

## GEO Checklist (per article)

- [ ] Article answers a specific question in the first 200 words
- [ ] FAQPage schema added via topify.ai
- [ ] Submitted to Bing IndexNow
- [ ] Summary posted on Quora with link
- [ ] Summary posted on Medium with link
- [ ] Internal links to relevant books and tools

---

© 2026 Yishuang (Sherry) Xu
