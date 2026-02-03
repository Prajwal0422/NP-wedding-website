# Wedding Website Customization Guide

This guide will help you customize your premium South Indian Hindu wedding website step by step.

## 📝 Step 1: Update Personal Information

### In `index.html`, find and replace:

#### Couple Names (Multiple locations)
```html
<!-- Search for: -->
[BRIDE_NAME]
[GROOM_NAME]

<!-- Replace with actual names, for example: -->
Priya
Rahul
```

#### Parents' Names (4 locations - bride's and groom's parents)
```html
<!-- Search for: -->
[UPDATE_FATHER_NAME]
[UPDATE_MOTHER_NAME]

<!-- Replace with actual names, for example: -->
Mr. Rajesh Kumar
Mrs. Lakshmi Rajesh
```

#### Cities
```html
<!-- Search for: -->
[CITY]

<!-- Replace with actual city, for example: -->
Bangalore, Karnataka
```

#### Reception Venue
```html
<!-- Search for: -->
[RECEPTION_HALL_NAME]
[COMPLETE_ADDRESS]

<!-- Replace with actual venue details, for example: -->
Grand Palace Convention Hall
123 MG Road, Bangalore, Karnataka - 560001
```

## 📸 Step 2: Update Photos

### Required Photos:

1. **Hero Background** (`images/RS2.jpeg`)
   - Recommended size: 1920x1080px
   - Should be a beautiful couple photo
   - Will be used as the main header background

2. **Groom Photo** (`images/RS3.jpeg`)
   - Recommended size: 800x800px (square)
   - Will be displayed in a circular frame
   - Should be a clear portrait

3. **Bride Photo** (`images/RS4.jpeg`)
   - Recommended size: 800x800px (square)
   - Will be displayed in a circular frame
   - Should be a clear portrait

4. **Gallery Photos** (6-8 photos recommended)
   - Current photos: RS2.jpeg, RS3.jpeg, RS4.jpeg, RS5.jpeg, and WhatsApp images
   - Recommended size: 1200x800px
   - Can add more by copying the gallery item code

### To Add More Gallery Photos:

```html
<!-- Copy this block and update the image path: -->
<li class="one-third animate-box" data-animate-effect="fadeIn" style="background-image: url(images/YOUR_NEW_PHOTO.jpeg); "> 
    <a href="images/YOUR_NEW_PHOTO.jpeg" class="gallery-item">
        <div class="case-studies-summary">
            <span class="gallery-overlay">👁️ View</span>
        </div>
    </a>
</li>
```

## 📅 Step 3: Update Event Details

### Wedding Date and Time

Find the countdown timer section and update:
```html
<h2 class="wedding-date">20th February 2026</h2>
```

### Event Cards

Update three event cards:

#### 1. Betrothal Ceremony
```html
<h3>Betrothal Ceremony</h3>
<span>19 February 2026</span>  <!-- Update date -->
<span>8:00 AM</span>            <!-- Update time -->
<p class="venue-details">At <b>Sri Chowdeshwari Mahalasa Temple, Kargal</b></p>
<p class="venue-address">B.H Road, State Highway 50, Kargal, Karnataka – 577421</p>
```

#### 2. Wedding Muhurtham
```html
<h3>Wedding Muhurtham</h3>
<span>20 February 2026</span>   <!-- Update date -->
<span>11:45 AM</span>            <!-- Update time -->
<p class="venue-details">At <b>Sri Chowdeshwari Mahalasa Temple, Kargal</b></p>
<p class="venue-address">B.H Road, State Highway 50, Kargal, Karnataka – 577421</p>
```

#### 3. Reception
```html
<h3>Reception</h3>
<span>22 February 2026</span>   <!-- Update date -->
<span>11:00 AM Onwards</span>   <!-- Update time -->
<p class="venue-details">At <b>[RECEPTION_HALL_NAME]</b></p>
<p class="venue-address">[COMPLETE_ADDRESS]</p>
```

## 🗺️ Step 4: Update Google Maps

### For Each Event:

