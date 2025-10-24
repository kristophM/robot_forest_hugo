# Robot Forest Hugo Site - Setup Guide

Your Hugo site with the Robot Forest theme is now ready! Here's how to get started.

## Quick Start

1. **Add Your Logo**
   - Place your logo image at `static/images/logo.png`
   - The logo from your attachment should be placed here
   - Alternatively, update the logo path in `hugo.toml` if you use a different location/filename

2. **Configure Newsletter**
   - Sign up for a newsletter service (Mailchimp, ConvertKit, Buttondown, Substack, etc.)
   - Get your form action URL from your newsletter provider
   - Update the `params.newsletter.action` value in `hugo.toml`

3. **Update Social Links**
   - Edit the `[[params.social]]` sections in `hugo.toml`
   - Replace placeholder URLs with your actual social media profiles
   - Remove any social networks you don't use

4. **Customize Content**
   - Edit the hero section in `hugo.toml` to match your messaging
   - Update the About page at `content/about/_index.md`
   - Customize the Consulting page at `content/consulting/_index.md`
   - Update contact information in `content/contact/_index.md`

## Running the Site

Start the Hugo development server:

```bash
hugo server -D
```

Then visit http://localhost:1313 in your browser.

## Creating New Content

### New Blog Post

```bash
hugo new posts/my-new-post.md
```

Edit the created file and add your content. Don't forget to set `draft: false` when ready to publish.

### New Static Page

```bash
hugo new page-name/_index.md
```

Then add it to the menu in `hugo.toml` if you want it in the navigation.

## Building for Production

When you're ready to deploy:

```bash
hugo
```

This generates your site in the `public/` directory. Upload this to your web host.

## Theme Configuration Reference

### Hero Section

The hero section appears on the homepage below the navigation. Configure it in `hugo.toml`:

```toml
[params.hero]
title = 'Your Main Headline'
subtitle = 'Supporting text that explains what you do'
```

### Newsletter

```toml
[params.newsletter]
enabled = true  # Set to false to hide the newsletter section
title = 'Custom Title'
description = 'Custom description'
action = 'https://your-newsletter-service.com/subscribe'
```

### Post Front Matter

For blog posts, use this front matter structure:

```yaml
---
title: "Post Title"
date: 2024-10-24T10:00:00-07:00
description: "SEO description"
tags: ["tag1", "tag2"]
featured_image: "/images/post-featured.jpg"  # Optional
draft: false
---
```

## Customization

### Colors

To customize the color scheme, edit `themes/robotforest/static/css/style.css` and modify the CSS variables in the `:root` section.

### Fonts

The theme uses:
- **Inter** for body text
- **JetBrains Mono** for code

These are loaded from Google Fonts in `themes/robotforest/layouts/partials/head.html`.

## Tips

1. **Images**: Place images in `static/images/` and reference them as `/images/filename.jpg`
2. **Drafts**: Posts with `draft: true` won't appear in production builds
3. **Tags**: Create meaningful tags to help readers find related content
4. **Descriptions**: Always add descriptions for better SEO
5. **Featured Images**: Add featured images to make your blog posts more visually appealing

## Deployment

The site can be deployed to:
- **Netlify**: Connect your Git repository and it will auto-deploy
- **Vercel**: Similar auto-deployment from Git
- **GitHub Pages**: Use GitHub Actions to build and deploy
- **Any static host**: Just upload the `public/` directory

## Need Help?

- Hugo Documentation: https://gohugo.io/documentation/
- Theme README: `themes/robotforest/README.md`
- Theme Support: Review the theme files in `themes/robotforest/`

## Next Steps

1. ✅ Add your logo to `static/images/logo.png`
2. ✅ Configure your newsletter service
3. ✅ Update social media links
4. ✅ Customize the About, Consulting, and Contact pages
5. ✅ Write your first blog post
6. ✅ Test the site locally with `hugo server -D`
7. ✅ Deploy to your hosting platform

Happy blogging! 🤖🌲

