# Testing Your Robot Forest Site

Due to shell configuration issues in my environment, I wasn't able to build the site automatically. However, all the theme files have been created successfully! Here's how to test and build your site:

## Quick Test

1. Open your terminal
2. Navigate to the project directory:
   ```bash
   cd /Users/kristophm/workspace/robotforest_hugo
   ```

3. Check Hugo version (to ensure Hugo is installed):
   ```bash
   hugo version
   ```

4. Run the development server:
   ```bash
   hugo server -D
   ```

5. Open your browser to http://localhost:1313

## What You Should See

When the site loads, you should see:

- **Navigation bar** with links to Home, Blog, About, Consulting, and Contact
- **Hero section** with the positioning statement configured in hugo.toml
- **Newsletter signup** section with email input
- **Latest blog posts** displayed in a grid (3 sample posts are included)
- **Social media icons** in the header and footer
- **Dark theme** with modern, clean aesthetics

## Building for Production

To build the static site:

```bash
hugo
```

The built site will be in the `public/` directory.

## Expected Issues & Fixes

### Missing Logo
- You'll see a text logo until you place your logo image at `static/images/logo.png`
- The theme is configured to show your logo when it's present

### Newsletter Form
- Update the form action URL in `hugo.toml` to connect to your newsletter service
- Currently set to a placeholder: `https://YOUR_NEWSLETTER_SERVICE_URL`

### Social Links
- Update the social media URLs in `hugo.toml` with your actual profiles
- Remove any social networks you don't use

## Theme Structure

All theme files are in: `themes/robotforest/`

- **Layouts**: HTML templates for pages
- **Static/CSS**: Dark theme styling
- **Static/JS**: Mobile navigation and interactions
- **Archetypes**: Template for new posts

## Troubleshooting

If Hugo reports any errors:

1. Check that Hugo is installed: `hugo version`
2. Ensure you're in the project directory
3. Check for syntax errors in `hugo.toml`
4. Make sure the theme directory exists: `themes/robotforest/`

All theme files have been created according to Hugo best practices, so it should work without issues!

