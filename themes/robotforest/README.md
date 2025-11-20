# Robot Forest Hugo Theme

A modern, minimalistic dark theme for Hugo, designed for robotics and IoT blogs and websites.

## Features

- **Dark Mode Design**: Clean, professional dark theme optimized for readability
- **Responsive**: Mobile-first design that works on all devices
- **Blog & Static Pages**: Supports both blog posts and static content pages
- **Newsletter Integration**: Built-in newsletter subscription CTA
- **Social Links**: Configurable social media icons in header and footer
- **Fast & Lightweight**: Minimal JavaScript, optimized CSS
- **SEO Friendly**: Semantic HTML and proper meta tags

## Installation

1. Add the theme to your Hugo site:
```bash
cd your-hugo-site
git clone https://github.com/kristophM/robotforest-theme.git themes/robotforest
```

2. Update your `hugo.toml` to use the theme:
```toml
theme = 'robotforest'
```

## Configuration

### Site Parameters

Add the following to your `hugo.toml`:

```toml
[params]
description = 'Your site description'
logo = '/images/logo.png'  # Optional

# Hero section (shown on homepage)
[params.hero]
title = 'Your Hero Title'
subtitle = 'Your hero subtitle'

# Newsletter configuration
[params.newsletter]
enabled = true
title = 'Newsletter Title'
description = 'Newsletter description'
action = 'https://YOUR_NEWSLETTER_SERVICE_URL'

# Social links
[[params.social]]
name = 'GitHub'
icon = 'github'
url = 'https://github.com/kristophM'

[[params.social]]
name = 'LinkedIn'
icon = 'linkedin'
url = 'https://linkedin.com/in/kristophermatthews'
```

### Menu Configuration

Configure your main navigation menu:

```toml
[[menu.main]]
name = 'Home'
url = '/'
weight = 1

[[menu.main]]
name = 'Blog'
url = '/posts/'
weight = 2

[[menu.main]]
name = 'About'
url = '/about/'
weight = 3
```

## Content Organization

### Blog Posts

Create blog posts in the `content/posts/` directory:

```bash
hugo new posts/my-first-post.md
```

Front matter example:
```yaml
---
title: "My Post Title"
date: 2024-10-24T10:00:00-07:00
description: "Post description"
tags: ["robotics", "iot"]
featured_image: "/images/post-image.jpg"  # Optional
---
```

### Static Pages

Create static pages in `content/`:

```bash
hugo new about/_index.md
hugo new consulting/_index.md
hugo new contact/_index.md
```

## Supported Icons

The theme includes the following social icons:
- GitHub
- LinkedIn
- Twitter
- Email
- RSS
- YouTube

## Customization

### Colors

Edit `/themes/robotforest/static/css/style.css` to customize colors. CSS variables are defined at the top of the file:

```css
:root {
    --color-bg: #0a0e1a;
    --color-accent: #60a5fa;
    /* ... more variables */
}
```

### Fonts

The theme uses Inter for body text and JetBrains Mono for code. These are loaded from Google Fonts.

## Newsletter Integration

The theme supports newsletter services like Mailchimp, ConvertKit, or Substack. Configure the form action URL in your `hugo.toml`:

```toml
[params.newsletter]
enabled = true
action = 'YOUR_NEWSLETTER_FORM_ACTION_URL'
```

## License

MIT License

## Credits

Designed for Robot Forest by the Robot Forest team.

