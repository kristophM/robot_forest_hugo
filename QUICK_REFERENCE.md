# Robot Forest - Quick Reference

Fast reference for common tasks and commands.

## 🚀 Common Commands

### Start Development Server
```bash
hugo server -D
```
- `-D` includes draft posts
- Visit http://localhost:1313
- Auto-reloads on file changes

### Build Production Site
```bash
hugo
```
- Outputs to `public/` directory
- Excludes draft posts
- Ready to deploy

### Create New Post
```bash
hugo new posts/my-post-title.md
```
- Creates file in `content/posts/`
- Uses template from `archetypes/default.md`
- Set `draft: false` to publish

### Create New Page
```bash
hugo new about/_index.md
```
- Creates static page
- Add to menu in `hugo.toml` if needed

## 📝 Front Matter Templates

### Blog Post
```yaml
---
title: "Your Post Title"
date: 2024-10-24T10:00:00-07:00
description: "SEO description for search engines"
tags: ["robotics", "iot", "automation"]
featured_image: "/images/post-image.jpg"
draft: false
---
```

### Static Page
```yaml
---
title: "Page Title"
description: "Page description"
---
```

## ⚙️ Configuration Quick Edits

### Update Hero Text
**File**: `hugo.toml`
```toml
[params.hero]
title = 'Your New Title'
subtitle = 'Your new subtitle'
```

### Update Newsletter
**File**: `hugo.toml`
```toml
[params.newsletter]
enabled = true
title = 'Newsletter Title'
description = 'Description text'
action = 'https://your-service.com/subscribe'
```

### Add/Remove Menu Items
**File**: `hugo.toml`
```toml
[[menu.main]]
name = 'New Page'
url = '/new-page/'
weight = 6
```

### Add/Remove Social Links
**File**: `hugo.toml`
```toml
[[params.social]]
name = 'GitHub'
icon = 'github'  # github, linkedin, twitter, email, rss, youtube
url = 'https://github.com/username'
```

## 🎨 Style Customization

### Change Colors
**File**: `themes/robotforest/static/css/style.css`
```css
:root {
    --color-accent: #60a5fa;        /* Change accent color */
    --color-accent-secondary: #8b5cf6;  /* Change secondary accent */
    --color-bg: #0a0e1a;            /* Change background */
}
```

### Change Fonts
**File**: `themes/robotforest/layouts/partials/head.html`

Update Google Fonts import and then in CSS:
```css
:root {
    --font-sans: 'Your Font', sans-serif;
    --font-mono: 'Your Mono Font', monospace;
}
```

## 📁 File Locations

### Content
- Blog posts: `content/posts/`
- Static pages: `content/[page-name]/`

### Images
- Logo: `static/images/logo.png`
- Post images: `static/images/`

### Theme Files
- HTML templates: `themes/robotforest/layouts/`
- CSS: `themes/robotforest/static/css/style.css`
- JS: `themes/robotforest/static/js/main.js`

### Configuration
- Main config: `hugo.toml`
- Theme config: `themes/robotforest/theme.toml`

## 🖼️ Adding Images

### Logo
1. Place at: `static/images/logo.png`
2. Already configured in `hugo.toml`

### Post Featured Image
1. Place in: `static/images/`
2. Add to front matter:
```yaml
featured_image: "/images/your-image.jpg"
```

### Inline Image in Post
```markdown
![Alt text](/images/inline-image.jpg)
```

## 🏷️ Working with Tags

### In Post Front Matter
```yaml
tags: ["robotics", "iot", "security"]
```

### Tag URLs
- Automatic: `/tags/robotics/`
- Lists all posts with that tag

## 📱 Testing Responsive Design

### Browser DevTools
1. Open developer tools (F12)
2. Toggle device toolbar (Ctrl+Shift+M)
3. Test mobile (375px), tablet (768px), desktop (1200px+)

### Mobile Menu
- Appears at 768px and below
- Hamburger icon in top right
- Full-height slide-in menu

## 🔍 SEO Checklist

For each post/page:
- ✅ Add descriptive title
- ✅ Add meta description
- ✅ Use relevant tags
- ✅ Add featured image
- ✅ Write clear, informative content
- ✅ Use proper heading hierarchy (H1 → H2 → H3)

## 📦 Deployment

### Netlify
1. Connect Git repository
2. Build command: `hugo`
3. Publish directory: `public`
4. Hugo version: Set in netlify.toml

### Vercel
1. Import Git repository
2. Framework preset: Hugo
3. Build command: `hugo`
4. Output directory: `public`

### GitHub Pages
1. Build site locally: `hugo`
2. Push `public/` to gh-pages branch
3. Or use GitHub Actions for auto-deploy

## 🐛 Troubleshooting

### Site not loading
- Check Hugo is installed: `hugo version`
- Check you're in project root
- Try: `hugo server --disableFastRender`

### Newsletter form not working
- Update `action` URL in `hugo.toml`
- Check newsletter service documentation
- Verify form accepts POST requests

### Images not showing
- Check file path (use `/images/file.jpg`)
- Verify file exists in `static/images/`
- Check file extension matches

### Menu links not working
- Verify URLs start with `/`
- Check content file exists
- Ensure file is not draft (if in production)

### CSS not updating
- Hard refresh: Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)
- Clear browser cache
- Restart `hugo server`

## 📚 Resources

### Hugo Documentation
- Getting Started: https://gohugo.io/getting-started/
- Content Management: https://gohugo.io/content-management/
- Templates: https://gohugo.io/templates/

### Theme Documentation
- `themes/robotforest/README.md` - Theme overview
- `DESIGN_SYSTEM.md` - Visual design details
- `VISUAL_PREVIEW.md` - What it looks like

### Markdown Reference
- Headings: `# H1`, `## H2`, etc.
- Links: `[text](url)`
- Images: `![alt](url)`
- Code: `` `inline` `` or ` ```language ` for blocks
- Lists: `- item` or `1. item`
- Bold: `**text**`
- Italic: `*text*`

## 💡 Pro Tips

1. **Write in drafts**: Use `draft: true` until ready to publish
2. **Descriptive filenames**: `edge-computing-robotics.md` not `post1.md`
3. **Consistent tagging**: Reuse tags across posts
4. **Optimize images**: Compress before uploading
5. **Preview before publishing**: Always test with `hugo server -D`
6. **Back up content**: Use Git to version control
7. **Regular posts**: Maintain consistent publishing schedule
8. **Update dates**: Keep dates current when editing old posts

## 🎯 Quick Wins

### Add Your Logo
```bash
# Place logo file
cp ~/path/to/your/logo.png static/images/logo.png
```

### First Blog Post
```bash
hugo new posts/my-first-real-post.md
# Edit file, set draft: false
hugo server -D
```

### Change Colors
Edit these two lines in `themes/robotforest/static/css/style.css`:
```css
--color-accent: #YOUR_COLOR;
--color-accent-secondary: #YOUR_COLOR;
```

### Update Social Links
Find `[[params.social]]` sections in `hugo.toml` and update URLs.

---

Bookmark this file for quick reference! 🔖

