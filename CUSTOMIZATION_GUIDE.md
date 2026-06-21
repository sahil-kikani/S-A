# Wedding Website - Customization Guide

## Quick Edits in 5 Minutes

### 1. Change Names
In `index.html`, find (Ctrl+F / Cmd+F) and replace:
- `Sahil` → Your groom's name
- `Aayushi` → Your bride's name

**Lines to edit:**
- Line ~100: Logo (S & A)
- Line ~330: Main invitation section

### 2. Change Wedding Date
Find and replace:
- `November 11, 2028` → Your wedding date
- `11 · 11 · 2028` → Your date format

**Lines to edit:**
- Line ~275: Hero section
- Line ~356: Countdown date
- Line ~360: Wedding details

### 3. Add Couple Photo
1. Save your photo to the same folder as `index.html`
   - Use JPG or PNG format
   - Name: `couple.jpg` (or any name)

2. Find this section (line ~420):
   ```html
   <div class="photo-placeholder">
       Replace with your couple photo
   </div>
   ```

3. Replace with:
   ```html
   <img src="couple.jpg" class="story-photo" alt="Sahil & Aayushi">
   ```

### 4. Update Email for RSVP
Find: `sahil.aayushi@example.com`

Replace with your actual email. Update both locations:
- Line ~484 (RSVP button)
- Line ~488 (RSVP text)

### 5. Update RSVP Deadline
Find: `October 15, 2028`

Change to your RSVP deadline date

## Detailed Customizations

### Change Your Love Story
Find section "Our Story" (around line ~410)

Current:
```html
<div class="story-text">
    Add your love story here. Share the moment you met, your favorite memories together, 
    and why you're excited to start this new chapter.
</div>
```

Change to:
```html
<div class="story-text">
    We met in college and knew we were meant to be. After 5 beautiful years together, 
    Sahil got down on one knee under the stars, and here we are! Join us as we start 
    this amazing new journey together.
</div>
```

### Update Wedding Details
Find "Wedding Details" section (around line ~435)

Current example:
```html
<div class="detail-item">
    <div class="detail-label">📅 Date</div>
    <div class="detail-value">November 11, 2028</div>
</div>
```

Update all four sections:
```html
<div class="detail-item">
    <div class="detail-label">📅 Date</div>
    <div class="detail-value">November 11, 2028</div>
</div>
<div class="detail-item">
    <div class="detail-label">🕐 Time</div>
    <div class="detail-value">6:00 PM onwards</div>
</div>
<div class="detail-item">
    <div class="detail-label">📍 Venue</div>
    <div class="detail-value">Taj Garden Palace<br>Ahmedabad, Gujarat</div>
</div>
<div class="detail-item">
    <div class="detail-label">🎭 Dress Code</div>
    <div class="detail-value">Indian Ethnic Wear</div>
</div>
```

### Add Accommodation Info
Find the accommodation section (around line ~460):

Current:
```html
<div style="margin-top: 40px; padding-top: 40px; border-top: 1px solid rgba(139, 74, 92, 0.1);">
    <h3 style="color: var(--primary-color); margin-bottom: 15px; font-weight: 300; font-size: 20px;">Accommodation</h3>
    <p style="color: #666; font-style: italic;">Add accommodation details and nearby hotels for your guests</p>
</div>
```

Change to:
```html
<div style="margin-top: 40px; padding-top: 40px; border-top: 1px solid rgba(139, 74, 92, 0.1);">
    <h3 style="color: var(--primary-color); margin-bottom: 15px; font-weight: 300; font-size: 20px;">Accommodation</h3>
    <p style="color: #666; font-style: italic;">
        <strong>Hotel Raj Palace</strong> - 5km away - ₹3000/night<br>
        <strong>Grand Heritage Inn</strong> - 3km away - ₹2500/night<br>
        Special wedding rates available. Contact us for codes!
    </p>
</div>
```

## Change Colors & Style

### Primary Colors
Find the `:root` section at the very top (line ~36):

```css
:root {
    --primary-color: #8b4a5c;      /* Main burgundy - change this */
    --secondary-color: #a85a6f;    /* Secondary accent */
    --accent-color: #b8906a;       /* Gold/brown accent */
    --light-bg: #fef9f3;           /* Light background */
    --cream-bg: #faf5f0;           /* Cream background */
    --text-light: #f5e6d3;         /* Light text color */
}
```

**Example color changes:**

For a blush pink theme:
```css
--primary-color: #c97f8a;      /* Blush pink */
--secondary-color: #d49ba7;    /* Light pink */
--accent-color: #f0a3b0;       /* Rose pink */
```

