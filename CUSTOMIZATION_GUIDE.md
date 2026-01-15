# Portfolio Customization Guide

## 🎨 Your Professional Portfolio is Ready!

This modern, responsive portfolio website has been customized with your information and is ready to deploy.

## 📋 What's Included

### ✅ Sections Implemented:
- **Hero Section** - Eye-catching introduction with your name, role, and call-to-action buttons
- **About Section** - Professional summary with key statistics (CGPAs, projects, certifications)
- **Education Timeline** - Visual timeline of your academic journey
- **Skills Section** - Categorized display of technical and soft skills
- **Projects Section** - Showcase of your 3 major projects with tech stacks
- **Certifications** - Display of your 4 professional certifications
- **Publications** - Research paper on Phishing URL Detection
- **Contact Section** - Contact form and social links

### 🎯 Features:
- ✨ Modern, clean, and professional design
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎭 Smooth animations and transitions
- 🎨 Professional color scheme (purple/indigo gradient)
- 🚀 Fast loading and optimized
- 💼 Recruiter-friendly and ATS-compatible content

## 🔧 Quick Customization Steps

### 1. Update Contact Information
Edit `public/index.html` and replace placeholder links:

```html
<!-- Line 35-37: Social Links -->
<a href="mailto:YOUR_EMAIL@example.com">
<a href="https://linkedin.com/in/YOUR_LINKEDIN">
<a href="https://github.com/YOUR_GITHUB">

<!-- Line 382-397: Contact Section -->
Update email, LinkedIn, and GitHub URLs
```

### 2. Add Your Profile Photo
- Place your photo in `public/` folder as `profile.jpg`
- Recommended size: 400x400px (square)
- Format: JPG or PNG
- The image will automatically display in the hero section

### 3. Add Resume Download Link
Edit line 32 in `public/index.html`:
```html
<a href="path/to/your-resume.pdf" class="btn outline" download>
```

### 4. Update Project Links
Replace `#` with your actual GitHub repository URLs (lines 267, 285, 303):
```html
<a href="https://github.com/yourusername/project-repo" class="project-link">
```

### 5. Customize Colors (Optional)
Edit `public/style.css` to change the color scheme:
```css
/* Primary Color: Search and replace #6366f1 with your color */
/* Accent Color: Search and replace #fbbf24 with your color */
/* Gradient: Line 127 - background: linear-gradient(...) */
```

## 🚀 Deployment Options

### Option 1: Railway (Recommended)
```bash
# Already configured with Dockerfile
# Just push to GitHub and connect to Railway
railway up
```

### Option 2: Netlify/Vercel
```bash
# Deploy the public folder directly
# Build command: (none needed)
# Publish directory: public
```

### Option 3: GitHub Pages
```bash
# Push to GitHub
# Settings > Pages > Deploy from branch
# Select main branch and /public folder
```

### Option 4: Traditional Hosting
- Upload contents of `public/` folder to your web host
- Ensure index.html is in the root directory

## 📝 Content Updates

### Adding More Projects
Copy this template in `public/index.html` (around line 260):

```html
<div class="project-card">
    <div class="project-image">
        <i class="fas fa-ICON-NAME"></i>
    </div>
    <div class="project-content">
        <h3>Project Title</h3>
        <p>Project description...</p>
        <div class="project-tech">
            <span>Tech1</span>
            <span>Tech2</span>
        </div>
        <div class="project-links">
            <a href="#" class="project-link"><i class="fab fa-github"></i></a>
        </div>
    </div>
</div>
```

### Adding More Skills
Add skill tags in the appropriate category (around line 180):
```html
<span class="skill-tag">New Skill</span>
```

### Adding More Certifications
Copy this template (around line 320):
```html
<div class="cert-card">
    <div class="cert-icon">
        <i class="fab fa-ICON"></i>
    </div>
    <h3>Certification Name</h3>
    <p>Issuing Organization</p>
</div>
```

## 🎨 Icon Reference

Using Font Awesome 6.0 icons. Common icons:
- `fa-java` - Java
- `fa-python` - Python
- `fa-js` - JavaScript
- `fa-aws` - AWS
- `fa-docker` - Docker
- `fa-github` - GitHub
- `fa-linkedin` - LinkedIn
- `fa-cloud` - Cloud
- `fa-database` - Database
- `fa-code` - Code

Browse more: https://fontawesome.com/icons

## 📱 Testing Checklist

Before deploying, test:
- [ ] All navigation links work
- [ ] Mobile menu opens/closes properly
- [ ] Contact form submits (configure backend)
- [ ] All social links are correct
- [ ] Profile image loads
- [ ] Resume download works
- [ ] Responsive on mobile, tablet, desktop
- [ ] All animations work smoothly

## 🔒 Contact Form Setup

The contact form needs a backend. Options:

### Option 1: Formspree (Easiest)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: EmailJS
Add EmailJS script and configure in `script.js`

### Option 3: Custom Backend
The current setup sends to `/api/contact` - implement in `index.js`

## 🎯 SEO Optimization

Already included:
- ✅ Meta description
- ✅ Semantic HTML
- ✅ Alt tags for images
- ✅ Fast loading

To improve further:
1. Add `robots.txt`
2. Add `sitemap.xml`
3. Configure Open Graph tags
4. Add Google Analytics

## 📊 Performance Tips

- Optimize images (use WebP format)
- Enable caching on your server
- Use CDN for Font Awesome (already configured)
- Minify CSS/JS for production

## 🆘 Troubleshooting

**Profile image not showing?**
- Check file name is exactly `profile.jpg`
- Check file is in `public/` folder
- Clear browser cache

**Mobile menu not working?**
- Check `script.js` is loaded
- Check browser console for errors

**Animations not smooth?**
- Disable animations in CSS if needed
- Check browser compatibility

## 📞 Support

For issues or questions:
- Check browser console for errors
- Validate HTML: https://validator.w3.org/
- Test responsiveness: Chrome DevTools

## 🎉 You're All Set!

Your portfolio is professional, modern, and ready to impress recruiters. Good luck with your job search!

---

**Built with:** HTML5, CSS3, JavaScript, Font Awesome, Google Fonts
**Optimized for:** Software Developer & Cloud/DevOps roles
**ATS-Friendly:** ✅ Yes
