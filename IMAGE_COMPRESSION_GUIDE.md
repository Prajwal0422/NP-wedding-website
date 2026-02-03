# Image Compression Guide

## ⚠️ Important: Your Images Need Compression

The original images (RS2.jpeg, RS3.jpeg, RS4.jpeg, RS5.jpeg) are too large for GitHub:
- RS5.jpeg: 45.2 MB
- RS3.jpeg: 38.2 MB
- RS4.jpeg: 35.3 MB
- RS2.jpeg: 34.0 MB

**Total: ~152 MB** (GitHub recommends files under 50MB total)

---

## 🎯 Recommended Image Sizes

### For Web Performance:
- **Hero Background (RS2.jpeg)**: 1920x1080px, < 500KB
- **Couple Photos (RS3, RS4)**: 800x800px, < 200KB each
- **Gallery Photos (RS5)**: 1200x800px, < 300KB

---

## 🛠️ How to Compress Images

### Option 1: Online Tools (Easiest)

#### TinyPNG (Recommended)
1. Go to [tinypng.com](https://tinypng.com)
2. Upload your images (RS2, RS3, RS4, RS5)
3. Download compressed versions
4. Replace the original files

#### Squoosh (Google)
1. Go to [squoosh.app](https://squoosh.app)
2. Upload each image
3. Adjust quality to 80-85%
4. Download and replace

### Option 2: Using Photoshop
1. Open image in Photoshop
2. File → Export → Save for Web
3. Choose JPEG quality: 80-85%
4. Resize if needed:
   - RS2: 1920x1080px
   - RS3, RS4: 800x800px
   - RS5: 1200x800px
5. Save and replace

### Option 3: Using Free Software

#### GIMP (Free Photoshop Alternative)
1. Download GIMP: [gimp.org](https://www.gimp.org)
2. Open image
3. Image → Scale Image (resize if needed)
4. File → Export As
5. Choose JPEG, quality 80-85%
6. Save and replace

#### IrfanView (Windows)
1. Download IrfanView: [irfanview.com](https://www.irfanview.com)
2. Open image
3. Image → Resize/Resample
4. File → Save As → JPEG, quality 80
5. Replace original

---

## 📋 Step-by-Step Process

### 1. Compress Images
Use any tool above to compress all 4 images

### 2. Replace Files
Replace the original files in the `images/` folder:
- images/RS2.jpeg (hero background)
- images/RS3.jpeg (groom photo)
- images/RS4.jpeg (bride photo)
- images/RS5.jpeg (gallery photo)

### 3. Update .gitignore
Remove these lines from `.gitignore`:
```
images/RS2.jpeg
images/RS3.jpeg
images/RS4.jpeg
images/RS5.jpeg
```

### 4. Commit and Push
```bash
git add images/
git commit -m "Add compressed wedding photos"
git push origin main
```

---

## ✅ Target File Sizes

After compression, your files should be:
- RS2.jpeg: ~300-500 KB (hero background)
- RS3.jpeg: ~150-200 KB (groom photo)
- RS4.jpeg: ~150-200 KB (bride photo)
- RS5.jpeg: ~200-300 KB (gallery photo)

**Total: ~1-1.5 MB** (much better!)

---

## 🎨 Quality Settings

### For Best Results:
- **JPEG Quality**: 80-85%
- **Format**: JPEG (not PNG for photos)
- **Color Space**: sRGB
- **Progressive**: Yes (for web)

### Don't Go Below:
- Quality: 70% (images will look bad)
- Resolution: Minimum sizes listed above

---

## 🚀 Quick Online Compression

**Fastest Method:**
1. Go to [tinypng.com](https://tinypng.com)
2. Drag all 4 images at once
3. Wait for compression (automatic)
4. Download all
5. Replace in `images/` folder
6. Git add, commit, push

**Time: 2-3 minutes**

---

## 📱 Current Status

✅ Website code pushed to GitHub
✅ All features working
✅ Documentation complete
❌ Large images excluded (need compression)

**Next Step:** Compress images and push them

---

## 🆘 If You Need Help

### Can't Compress?
You can use placeholder images temporarily:
1. Find smaller images online (free stock photos)
2. Use them temporarily
3. Replace with compressed originals later

### Alternative: Use Image CDN
Upload images to:
- Cloudinary (free tier)
- ImgBB
- Imgur

Then update image URLs in `index.html`

---

## 📞 Testing After Compression

After pushing compressed images:
1. Visit: `https://prajwal0422.github.io/NP-wedding-website/`
2. Check if images load
3. Test on mobile
4. Verify page speed

---

**Remember: Compressed images = Faster website = Better user experience!**

*Your guests will thank you for the fast loading times!* 🚀
