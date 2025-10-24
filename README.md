# Robot Forest Hugo Site

Welcome to your Robot Forest website! This is a complete Hugo site with a custom-built theme designed for robotics and IoT consulting and blogging.

## 🚀 Quick Start

```bash
# Start the development server
hugo server -D

# Visit http://localhost:1313 in your browser

# When ready, build for production
hugo
```

## 📚 Documentation

This project includes comprehensive documentation:

### Getting Started
- **[SETUP_GUIDE.md](SETUP_GUIDE.md)** - Complete setup instructions and next steps
- **[QUICK_REFERENCE.md](QUICK_REFERENCE.md)** - Fast reference for common tasks
- **[TESTING.md](TESTING.md)** - How to test and build the site

### Understanding the Design
- **[THEME_SUMMARY.md](THEME_SUMMARY.md)** - Complete overview of what was built
- **[VISUAL_PREVIEW.md](VISUAL_PREVIEW.md)** - Detailed description of the visual design
- **[themes/robotforest/DESIGN_SYSTEM.md](themes/robotforest/DESIGN_SYSTEM.md)** - Design system and style guide
- **[themes/robotforest/README.md](themes/robotforest/README.md)** - Theme documentation

### Start Here
👉 **New to this site?** Start with [SETUP_GUIDE.md](SETUP_GUIDE.md)  
👉 **Want to customize?** Check [QUICK_REFERENCE.md](QUICK_REFERENCE.md)  
👉 **Visual overview?** Read [VISUAL_PREVIEW.md](VISUAL_PREVIEW.md)

## ✨ Features

- ✅ Modern dark theme optimized for robotics/IoT
- ✅ Responsive design (mobile, tablet, desktop)
- ✅ Blog with featured posts on homepage
- ✅ Static pages (About, Consulting, Contact)
- ✅ Newsletter subscription integration
- ✅ Social media links
- ✅ Tag system for posts
- ✅ SEO optimized
- ✅ Fast and lightweight

## 🏗️ Project Structure

```
robotforest_hugo/
├── README.md                    # This file
├── SETUP_GUIDE.md              # Setup instructions
├── QUICK_REFERENCE.md          # Quick reference
├── THEME_SUMMARY.md            # What was built
├── VISUAL_PREVIEW.md           # Visual design description
├── TESTING.md                  # Testing guide
├── hugo.toml                   # Site configuration
├── content/                    # Your content
│   ├── posts/                 # Blog posts
│   ├── about/                 # About page
│   ├── consulting/            # Consulting page
│   └── contact/               # Contact page
├── static/
│   └── images/                # Images and logo
└── themes/robotforest/        # The custom theme
    ├── README.md              # Theme docs
    ├── DESIGN_SYSTEM.md       # Design system
    ├── layouts/               # HTML templates
    └── static/                # CSS and JS
```

## 🎨 Theme

The **Robot Forest** theme was custom-built for this site with:
- Professional dark theme aesthetic
- Modern, clean design
- Robotics/IoT focused
- Fully responsive
- Newsletter integration built-in
- Social media integration
- Follows Hugo best practices

## 📝 Content

### Sample Content Included
- 3 blog posts demonstrating the format
- About page with mission and services
- Consulting page with service offerings
- Contact page with contact information

### Creating New Content

**New blog post:**
```bash
hugo new posts/my-post-title.md
```

**New static page:**
```bash
hugo new page-name/_index.md
```

## ⚙️ Configuration

Main configuration is in `hugo.toml`. Key settings:

- **Site info**: Title, description, base URL
- **Hero section**: Homepage positioning statement
- **Newsletter**: Subscription form configuration
- **Social links**: GitHub, LinkedIn, Twitter, etc.
- **Navigation menu**: Pages in the nav bar

See [QUICK_REFERENCE.md](QUICK_REFERENCE.md) for specific configuration examples.

## 🎯 Next Steps