For a classic gold theme:
```css
--primary-color: #8b6f47;      /* Brown */
--secondary-color: #a8885c;    /* Tan */
--accent-color: #d4af37;       /* Gold */
```

For a royal blue theme:
```css
--primary-color: #1e3a8a;      /* Dark blue */
--secondary-color: #3b82f6;    /* Blue */
--accent-color: #fbbf24;       /* Gold */
```

## Add Multiple Photos

### Add Photo Gallery Section
Add this after the couple photo section (around line ~420):

```html
<!-- GALLERY SECTION -->
<section class="story" id="gallery">
    <div class="container">
        <div class="story-card">
            <div class="section-label">Gallery</div>
            <div class="story-title">Our Moments</div>
            
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 20px; margin: 30px 0;">
                <img src="photo1.jpg" style="width: 100%; border-radius: 12px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);" alt="Memory 1">
                <img src="photo2.jpg" style="width: 100%; border-radius: 12px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);" alt="Memory 2">
                <img src="photo3.jpg" style="width: 100%; border-radius: 12px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);" alt="Memory 3">
                <img src="photo4.jpg" style="width: 100%; border-radius: 12px; box-shadow: 0 5px 15px rgba(0,0,0,0.1);" alt="Memory 4">
            </div>
        </div>
    </div>
</section>
```

## Add Events/Ceremonies

Add this section before the RSVP section:

```html
<!-- EVENTS SECTION -->
<section class="story" id="events">
    <div class="container">
        <div class="story-card">
            <div class="section-label">Celebrations</div>
            <div class="story-title">Wedding Events</div>
            
            <div style="text-align: left; max-width: 600px; margin: 0 auto;">
                <div style="margin-bottom: 30px; padding-bottom: 20px; border-bottom: 1px solid rgba(139, 74, 92, 0.1);">
                    <h4 style="color: var(--primary-color); font-size: 20px; margin-bottom: 10px;">Mehendi</h4>
                    <p style="color: #666; margin: 5px 0;">📅 November 9, 2028</p>
                    <p style="color: #666; margin: 5px 0;">🕐 6:00 PM - 10:00 PM</p>
                    <p style="color: #666; margin: 5px 0;">📍 Venue Name</p>
                </div>
                
                <div style="margin-bottom: 30px; padding-bottom: 20px; border-bottom: 1px solid rgba(139, 74, 92, 0.1);">
                    <h4 style="color: var(--primary-color); font-size: 20px; margin-bottom: 10px;">Sangeet</h4>
                    <p style="color: #666; margin: 5px 0;">📅 November 10, 2028</p>
                    <p style="color: #666; margin: 5px 0;">🕐 7:00 PM - 11:00 PM</p>
                    <p style="color: #666; margin: 5px 0;">📍 Venue Name</p>
                </div>
                
                <div style="margin-bottom: 30px;">
                    <h4 style="color: var(--primary-color); font-size: 20px; margin-bottom: 10px;">Wedding Ceremony</h4>
                    <p style="color: #666; margin: 5px 0;">📅 November 11, 2028</p>
                    <p style="color: #666; margin: 5px 0;">🕐 6:00 PM - 10:30 PM</p>
                    <p style="color: #666; margin: 5px 0;">📍 Taj Garden Palace</p>
                </div>
            </div>
        </div>
    </div>
</section>
```

Also update the navigation menu to include the new section:
Find line ~265 and update:
```html
<ul class="nav-menu">
    <li><a href="#home">Home</a></li>
    <li><a href="#story">Our Story</a></li>
    <li><a href="#events">Events</a></li>
    <li><a href="#venue">Venue</a></li>
    <li><a href="#rsvp">RSVP</a></li>
</ul>
```

## Common Changes Summary

| What to Change | Where to Find | Replace With |
|---|---|---|
| Groom's name | Sahil | Your groom's name |
| Bride's name | Aayushi | Your bride's name |
| Wedding date | November 11, 2028 | Your date |
| Email for RSVP | sahil.aayushi@example.com | Your email |
| RSVP deadline | October 15, 2028 | Your deadline |
| Venue name | Add your venue | Your venue |
| Primary color | #8b4a5c | Your color code |

## Testing Your Changes

1. **Local Testing**
   - Open `index.html` directly in your browser
   - Test all interactive features
   - Check on mobile (use browser's mobile view - press F12)

2. **After Upload to Vercel**
   - Visit your live URL
   - Test on mobile phone
   - Share with a friend to test RSVP
   - Check countdown timer

## Need More Help?

- Use browser DevTools (F12) to inspect elements
- Copy full sections to add similar blocks
- All colors use standard hex codes (#RRGGBB)
- HTML comments start with `<!--` and end with `-->`

Good luck with your wedding! 💕
