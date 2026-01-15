# How to Add Your Profile Picture

## Quick Steps

1. **Save the photo you provided** (the one in your school uniform) to your computer

2. **Rename the file** to `profile.jpg`

3. **Copy the file** to the `public` folder in this project:
   ```
   railway-deployment/public/profile.jpg
   ```

4. **That's it!** The portfolio is already configured to use this image.

## Detailed Instructions

### Option 1: Using File Explorer (Windows)

1. Locate your profile picture file on your computer
2. Right-click the file and select "Rename"
3. Change the name to `profile.jpg`
4. Copy the file (Ctrl+C)
5. Navigate to your project folder: `railway-deployment/public/`
6. Paste the file (Ctrl+V)

### Option 2: Using Command Line

```bash
# Navigate to the public folder
cd railway-deployment/public

# Copy your image file here and rename it
# Replace 'path/to/your/image.jpg' with your actual image path
copy "path/to/your/image.jpg" profile.jpg
```

### Option 3: Using a Different Filename

If you want to keep your original filename (e.g., `my-photo.png`):

1. Copy your image to the `public` folder with any name
2. Open `public/index.html` in a text editor
3. Find this line (around line 60):
   ```html
   <img src="profile.jpg" alt="Tejaswini Kawade" id="profileImage">
   ```
4. Change `profile.jpg` to your filename:
   ```html
   <img src="my-photo.png" alt="Tejaswini Kawade" id="profileImage">
   ```
5. Save the file

## Image Recommendations

For best results:
- **Format:** JPG, JPEG, or PNG
- **Size:** 400x400 pixels or larger (square format works best)
- **File size:** Under 1MB for faster loading
- **Quality:** High resolution, well-lit photo

## Troubleshooting

**Image not showing?**
- Check that the filename matches exactly (case-sensitive)
- Make sure the file is in the `public` folder
- Clear your browser cache (Ctrl+Shift+R)
- Check the browser console for errors (F12)

**Image looks stretched or distorted?**
- The CSS is set to maintain aspect ratio
- For best results, use a square image (same width and height)
- You can crop your image to square format using:
  - Windows Photos app
  - Online tools like [Canva](https://www.canva.com)
  - [Photopea](https://www.photopea.com) (free Photoshop alternative)

## Testing

After adding your photo:

1. Start the server:
   ```bash
   npm start
   ```

2. Open your browser to:
   ```
   http://localhost:3000
   ```

3. You should see your profile picture in the hero section with a floating animation!

## Need Help?

If you're having trouble, feel free to reach out:
- Email: tejaswinikawade@gmail.com
- Or check the browser console (F12) for error messages

---

**Note:** The image you provided (in school uniform) looks professional and is perfect for the portfolio!
