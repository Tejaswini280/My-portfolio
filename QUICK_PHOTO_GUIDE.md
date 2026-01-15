# 📸 Quick Photo Setup Guide

## 🎯 Simple 3-Step Process

### Step 1: Save Your Professional Photo
1. Right-click on your professional photo (the one in formal attire)
2. Save it as: **`profile.jpg`**
3. Place it in: **`railway-deployment/public/`** folder

### Step 2: Verify Location
Your file structure should look like this:
```
railway-deployment/
└── public/
    ├── index.html
    ├── style.css
    ├── script.js
    └── profile.jpg  ← Your photo goes here!
```

### Step 3: Test It
1. Open browser: `http://localhost:3000`
2. Your photo should appear in the hero section!
3. If you see a placeholder icon, the photo isn't in the right place

## 🖼️ About Your Images

You have 2 images:

**Image 1: Professional Photo** ✅ USE THIS
- Your formal photo in professional attire
- Save as: `profile.jpg`
- This will appear in the circular frame on your portfolio

**Image 2: Green Card Design** ℹ️ OPTIONAL
- The design mockup with "Available for opportunities"
- This is just a design reference
- You don't need to add this - the portfolio already has this design built-in!

## ⚡ Quick Commands

If you're comfortable with command line:

```bash
# Navigate to public folder
cd railway-deployment/public

# Check if profile.jpg exists
ls profile.jpg

# If it exists, you'll see: profile.jpg
# If not, add your photo to this folder
```

## 🎨 Image Requirements

- **Format:** JPG or PNG
- **Size:** 400x400 pixels (recommended)
- **File name:** Exactly `profile.jpg` (lowercase)
- **Max file size:** Under 500KB for fast loading

## 🔧 Troubleshooting

**Photo not showing?**

1. ✅ Check file name is exactly: `profile.jpg`
2. ✅ Check it's in the `public` folder
3. ✅ Refresh browser with Ctrl+F5
4. ✅ Check browser console (F12) for errors

**Want to use PNG instead?**

1. Save as `profile.png`
2. Update line 70 in `index.html`:
   ```html
   <img src="profile.png" alt="Tejaswini Kawade">
   ```

## 🚀 After Adding Photo

Once your photo is added and looks good:

```bash
cd railway-deployment
git add public/profile.jpg
git commit -m "Add profile photo"
git push origin dev
```

Your photo will automatically deploy with your portfolio!

## 💡 Pro Tip

The portfolio already has:
- ✅ Circular frame styling
- ✅ Animated gradient border
- ✅ Floating animation
- ✅ Hover glow effect
- ✅ Responsive sizing

Just add your photo and everything else is automatic! 🎉

---

**Current Status:** Portfolio is ready, just waiting for your `profile.jpg` file!
