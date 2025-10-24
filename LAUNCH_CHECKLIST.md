# Robot Forest - Launch Checklist

Use this checklist to prepare your site for launch.

## 🎯 Pre-Launch Tasks

### 1. Branding & Identity
- [ ] Add logo to `static/images/logo.png`
- [ ] Verify site title in `hugo.toml`
- [ ] Update baseURL in `hugo.toml` to your domain
- [ ] Check hero title and subtitle match your messaging
- [ ] Verify site description in `hugo.toml`

### 2. Configuration
- [ ] Update all social media URLs in `hugo.toml`
- [ ] Remove social networks you don't use
- [ ] Configure newsletter service action URL
- [ ] Test newsletter signup form
- [ ] Verify email addresses in contact page
- [ ] Check all menu items link correctly

### 3. Content
- [ ] Customize About page (`content/about/_index.md`)
- [ ] Customize Consulting page (`content/consulting/_index.md`)
- [ ] Customize Contact page (`content/contact/_index.md`)
- [ ] Remove or edit sample blog posts
- [ ] Write at least 1-3 real blog posts
- [ ] Set `draft: false` on published posts
- [ ] Add featured images to posts
- [ ] Review all tags for consistency
- [ ] Check all internal links work

### 4. SEO & Meta
- [ ] Verify page titles are descriptive
- [ ] Add meta descriptions to all pages
- [ ] Check that featured images are set
- [ ] Review heading hierarchy (H1 → H2 → H3)
- [ ] Verify baseURL matches your domain
- [ ] Test RSS feed generation
- [ ] Check sitemap.xml generates

### 5. Media & Assets
- [ ] Optimize all images (compress, resize)
- [ ] Add alt text to all images
- [ ] Verify logo displays correctly
- [ ] Check featured images on all posts
- [ ] Test image loading on slow connections
- [ ] Ensure all images are web-optimized (< 200KB each)

### 6. Testing

#### Local Testing
- [ ] Run `hugo server -D` and review entire site
- [ ] Test all navigation links
- [ ] Test newsletter form submission
- [ ] Test social media links
- [ ] Read through all content for typos
- [ ] Check mobile responsiveness
- [ ] Test on different browsers

#### Responsive Testing
- [ ] Test on mobile phone (375px)
- [ ] Test on tablet (768px)
- [ ] Test on laptop (1024px)
- [ ] Test on desktop (1440px+)
- [ ] Verify mobile menu works
- [ ] Check newsletter form on mobile
- [ ] Verify images scale properly

#### Browser Testing
- [ ] Chrome/Chromium
- [ ] Firefox
- [ ] Safari
- [ ] Edge
- [ ] Mobile Safari (iOS)
- [ ] Chrome Mobile (Android)

### 7. Performance
- [ ] Run Lighthouse audit
- [ ] Check page load times
- [ ] Verify images are optimized
- [ ] Test on slow 3G connection
- [ ] Confirm CSS/JS are minified (Hugo does this)
- [ ] Check there are no console errors

### 8. Accessibility
- [ ] All images have alt text
- [ ] Links have descriptive text
- [ ] Color contrast is sufficient
- [ ] Test keyboard navigation
- [ ] Test with screen reader (if possible)
- [ ] Verify ARIA labels on icon buttons

### 9. Legal & Privacy
- [ ] Add privacy policy (if collecting emails)
- [ ] Add terms of service (if needed)
- [ ] Verify GDPR compliance (if EU visitors)
- [ ] Check newsletter service compliance
- [ ] Add cookie notice (if using cookies)

## 🚀 Deployment

### Hosting Setup
- [ ] Choose hosting platform (Netlify, Vercel, etc.)
- [ ] Create account on hosting platform
- [ ] Connect Git repository
- [ ] Configure build settings:
  - Build command: `hugo`
  - Publish directory: `public`
  - Hugo version: Set in environment variables

### Domain Configuration
- [ ] Purchase domain (if needed)
- [ ] Configure DNS settings
- [ ] Set up HTTPS/SSL certificate
- [ ] Verify domain points to hosting
- [ ] Update baseURL in `hugo.toml` to final domain

### First Deploy
- [ ] Push code to Git repository
- [ ] Trigger first build
- [ ] Verify build succeeds
- [ ] Check deployed site URL
- [ ] Test all functionality on live site
- [ ] Verify forms work on production
- [ ] Check SSL certificate is active

## 📊 Post-Launch