1. Go to [Google Maps](https://www.google.com/maps)
2. Search for your venue
3. Click "Share" → "Embed a map"
4. Copy the iframe code
5. Replace the existing iframe in the event card

Example:
```html
<iframe 
    src="https://maps.google.com/?q=YOUR_VENUE_NAME&output=embed" 
    width="300" 
    height="200" 
    style="border:0; border-radius:10px; margin-top:15px;" 
    allowfullscreen="" 
    loading="lazy" 
    referrerpolicy="no-referrer-when-downgrade">
</iframe>
```

## ⏰ Step 5: Set Countdown Timer

### Edit `js/clock.js`:

Find this line:
```javascript
let targetDate = moment.tz("2023-10-29 12:00", "Asia/Kolkata");
```

Update to your wedding date and time:
```javascript
let targetDate = moment.tz("2026-02-20 11:45", "Asia/Kolkata");
```

Format: `"YYYY-MM-DD HH:MM"`

## 📞 Step 6: Update Contact Information

Find the "Contact Us" section:
```html
<p><strong>For queries:</strong><br>
📞 +91 XXXXXXXXXX<br>
📧 contact@wedding.com</p>
```

Replace with actual contact details:
```html
<p><strong>For queries:</strong><br>
📞 +91 9876543210<br>
📧 priya.rahul.wedding@gmail.com</p>
```

## 🎵 Step 7: Add Audio Files (Optional)

### 1. Background Music

1. Get a Carnatic instrumental music file (royalty-free)
2. Name it `carnatic-music.mp3`
3. Place it in the `assets/` folder
4. The music toggle button will automatically work

### 2. Bell Chime (Optional)

1. Get a temple bell sound (2-3 seconds)
2. Name it `bell-chime.mp3`
3. Place it in the `assets/` folder
4. Uncomment these lines in the script section:
```javascript
// Uncomment to play bell sound on load
const bellSound = new Audio('assets/bell-chime.mp3');
bellSound.play();
```

## 📄 Step 8: Add PDF Invitation

1. Create your wedding invitation PDF
2. Name it `invitation.pdf`
3. Place it in the `assets/` folder
4. The download button will automatically work

## 🎨 Step 9: Customize Colors (Optional)

### Edit CSS Variables in `index.html`:

Find the `:root` section:
```css
:root {
    --maroon: #7B1E1E;           /* Main maroon color */
    --gold: #D4AF37;             /* Gold accent */
    --cream: #FFF8DC;            /* Cream background */
    --dark-gold: #B8860B;        /* Dark gold */
    --sandalwood: #F4E4C1;       /* Sandalwood tone */
    --temple-gold: #FFD700;      /* Bright gold */
    --floral-cream: #FEF5E7;     /* Light cream */
    --deep-maroon: #5D0E0E;      /* Deep maroon */
}
```

Change any color by updating the hex code.

## 🌐 Step 10: Update Meta Tags for SEO

### Update these meta tags in `<head>`:

```html
<title>Priya ❤️ Rahul - Wedding Invitation</title>
<meta name="description" content="Join us in celebrating the wedding of Priya and Rahul on February 20, 2026" />
<meta name="keywords" content="priya,rahul,wedding,invitation,hindu,traditional,south indian" />
<meta name="author" content="Priya & Rahul" />

<!-- Open Graph for social sharing -->
<meta property="og:title" content="Priya ❤️ Rahul - Wedding Invitation">
<meta property="og:description" content="Join us in celebrating our traditional South Indian Hindu wedding.">
<meta property="og:url" content="https://your-website-url.com">
```

## 📱 Step 11: Test Your Website

### Checklist:

- [ ] All names are updated
- [ ] All photos load correctly
- [ ] Countdown timer shows correct date
- [ ] All event details are correct
- [ ] Google Maps work for all venues
- [ ] Contact information is correct
- [ ] RSVP form works
- [ ] PDF download works (if added)
- [ ] Music toggle works (if audio added)
- [ ] Website looks good on mobile
- [ ] Website looks good on tablet
- [ ] Website looks good on desktop
- [ ] All navigation links work
- [ ] Gallery lightbox works

### Test on Multiple Devices:

1. **Desktop** - Chrome, Firefox, Safari, Edge
2. **Mobile** - iOS Safari, Chrome Mobile
3. **Tablet** - iPad, Android tablets

## 🚀 Step 12: Deploy Your Website

### Option 1: GitHub Pages (Free)

1. Create a GitHub account
2. Create a new repository
3. Upload all files
4. Go to Settings → Pages
5. Select main branch
6. Your site will be live!

### Option 2: Custom Domain

1. Purchase a domain (e.g., priyarahulwedding.com)
2. Update the `CNAME` file with your domain
3. Configure DNS settings
4. Point to your hosting

### Option 3: Web Hosting

1. Choose a hosting provider
2. Upload files via FTP or cPanel
3. Your site will be live at your hosting URL

## 🎯 Common Issues and Solutions

### Issue: Countdown timer not working
**Solution:** Check `js/clock.js` and ensure the date format is correct

### Issue: Images not loading
**Solution:** Check file paths and ensure images are in the `images/` folder

### Issue: Music not playing
**Solution:** Ensure `carnatic-music.mp3` is in the `assets/` folder and the path is correct

### Issue: RSVP form not submitting
**Solution:** The current form shows a thank you message. For actual submissions, integrate with a backend service or Google Forms

### Issue: Google Maps not showing
**Solution:** Check the iframe embed code and ensure it's properly formatted

## 💡 Pro Tips

1. **Optimize Images:** Compress images before uploading to improve load time
2. **Test Early:** Test on mobile devices early in the customization process
3. **Backup:** Keep a backup of the original files before making changes
4. **Browser Cache:** Clear browser cache when testing changes
5. **Mobile First:** Always check how it looks on mobile - most guests will view on phones

## 📞 Need Help?

If you encounter any issues:
1. Check this guide again
2. Review the code comments in `index.html`
3. Test in a different browser
4. Check browser console for errors (F12)

---

**Congratulations on your upcoming wedding! 🎊**

*This website will be a beautiful digital invitation for your guests.*
