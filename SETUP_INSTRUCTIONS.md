# Portfolio Setup Instructions

## Adding Your Profile Picture

To add your profile picture to the portfolio:

1. **Save your profile picture** as `profile.jpg` in the `public` folder
   - Path: `railway-deployment/public/profile.jpg`
   - Recommended size: 400x400 pixels or larger (square format)
   - Supported formats: JPG, JPEG, PNG

2. **Alternative method** - If you want to use a different filename:
   - Save your image in the `public` folder with any name (e.g., `my-photo.png`)
   - Open `public/index.html`
   - Find the line: `<img src="profile.jpg" alt="Tejaswini Kawade" id="profileImage">`
   - Change `profile.jpg` to your filename (e.g., `my-photo.png`)

## Running the Portfolio Locally

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start the development server:**
   ```bash
   npm start
   ```

3. **Open in browser:**
   - Navigate to `http://localhost:3000`

## Deploying to Railway

1. **Push your code to GitHub** (including your profile picture)

2. **Connect to Railway:**
   - Go to [railway.app](https://railway.app)
   - Create a new project
   - Connect your GitHub repository
   - Railway will automatically detect and deploy your Node.js application

3. **Environment Variables:**
   - No additional environment variables needed for basic deployment

## Customization Tips

### Updating Personal Information

1. **Contact Details** - Edit in `public/index.html`:
   - Email: Search for `tejaswinikawade@gmail.com`
   - LinkedIn: Search for `linkedin.com/in/tejaswini-kawade`
   - GitHub: Search for `github.com/Tejaswini280`

2. **Projects** - Add/edit projects in the "Projects Section" of `public/index.html`

3. **Skills** - Update skills in the "Skills Section" of `public/index.html`

4. **Education** - Modify education timeline in the "Education Section"

### Changing Colors

Edit `public/style.css` to change the color scheme:
- Primary color: `#6366f1` (indigo)
- Accent color: `#fbbf24` (yellow/gold)
- Search and replace these hex codes with your preferred colors

### Adding More Animations

The portfolio includes several animations:
- Typing effect on hero subtitle
- Floating profile image
- Hover effects on cards and buttons
- Scroll-triggered animations
- Parallax effects
- Skill tag color changes

You can enable/disable animations in `public/script.js`

## Features Included

✅ Responsive design (mobile, tablet, desktop)
✅ Smooth scrolling navigation
✅ Animated hero section with typing effect
✅ Interactive project cards with tilt effect
✅ Skill tags with hover animations
✅ Timeline for education
✅ Contact form with API integration
✅ Social media links
✅ Certifications section
✅ Publications section
✅ Scroll progress indicator
✅ Active navigation highlighting
✅ Professional color scheme
✅ Modern UI/UX design

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Troubleshooting

**Profile picture not showing:**
- Check that the image file is in the `public` folder
- Verify the filename matches exactly (case-sensitive)
- Clear browser cache and refresh
- Check browser console for errors

**Animations not working:**
- Ensure JavaScript is enabled in your browser
- Check browser console for errors
- Try a different browser

**Contact form not working:**
- The form currently logs to console
- To enable email functionality, integrate with a service like:
  - EmailJS
  - SendGrid
  - Nodemailer with SMTP

## Support

For questions or issues, contact:
- Email: tejaswinikawade@gmail.com
- GitHub: github.com/Tejaswini280

---

**Last Updated:** January 2026