### Analytics (Optional)
- [ ] Set up Google Analytics or Plausible
- [ ] Add tracking code to theme
- [ ] Verify analytics is collecting data
- [ ] Set up conversion tracking for newsletter

### Monitoring
- [ ] Set up uptime monitoring
- [ ] Configure error notifications
- [ ] Monitor site performance
- [ ] Check for broken links regularly

### Newsletter
- [ ] Verify newsletter integration works
- [ ] Test signup flow end-to-end
- [ ] Check confirmation emails arrive
- [ ] Verify subscriber list updates
- [ ] Set up welcome email

### SEO
- [ ] Submit sitemap to Google Search Console
- [ ] Submit to Bing Webmaster Tools
- [ ] Verify robots.txt is correct
- [ ] Check indexing status
- [ ] Set up structured data (if desired)

### Social Media
- [ ] Share launch on social media
- [ ] Update social media bios with website link
- [ ] Create social media images (OG images)
- [ ] Test social media preview cards
- [ ] Pin introductory post

### Content Plan
- [ ] Create editorial calendar
- [ ] Plan first 5-10 blog posts
- [ ] Schedule regular posting
- [ ] Plan newsletter schedule
- [ ] Identify content topics/themes

## ✅ Launch Day

### Final Checks
- [ ] Clear browser cache and test
- [ ] Send test email through newsletter
- [ ] Test from different devices
- [ ] Check all links one more time
- [ ] Verify contact form/email works
- [ ] Take screenshots for records
- [ ] Backup site files

### Go Live
- [ ] Update DNS to point to hosting
- [ ] Wait for DNS propagation (up to 48 hours)
- [ ] Test on live domain
- [ ] Verify HTTPS works
- [ ] Check all functionality
- [ ] Announce launch!

## 🎉 Post-Launch Checklist

### Week 1
- [ ] Monitor analytics daily
- [ ] Check for any error reports
- [ ] Respond to any contact form submissions
- [ ] Share launch on social media
- [ ] Publish first post-launch blog post
- [ ] Engage with early visitors

### Month 1
- [ ] Review analytics insights
- [ ] Publish 2-4 blog posts
- [ ] Grow newsletter subscribers
- [ ] Optimize based on user behavior
- [ ] Fix any issues found
- [ ] Gather feedback

### Ongoing
- [ ] Regular blog posts (weekly/bi-weekly)
- [ ] Newsletter campaigns
- [ ] SEO optimization
- [ ] Content updates
- [ ] Performance monitoring
- [ ] Security updates

## 🔧 Troubleshooting

### Build Fails
1. Check Hugo version matches requirements
2. Verify `hugo.toml` syntax
3. Check for draft posts in production
4. Review build logs for errors

### Forms Don't Work
1. Verify newsletter action URL
2. Check form method is POST
3. Test with different email addresses
4. Review service provider documentation

### Images Not Loading
1. Check file paths (must start with `/`)
2. Verify files exist in `static/images/`
3. Check file permissions
4. Clear CDN cache if using one

### Styling Issues
1. Hard refresh browser (Ctrl+F5)
2. Clear browser cache
3. Check CSS file is loading
4. Verify no console errors
5. Test in incognito mode

## 📞 Support Resources

- **Hugo Docs**: https://gohugo.io/documentation/
- **Hugo Forum**: https://discourse.gohugo.io/
- **Netlify Docs**: https://docs.netlify.com/
- **Vercel Docs**: https://vercel.com/docs
- **Theme Docs**: `themes/robotforest/README.md`

## 💡 Pro Tips

1. **Test early, test often** - Don't wait until launch day
2. **Mobile first** - Most visitors will be on mobile
3. **Real content** - Test with real, not Lorem Ipsum
4. **Slow connections** - Test on throttled connections
5. **Ask for feedback** - Get others to review before launch
6. **Backup everything** - Keep backups of content and config
7. **Document changes** - Keep notes on customizations
8. **Version control** - Use Git for all changes

---

## Quick Launch Path (Minimum Viable)

If you want to launch quickly with minimum setup:

1. ✅ Add logo
2. ✅ Update About page
3. ✅ Write 1-2 blog posts
4. ✅ Configure social links
5. ✅ Set up basic newsletter
6. ✅ Test on mobile
7. ✅ Deploy!

You can enhance and optimize after launch. Don't let perfectionism delay you!

---

**Ready to launch?** Check off each item as you complete it. Good luck! 🚀

