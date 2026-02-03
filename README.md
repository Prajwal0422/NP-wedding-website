# Premium South Indian Hindu Wedding Website

A beautiful, responsive wedding invitation website with traditional South Indian Hindu wedding elements, featuring deep maroon and temple gold color scheme.

## 🎨 Features

### ✨ Core Features
- **Elegant Hero Section** with animated couple names and heart symbol
- **Flower Petal Animation** falling across the screen
- **Countdown Timer** to Muhurtham (Wedding ceremony)
- **Background Music Toggle** for Carnatic music
- **Responsive Design** - works perfectly on mobile, tablet, and desktop
- **Traditional Color Scheme** - Deep maroon (#7B1E1E) and temple gold (#FFD700)

### 📋 Sections
1. **Hero/Header** - Couple names with countdown timer
2. **Couple Section** - Side-by-side photos with family details
3. **Wedding Events** - Betrothal, Muhurtham, and Reception details with Google Maps
4. **Gallery** - Photo gallery with lightbox (6 photos)
5. **RSVP Form** - Simple form with name, phone, guests, attendance
6. **Blessings Section** - Parents' names and contact information

### 🎵 Interactive Elements
- Flower petal animation on page load
- Background Carnatic music with toggle control
- Smooth scroll navigation
- Add to Calendar buttons
- PDF invitation download
- Animated elements on scroll

## 🚀 Quick Start

### 1. Customize Names and Details

Open `index.html` and replace the following placeholders:

```html
[BRIDE_NAME] - Replace with bride's name
[GROOM_NAME] - Replace with groom's name
[UPDATE_FATHER_NAME] - Replace with father's name
[UPDATE_MOTHER_NAME] - Replace with mother's name
[CITY] - Replace with city name
[RECEPTION_HALL_NAME] - Replace with reception venue name
[COMPLETE_ADDRESS] - Replace with complete address
```

### 2. Update Photos

Replace the following images in the `images/` folder:
- `RS2.jpeg` - Hero background image
- `RS3.jpeg` - Groom's photo
- `RS4.jpeg` - Bride's photo
- `RS5.jpeg` - Gallery photo
- Additional gallery photos as needed

### 3. Add Audio Files (Optional)

Place these files in the `assets/` folder:
- `carnatic-music.mp3` - Background music
- `bell-chime.mp3` - Bell sound on page load (optional)
- `invitation.pdf` - Downloadable PDF invitation

### 4. Update Event Details

In `index.html`, update:
- Wedding date and time
- Venue names and addresses
- Google Maps embed URLs
- Contact phone numbers and email

### 5. Set Countdown Timer

Edit `js/clock.js` and update the target date:

```javascript
// Target future date/24 hour time/Timezone
let targetDate = moment.tz("2026-02-20 11:45", "Asia/Kolkata");
```

## 📱 Sections Breakdown

### Hero Section
- Animated couple names with heart symbol
- Countdown timer to wedding date (Feb 20, 2026)
- Floral dividers and rangoli design
- "Save our date" button

### Couple Section
- Circular photo frames with gold borders
- Parent names and cities
- Traditional styling with Sanskrit quote

### Events Section
- **Betrothal Ceremony** - Feb 19, 2026, 8:00 AM
- **Wedding Muhurtham** - Feb 20, 2026, 11:45 AM
- **Reception** - Feb 22, 2026, 11:00 AM onwards
- Each event includes Google Maps integration

### Gallery
- Masonry grid layout
- Lightbox functionality for viewing
- 6 photos displayed (easily expandable)

### RSVP Form
- Name (required)
- Phone number (required)
- Number of guests (dropdown)
- Attendance confirmation (Yes/No)
- Thank you message on submission

## 🎨 Color Scheme

```css
--deep-maroon: #5D0E0E
--maroon: #7B1E1E
--temple-gold: #FFD700
--gold: #D4AF37
--dark-gold: #B8860B
--floral-cream: #FEF5E7
--sandalwood: #F4E4C1
--cream: #FFF8DC
```

## 🛠️ Customization Guide

### Change Colors
Edit the `:root` CSS variables in the `<style>` section of `index.html`

### Add More Gallery Photos
Copy an existing `<li>` element in the gallery section and update the image path

### Modify Events
Edit the event cards in the `#fh5co-event` section

### Update Countdown Date
Modify the countdown timer in `js/clock.js`:
```javascript
let targetDate = moment.tz("2026-02-20 11:45", "Asia/Kolkata");
```

## 📦 File Structure

```
├── index.html              # Main HTML file
├── css/
│   ├── style.css          # Main stylesheet
│   ├── animate.css        # Animation library
│   └── ...                # Other CSS files
├── js/
│   ├── main.js            # Main JavaScript
│   ├── clock.js           # Countdown timer
│   └── ...                # Other JS files
├── images/
│   ├── RS2.jpeg           # Hero image
│   ├── RS3.jpeg           # Groom photo
│   ├── RS4.jpeg           # Bride photo
│   └── ...                # Gallery photos
├── assets/
│   ├── carnatic-music.mp3 # Background music
│   ├── bell-chime.mp3     # Bell sound
│   └── invitation.pdf     # PDF invitation
└── fonts/                 # Custom fonts
```

## 🌐 Deployment

### GitHub Pages
1. Push code to GitHub repository
2. Go to Settings > Pages
3. Select main branch
4. Your site will be live at `https://username.github.io/repo-name`

### Custom Domain
1. Add `CNAME` file with your domain
2. Configure DNS settings with your domain provider
3. Point to GitHub Pages

### Other Hosting
Upload all files to your web hosting via FTP or hosting panel

## 📱 Mobile Optimization

- Fully responsive design
- Touch-friendly UI
- Optimized images for fast loading
- Mobile-first approach

## 🎯 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 SEO Optimization

- Meta tags included
- Open Graph tags for social sharing
- Descriptive alt texts for images
- Semantic HTML structure

## 🎵 Audio Files

### Recommended Sources for Carnatic Music
- Use royalty-free Carnatic instrumental music
- Keep file size under 5MB for faster loading
- Format: MP3, 128-192 kbps

### Bell Chime
- Short temple bell sound (2-3 seconds)
- Optional feature - can be disabled

## 🔧 Technical Details

### Dependencies
- jQuery 3.x
- Bootstrap 3.x
- Owl Carousel
- Magnific Popup (lightbox)
- FlipClock (countdown)
- Animate.css

### Performance
- Lazy loading for images
- Minified CSS and JS
- Optimized animations
- Fast page load time

## 🙏 Credits

Based on HTML theme from [FreeHTML5.co](https://freehtml5.co/wedding-free-html5-bootstrap-template-for-wedding-websites)

Enhanced with:
- Traditional South Indian wedding aesthetics
- Premium color scheme and animations
- Modern interactive features
- Mobile-first responsive design

Fonts: Great Vibes, Cinzel, Playfair Display, Work Sans, Lora

---

**Made with ❤️ for your special day**

*May your wedding be filled with joy, blessings, and beautiful memories!*

## 🎊 Final Checklist

- [ ] Replace all placeholder names ([BRIDE_NAME], [GROOM_NAME], etc.)
- [ ] Update all photos (RS2.jpeg, RS3.jpeg, RS4.jpeg, etc.)
- [ ] Add audio files to assets/ folder (optional)
- [ ] Update event dates and times
- [ ] Update venue addresses
- [ ] Update Google Maps embeds
- [ ] Add PDF invitation to assets/
- [ ] Update contact information
- [ ] Set countdown timer date in js/clock.js
- [ ] Test on mobile devices
- [ ] Test RSVP form
- [ ] Test all navigation links
- [ ] Test music toggle
- [ ] Check all images load correctly
- [ ] Deploy to hosting/GitHub Pages
