# Quick Start Guide - 5 Minutes Setup

## 🚀 Essential Changes (Must Do)

### 1. Update Names in `index.html`

**Find and Replace:**
```
[BRIDE_NAME]          → Your bride's name
[GROOM_NAME]          → Your groom's name
[UPDATE_FATHER_NAME]  → Father's name (4 places)
[UPDATE_MOTHER_NAME]  → Mother's name (4 places)
[CITY]                → Your city (2 places)
```

**How to do it:**
- Open `index.html` in any text editor
- Use Find & Replace (Ctrl+H or Cmd+H)
- Replace each placeholder with actual names

---

### 2. Update Wedding Date

**In `index.html`:**
```html
<!-- Find this line: -->
<h2 class="wedding-date">20th February 2026</h2>

<!-- Change to your date: -->
<h2 class="wedding-date">15th March 2026</h2>
```

**In `js/clock.js`:**
```javascript
// Find this line:
let targetDate = moment.tz("2023-10-29 12:00", "Asia/Kolkata");

// Change to your wedding date and time:
let targetDate = moment.tz("2026-03-15 11:30", "Asia/Kolkata");
```

---

### 3. Replace Photos

**Required Photos:**
- `images/RS2.jpeg` - Main hero background (couple photo)
- `images/RS3.jpeg` - Groom's photo (square, 800x800px)
- `images/RS4.jpeg` - Bride's photo (square, 800x800px)

**Just replace these files with your photos (keep the same names)**

---

### 4. Update Event Details

**Find these three sections in `index.html` and update:**

```html
<!-- Betrothal -->
<span>19 February 2026</span>  → Your date
<span>8:00 AM</span>            → Your time

<!-- Wedding Muhurtham -->
<span>20 February 2026</span>   → Your date
<span>11:45 AM</span>            → Your time

<!-- Reception -->
<span>22 February 2026</span>   → Your date
<span>11:00 AM Onwards</span>   → Your time
```

---

### 5. Update Contact Info

**Find and update:**
```html
📞 +91 XXXXXXXXXX  → Your phone number
📧 contact@wedding.com  → Your email
```

---

## ✅ You're Done!

Your website is now ready to use! 

### Next Steps:
1. Open `index.html` in a browser to preview
2. Test on your phone
3. Deploy to GitHub Pages or web hosting

---

## 🎨 Optional Enhancements

### Add Background Music
1. Get a Carnatic music MP3 file
2. Name it `carnatic-music.mp3`
3. Put it in `assets/` folder
4. Music toggle will work automatically!

### Add PDF Invitation
1. Create your invitation PDF
2. Name it `invitation.pdf`
3. Put it in `assets/` folder
4. Download button will work automatically!

### Update Venue Addresses
Search for these in `index.html`:
- `Sri Chowdeshwari Mahalasa Temple, Kargal`
- `[RECEPTION_HALL_NAME]`
- `[COMPLETE_ADDRESS]`

Replace with your actual venues.

---

## 📱 Testing Checklist

- [ ] Open `index.html` in browser
- [ ] Check all names are correct
- [ ] Verify countdown timer shows correct date
- [ ] Test on mobile phone
- [ ] Click all navigation links
- [ ] Test RSVP form
- [ ] Check gallery photos

---

## 🚀 Deploy to GitHub Pages (Free Hosting)

1. Create GitHub account (if you don't have one)
2. Create new repository
3. Upload all files
4. Go to Settings → Pages
5. Select main branch → Save
6. Your site is live! 🎉

**URL will be:** `https://yourusername.github.io/repository-name`

---

## 💡 Pro Tips

- **Use Ctrl+F (Cmd+F)** to find text in `index.html`
- **Keep original files as backup** before editing
- **Test on mobile** - most guests will view on phones
- **Compress images** before uploading for faster loading

---

## 🆘 Common Issues

**Countdown not working?**
→ Check date format in `js/clock.js`: `"YYYY-MM-DD HH:MM"`

**Photos not showing?**
→ Make sure photos are in `images/` folder with correct names

**Music not playing?**
→ Ensure `carnatic-music.mp3` is in `assets/` folder

---

## 📚 Need More Help?

See detailed guides:
- `CUSTOMIZATION_GUIDE.md` - Complete customization guide
- `README.md` - Full documentation

---

**That's it! Your wedding website is ready! 🎊💒**

*Estimated setup time: 5-10 minutes*
