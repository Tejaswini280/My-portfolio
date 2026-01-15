# 📸 How to Add Your Photos to the Portfolio

## Step 1: Save Your Photos

You have two images to add:

### 1. Profile Photo (Professional Photo)
- **File name:** `profile.jpg`
- **Location:** Save to `railway-deployment/public/profile.jpg`
- **Recommended size:** 400x400 pixels (square)
- **Format:** JPG or PNG
- **This is:** Your professional headshot photo

### 2. Hero Card Design (Optional)
- **File name:** `hero-card.jpg` or `hero-card.png`
- **Location:** Save to `railway-deployment/public/hero-card.jpg`
- **This is:** The green card design with your name and "Available for opportunities"

## Step 2: How to Save the Images

### Option A: Manual Save (Easiest)
1. Right-click on each image
2. Select "Save Image As..."
3. Navigate to `railway-deployment/public/` folder
4. Save as:
   - Professional photo → `profile.jpg`
   - Green card design → `hero-card.jpg`

### Option B: Using File Explorer
1. Open the folder: `railway-deployment/public/`
2. Copy your images into this folder
3. Rename them to:
   - `profile.jpg` (your professional photo)
   - `hero-card.jpg` (the green card design)

## Step 3: Verify the Images

After saving, your `public` folder should contain:
```
railway-deployment/public/
├── index.html
├── style.css
├── script.js
├── profile.jpg          ← Your professional photo
└── hero-card.jpg        ← (Optional) Green card design
```

## Step 4: Test Locally

1. Refresh your browser at `http://localhost:3000`
2. Your profile photo should appear in the hero section
3. If it doesn't show, check:
   - File name is exactly `profile.jpg` (lowercase)
   - File is in the `public` folder
   - Clear browser cache (Ctrl+F5)

## Step 5: Push to GitHub

After adding the images:

```bash
cd railway-deployment
git add public/profile.jpg
git add public/hero-card.jpg  # if you added this
git commit -m "Add profile photos"
git push origin dev
```

## 🎨 Image Optimization Tips

### For Best Results:
1. **Profile Photo:**
   - Square format (1:1 ratio)
   - Minimum 400x400 pixels
   - Maximum 1000x1000 pixels
   - Professional background
   - Good lighting
   - Clear face visibility

2. **File Size:**
   - Keep under 500KB for fast loading
   - Use online tools to compress:
     - https://tinypng.com/
     - https://squoosh.app/

3. **Format:**
   - JPG for photos (smaller file size)
   - PNG for graphics with transparency

## 🔧 Troubleshooting

### Image Not Showing?

**Check 1: File Name**
- Must be exactly `profile.jpg` (lowercase)
- No spaces or special characters

**Check 2: File Location**
- Must be in `railway-deployment/public/` folder
- Not in a subfolder

**Check 3: Browser Cache**
- Press Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)
- Or open in incognito/private mode

**Check 4: File Format**
- If using PNG, update HTML:
  ```html
  <img src="profile.png" alt="Tejaswini Kawade">
  ```

### Image Too Large or Small?

The CSS is already set to:
- Width: 200px
- Height: 200px
- Border-radius: 50% (makes it circular)

If you want to change the size, edit `style.css`:
```css
.profile-img img {
    width: 250px;    /* Change this */
    height: 250px;   /* Change this */
}
```

## 🎯 Current Setup

Your portfolio is already configured to display:
- Profile photo in the hero section (right side)
- Circular frame with animated border
- Floating animation effect
- Glowing border on hover

The image will automatically:
- ✅ Be cropped to circular shape
- ✅ Have animated gradient border
- ✅ Float up and down smoothly
- ✅ Glow on hover
- ✅ Be responsive on mobile

## 📱 Mobile Display

On mobile devices:
- Image size reduces to 150x150px
- Still maintains circular shape
- Animation continues smoothly

## ✨ Alternative: Use the Green Card Design

If you want to use the green card design instead of just the photo:

1. Save the green card as `hero-card.jpg`
2. Update the HTML (line ~70):
   ```html
   <img src="hero-card.jpg" alt="Tejaswini Kawade">
   ```
3. Update CSS to make it rectangular instead of circular:
   ```css
   .profile-img img {
       border-radius: 15px;  /* Instead of 50% */
   }
   ```

## 🚀 Quick Start

**Fastest way to add your photo:**

1. Save your professional photo as `profile.jpg`
2. Copy it to `railway-deployment/public/`
3. Refresh browser
4. Done! ✅

---

**Need help?** Check the browser console (F12) for any image loading errors.

**Ready to deploy?** Once the image looks good locally, push to GitHub and it will automatically deploy!
