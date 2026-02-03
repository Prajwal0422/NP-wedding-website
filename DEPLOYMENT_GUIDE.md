# Deployment Guide - Wedding Website

This guide covers multiple ways to deploy your wedding website online.

---

## 🚀 Option 1: GitHub Pages (Recommended - FREE)

### Why GitHub Pages?
- ✅ Completely FREE
- ✅ HTTPS included
- ✅ Custom domain support
- ✅ Easy updates
- ✅ Version control
- ✅ No server management

### Step-by-Step Instructions

#### 1. Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Follow the registration process

#### 2. Create New Repository
1. Click the "+" icon (top right)
2. Select "New repository"
3. Name it: `wedding-website` (or any name)
4. Make it **Public**
5. Click "Create repository"

#### 3. Upload Your Files

**Option A: Using GitHub Web Interface**
1. Click "uploading an existing file"
2. Drag and drop ALL your files
3. Write commit message: "Initial wedding website"
4. Click "Commit changes"

**Option B: Using Git Command Line**
```bash
# Navigate to your website folder
cd path/to/your/wedding-website

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial wedding website"

# Add remote
git remote add origin https://github.com/YOUR_USERNAME/wedding-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### 4. Enable GitHub Pages
1. Go to repository Settings
2. Scroll to "Pages" section (left sidebar)
3. Under "Source", select "main" branch
4. Click "Save"
5. Wait 2-3 minutes

#### 5. Access Your Website
Your site will be live at:
```
https://YOUR_USERNAME.github.io/wedding-website/
```

### Using Custom Domain (Optional)

#### 1. Purchase Domain
Buy from: GoDaddy, Namecheap, Google Domains, etc.
Example: `priyarahulwedding.com`

#### 2. Update CNAME File
Create/edit `CNAME` file in your repository:
```
priyarahulwedding.com
```

#### 3. Configure DNS
In your domain provider's DNS settings:

**For Apex Domain (example.com):**
```
Type: A
Name: @
Value: 185.199.108.153
Value: 185.199.109.153
Value: 185.199.110.153
Value: 185.199.111.153
```

**For WWW Subdomain:**
```
Type: CNAME
Name: www
Value: YOUR_USERNAME.github.io
```

#### 4. Wait for DNS Propagation
- Usually takes 1-24 hours
- Check status: [whatsmydns.net](https://www.whatsmydns.net)

---

## 🌐 Option 2: Netlify (FREE)

### Why Netlify?
- ✅ FREE tier available
- ✅ Drag-and-drop deployment
- ✅ HTTPS included
- ✅ Custom domain support
- ✅ Continuous deployment

### Step-by-Step Instructions

#### 1. Create Netlify Account
1. Go to [netlify.com](https://www.netlify.com)
2. Sign up (can use GitHub account)

#### 2. Deploy Site

**Option A: Drag and Drop**
1. Click "Add new site" → "Deploy manually"
2. Drag your entire website folder
3. Wait for deployment
4. Your site is live!

**Option B: Connect to GitHub**
1. Click "Add new site" → "Import an existing project"
2. Choose GitHub
3. Select your repository
4. Click "Deploy site"

#### 3. Custom Domain (Optional)
1. Go to "Domain settings"
2. Click "Add custom domain"
3. Follow DNS configuration instructions

---

## 💻 Option 3: Vercel (FREE)

### Why Vercel?
- ✅ FREE tier
- ✅ Fast deployment
- ✅ HTTPS included
- ✅ GitHub integration

### Step-by-Step Instructions

#### 1. Create Vercel Account
1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub

#### 2. Deploy
1. Click "Add New" → "Project"
2. Import your GitHub repository
3. Click "Deploy"
4. Your site is live!

---

## 🖥️ Option 4: Traditional Web Hosting

### Recommended Hosts
- **Hostinger** - Budget-friendly
- **Bluehost** - Popular choice
- **SiteGround** - Good performance
- **GoDaddy** - Well-known

### Step-by-Step Instructions

#### 1. Purchase Hosting Plan
- Choose shared hosting (cheapest)
- Register domain (if not already owned)

#### 2. Access cPanel/File Manager
- Login to your hosting account
- Open cPanel or File Manager

#### 3. Upload Files

**Via File Manager:**
1. Navigate to `public_html` folder
2. Click "Upload"
3. Select all your website files
4. Wait for upload to complete

**Via FTP:**
1. Download FileZilla (free FTP client)
2. Connect using FTP credentials from host
3. Upload all files to `public_html`

#### 4. Access Your Website
Your site will be live at your domain:
```
https://yourdomain.com
```

---

## 📱 Option 5: Firebase Hosting (FREE)

### Why Firebase?
- ✅ FREE tier (generous)
- ✅ Fast CDN
- ✅ HTTPS included
- ✅ Custom domain support

### Step-by-Step Instructions

#### 1. Install Firebase CLI
```bash
npm install -g firebase-tools
```

#### 2. Login to Firebase
```bash
firebase login
```

#### 3. Initialize Project
```bash
cd your-wedding-website
firebase init hosting
```

Select:
- Use existing project or create new
- Public directory: `.` (current directory)
- Single-page app: No
- Overwrite index.html: No

#### 4. Deploy
```bash
firebase deploy
```

Your site will be live at:
```
https://your-project.web.app
```

---

## 🔧 Pre-Deployment Checklist

Before deploying, ensure:

### Content
- [ ] All names updated
- [ ] All photos replaced
- [ ] Event dates correct
- [ ] Venue addresses updated
- [ ] Contact info updated
- [ ] Countdown timer date set

### Files
- [ ] All images optimized
- [ ] Audio files added (if using)
- [ ] PDF invitation added (if using)
- [ ] No placeholder text remaining

### Testing
- [ ] Test on desktop browser
- [ ] Test on mobile phone
- [ ] Test on tablet
- [ ] All links work
- [ ] RSVP form works
- [ ] Gallery lightbox works
- [ ] Music toggle works (if using)
- [ ] Countdown timer works

### SEO
- [ ] Meta tags updated
- [ ] Title updated
- [ ] Description updated
- [ ] Open Graph image set
- [ ] Keywords updated

---

## 🔄 Updating Your Website

### GitHub Pages
1. Edit files locally
2. Commit changes:
```bash
git add .
git commit -m "Update wedding details"
git push
```
3. Wait 2-3 minutes for changes to appear

### Netlify/Vercel
- Changes auto-deploy when you push to GitHub
- Or drag-and-drop new files

### Traditional Hosting
- Upload changed files via FTP or File Manager
- Overwrite existing files

---

## 📊 Post-Deployment Tasks

### 1. Test Everything
- Visit your live site
- Test on multiple devices
- Check all links
- Test forms

### 2. Share Your Website
- Share URL with family
- Post on social media
- Include in physical invitations
- Send via WhatsApp

### 3. Monitor (Optional)
- Add Google Analytics
- Track visitor count
- Monitor RSVP submissions

### 4. Backup
- Keep local copy of all files
- Export RSVP data regularly

---

## 🆘 Troubleshooting

### Site Not Loading
- **Check DNS:** Wait 24 hours for propagation
- **Check HTTPS:** Ensure SSL certificate is active
- **Clear Cache:** Clear browser cache and try again

### Images Not Showing
- **Check Paths:** Ensure image paths are correct
- **Check Upload:** Verify all images uploaded
- **Check Names:** File names are case-sensitive

### Countdown Not Working
- **Check Date:** Verify date format in `js/clock.js`
- **Check Timezone:** Ensure timezone is correct
- **Check Console:** Open browser console (F12) for errors

### Music Not Playing
- **Check File:** Ensure audio file uploaded
- **Check Path:** Verify path in HTML
- **Check Format:** Use MP3 format
- **Check Size:** Keep under 5MB

---

## 💡 Pro Tips

### Performance
1. **Compress Images:** Use TinyPNG or similar
2. **Optimize Audio:** Use 128kbps MP3
3. **Enable Caching:** Most hosts do this automatically
4. **Use CDN:** GitHub Pages/Netlify include CDN

### Security
1. **Use HTTPS:** All recommended hosts provide this
2. **Keep Backups:** Download site files regularly
3. **Update Regularly:** Keep content fresh

### Sharing
1. **Short URL:** Use bit.ly for easier sharing
2. **QR Code:** Generate QR code for physical invitations
3. **Social Media:** Share with nice preview image

---

## 📱 Mobile-Specific Testing

Test these on actual mobile devices:
- [ ] Navigation menu works
- [ ] Photos load quickly
- [ ] Forms are easy to fill
- [ ] Buttons are easy to tap
- [ ] Text is readable
- [ ] No horizontal scrolling

---

## 🎯 Domain Name Ideas

If you need a domain name:
- `priyarahulwedding.com`
- `priyawedrahul.com`
- `priyaandrahul.com`
- `priyarahul2026.com`
- `weddingpriyarahul.com`

**Tips:**
- Keep it short and memorable
- Use couple names
- Add year if names are common
- Check availability on Namecheap/GoDaddy

---

## 📞 Support Resources

### GitHub Pages
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Custom Domain Guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

### Netlify
- [Netlify Docs](https://docs.netlify.com)
- [Custom Domain Guide](https://docs.netlify.com/domains-https/custom-domains/)

### General Help
- Check browser console (F12) for errors
- Search error messages on Google
- Ask in web development forums

---

## ✅ Final Deployment Checklist

- [ ] Website fully customized
- [ ] All content tested
- [ ] Hosting platform chosen
- [ ] Domain purchased (if using custom)
- [ ] Files uploaded/deployed
- [ ] DNS configured (if custom domain)
- [ ] HTTPS working
- [ ] Mobile tested
- [ ] Shared with family
- [ ] Backup created

---

**Congratulations! Your wedding website is now live! 🎉**

*Share the URL with your guests and let them celebrate with you online!*

---

## 📧 Example Invitation Message

```
🎊 You're Invited! 🎊

Join us in celebrating the wedding of
Priya & Rahul

📅 February 20, 2026
📍 Sri Chowdeshwari Temple, Kargal

View our wedding invitation and RSVP:
🔗 https://priyarahulwedding.com

We look forward to your blessings!

With love,
Priya & Rahul
```

---

*Need help? Review this guide or check the CUSTOMIZATION_GUIDE.md*