1. ✅ **Add your logo** - Place at `static/images/logo.png`
2. ✅ **Configure newsletter** - Update action URL in `hugo.toml`
3. ✅ **Update social links** - Edit social URLs in `hugo.toml`
4. ✅ **Customize pages** - Edit About, Consulting, Contact pages
5. ✅ **Write content** - Create your first blog post
6. ✅ **Test locally** - Run `hugo server -D`
7. ✅ **Deploy** - Build and upload to your hosting

## 🌐 Deployment

The site can be deployed to:
- **Netlify** - Automatic deployment from Git
- **Vercel** - Auto-deploy with Hugo preset
- **GitHub Pages** - Static site hosting
- **Cloudflare Pages** - Fast global CDN
- **Any static host** - Upload the `public/` folder

See [SETUP_GUIDE.md](SETUP_GUIDE.md) for deployment details.

## 🛠️ Customization

### Change Colors
Edit CSS variables in `themes/robotforest/static/css/style.css`

### Modify Layouts
Edit templates in `themes/robotforest/layouts/`

### Update Styles
Edit `themes/robotforest/static/css/style.css`

### Add Functionality
Edit `themes/robotforest/static/js/main.js`

## 📱 Responsive Design

The site is fully responsive and tested on:
- Mobile phones (375px+)
- Tablets (768px+)
- Desktops (1024px+)
- Large screens (1440px+)

## 🔍 SEO

The theme includes:
- Semantic HTML structure
- Meta descriptions
- Open Graph tags
- RSS feed
- Sitemap generation
- Fast load times

## 🐛 Support

### Documentation
- Check the documentation files listed above
- Hugo docs: https://gohugo.io/documentation/
- Theme README: `themes/robotforest/README.md`

### Common Issues
- **Images not showing**: Check file path starts with `/images/`
- **Menu not working**: Verify URLs in `hugo.toml`
- **CSS not updating**: Hard refresh browser (Ctrl+F5)
- **Build errors**: Check `hugo.toml` syntax

## 📦 What's Included

### Theme Components
- ✅ Base template structure
- ✅ Homepage with blog post grid
- ✅ Single post layout
- ✅ List/archive layout
- ✅ Navigation with mobile menu
- ✅ Footer with multiple columns
- ✅ Newsletter signup section
- ✅ Social media icons
- ✅ Responsive CSS
- ✅ Interactive JavaScript
- ✅ Dark theme styling

### Sample Content
- ✅ 3 blog posts about robotics/IoT
- ✅ About page
- ✅ Consulting services page
- ✅ Contact page

### Documentation
- ✅ Setup guide
- ✅ Quick reference
- ✅ Theme summary
- ✅ Visual preview
- ✅ Design system
- ✅ Testing guide

## 🎓 Learning Resources

### Hugo
- [Hugo Quick Start](https://gohugo.io/getting-started/quick-start/)
- [Content Management](https://gohugo.io/content-management/)
- [Hugo Themes](https://themes.gohugo.io/)

### Markdown
- [Markdown Guide](https://www.markdownguide.org/)
- [Hugo Markdown](https://gohugo.io/content-management/formats/)

### Deployment
- [Netlify Hugo Guide](https://docs.netlify.com/configure-builds/common-configurations/hugo/)
- [Vercel Hugo Guide](https://vercel.com/guides/deploying-hugo-with-vercel)

## 📄 License

The theme is MIT licensed. Use it however you like!

## 🙏 Credits

Theme designed and built for Robot Forest.  
Fonts: Inter (Google Fonts), JetBrains Mono (Google Fonts)  
Icons: Custom SVG icons  
Framework: Hugo static site generator

---

## 🚦 Status

✅ **Theme Complete** - All features implemented  
✅ **Sample Content** - Ready to customize  
✅ **Documentation** - Comprehensive guides included  
✅ **Ready to Deploy** - Test and launch!

---

**Ready to get started?** Open [SETUP_GUIDE.md](SETUP_GUIDE.md) and follow the steps!

Built with ❤️ for robotics and IoT professionals. 🤖🌲

