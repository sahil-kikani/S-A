# Sahil & Aayushi - Wedding Website

A beautiful, interactive wedding invitation website built with HTML, CSS, and JavaScript. Fully responsive and ready to deploy on Vercel.

## Features

✨ **Interactive Design**
- Elegant tap-to-reveal invitation
- Scratch cards for date reveal
- Live countdown timer
- Smooth animations and transitions

📱 **Fully Responsive**
- Mobile-friendly design
- Works on all devices
- Touch-enabled interactions

🎨 **Beautiful UI**
- Soft pink and burgundy color scheme
- Elegant serif typography
- Professional layout
- Customizable sections

📋 **Complete Sections**
- Hero landing page
- Invitation card
- Save the date
- Countdown timer
- Our story/photos
- Venue & details
- RSVP form

## Quick Start - Deploy to Vercel

### Option 1: Using Git (Recommended)

1. **Create a GitHub repository**
   - Go to github.com and create a new public repository
   - Name it `wedding` or similar

2. **Initialize Git locally**
   ```bash
   cd your-project-folder
   git init
   git add .
   git commit -m "Initial wedding website"
   git remote add origin https://github.com/yourusername/wedding.git
   git branch -M main
   git push -u origin main
   ```

3. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy"
   - Your site will be live at `your-project.vercel.app`

### Option 2: Drag & Drop

1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag and drop your project folder
3. Vercel will automatically deploy it

## Customization Guide

### 1. Edit Names and Date
Open `index.html` and search for:
- `Sahil` → Replace with groom's name
- `Aayushi` → Replace with bride's name
- `November 11, 2028` → Replace with your wedding date

### 2. Add Couple Photo
1. Upload your photo to the same folder as `index.html`
2. Find the line with `photo-placeholder`
3. Replace:
   ```html
   <div class="photo-placeholder">
       Replace with your couple photo
   </div>
   ```
   With:
   ```html
   <img src="your-photo.jpg" class="story-photo" alt="Couple Photo">
   ```

### 3. Update Venue Details
Find the "Wedding Details" section and update:
- Wedding date and time
- Venue name and address
- Dress code
- Accommodation information

### 4. Add Your Story
Find the "Our Story" section and replace the placeholder text with your love story.

### 5. Set Up RSVP
Update the email address:
- Find `sahil.aayushi@example.com`
- Replace with your actual email
- Update RSVP deadline date

### 6. Customize Colors (Optional)
At the top of `index.html`, find the `:root` section:
```css
:root {
    --primary-color: #8b4a5c;      /* Change burgundy */
    --secondary-color: #a85a6f;    /* Change accent */
    --accent-color: #b8906a;       /* Change gold */
    --light-bg: #fef9f3;           /* Change background */
    --cream-bg: #faf5f0;           /* Change cream */
}
```

## File Structure

```
.
├── index.html          # Main website file (all HTML, CSS, JS in one)
├── vercel.json         # Vercel configuration
└── README.md          # This file
```

## What You Can Customize

- [x] Names of bride and groom
- [x] Wedding date and time
- [x] Venue location
- [x] Photos (couple, venue)
- [x] Colors and fonts
- [x] RSVP email
- [x] Guest accommodations
- [x] Dress code
- [x] Any text content

## How It Works

The website includes:
1. **Navigation header** - Sticky header with smooth scrolling
2. **Hero section** - Eye-catching landing with interactive seal
3. **Invitation** - Formal invitation card
4. **Save the Date** - Interactive scratch cards reveal date
5. **Countdown** - Live countdown timer (updates every second)
6. **Story** - Your love story and couple photos
7. **Venue** - Wedding details and accommodation info
8. **RSVP** - Guest confirmation link
9. **Footer** - Final message

## Mobile Optimization

The website is fully optimized for:
- Desktop (1200px+)
- Tablet (768px - 1199px)
- Mobile (480px - 767px)
- Small phones (<480px)

## Browser Support

Works on:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Tips for Best Results

1. **Use a high-quality couple photo** (at least 400x500px)
2. **Test on mobile** before sharing link
3. **Update venue details clearly** so guests know where to go
4. **Use a professional email** for RSVP
5. **Share your Vercel link** instead of re-uploading
6. **Keep RSVP deadline realistic** (at least 2 weeks before)

## Need Help?

### Vercel Deployment Issues
- Check vercel.json is in root folder
- Ensure all files are uploaded
- Clear browser cache and reload

### Customization Issues
- Use Firefox/Chrome DevTools (F12) to inspect
- Make sure image filenames match exactly
- Check that HTML syntax is correct after edits

### Email Issues
- Gmail users: May need app password instead of regular password
- Use mailto: links for simple email functionality

## License

This template is free to use for personal and commercial purposes.

## Questions?

Refer to the inline comments in index.html for specific sections. The code is well-structured and easy to modify!

Happy wedding! 💕
# S-A
