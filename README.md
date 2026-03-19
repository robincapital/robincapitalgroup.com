# Robin Capital Group — robincapitalgroup.com

Static site hosted via GitHub Pages.

**Live site:** https://robincapitalgroup.com  
**Substack:** https://robincapitalgroup.substack.com

## Structure

```
index.html        ← entire site (single file)
README.md         ← this file
CNAME             ← custom domain config for GitHub Pages
```

## To update content

Edit `index.html` directly — all content, styles, and scripts are in one file.  
Commit and push → GitHub Pages auto-deploys within ~60 seconds.

## Performance notes

- No WordPress, no plugins, no page builder
- No external JS libraries (all CSS animations are native)
- Images served directly from robincapitalgroup.com CDN
- Google Fonts is the only external dependency (can be self-hosted if needed)
