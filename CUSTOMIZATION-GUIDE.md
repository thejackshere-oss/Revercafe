# Rever Cafe Website - Quick Customization Guide

## 🎨 Color Changes

If you want to change the brand colors, find and replace in `index.html`:

### Current Colors
```
Forest Green:  #1b3022  (Main color)
Cream:         #f4f1de  (Background)
Gold:          #d4af37  (Accent)
```

### To Change Colors
1. Open `index.html` in a text editor
2. Use Find & Replace (Ctrl+H):
   - Search: `#1b3022` Replace with: `your-new-forest-color`
   - Search: `#f4f1de` Replace with: `your-new-cream-color`
   - Search: `#d4af37` Replace with: `your-new-gold-color`

### Recommended Color Combinations

**Option 1: Deep Burgundy Theme**
- Forest: #3d1f2a (Deep Burgundy)
- Cream: #f5f1e8 (Warm Cream)
- Gold: #c9a961 (Dusty Gold)

**Option 2: Navy Theme**
- Forest: #1a3a52 (Navy)
- Cream: #f9f7f4 (Off-white)
- Gold: #e4b741 (Bright Gold)

**Option 3: Dark Charcoal Theme**
- Forest: #2c2c2c (Charcoal)
- Cream: #f5f3f0 (Ivory)
- Gold: #d4af37 (Classic Gold)

---

## 📝 Content Changes

### Business Information

**Location Address**
```html
Find: "AJC Bose Road Area, Kolkata, West Bengal"
Replace with: Your actual address
```

**Phone Number**
```html
Find: "099033 15530"
Replace with: Your phone number
```
```html
Find: "919903315530"
Replace with: Your phone number WITHOUT + (for WhatsApp)
```

**Email**
```html
Find: "hello@revercafe.com"
Replace with: Your email address
```

**Hours**
```html
Find: "Mon-Fri: 8 AM - 10 PM"
Find: "Sat-Sun: 9 AM - 11 PM"
Replace with: Your actual hours
```

### Menu Items

Find the menu section and update:

**Brew Section** (Search for "Signature Espresso")
```html
<h4 class="font-bold text-lg text-forest">ITEM_NAME</h4>
<p class="text-gray-600 text-sm mb-2">DESCRIPTION</p>
<span class="text-gold font-bold">₹PRICE</span>
```

**Bake Section** (Search for "Croissant")
Same format as above

**Bites Section** (Search for "Avocado Toast")
Same format as above

### Social Links

**Instagram**
```html
Find: "https://www.instagram.com/revercafekolkata"
Replace with: Your Instagram profile link
```

**WhatsApp**
```html
Find: "https://wa.me/919903315530"
Replace with: https://wa.me/YOUR_PHONE_NUMBER (no spaces, no +)
```

**Google Maps Review**
```html
Find: "https://maps.app.goo.gl/GhFE3Nk4djbS52WG6"
Replace with: Your Google Maps review link
```

---

## 🖼️ Image Replacements

### How to Add Your Images

1. **Prepare images** (optimize for web):
   - Interior photos: ~500x500px each
   - Food photos: ~400x400px each
   - Keep file size < 500KB

2. **Name your files clearly**:
   - Interior1.jpg, Interior2.jpg, Interior3.jpg, Interior4.jpg
   - Food1.jpg, Food2.jpg, Food3.jpg, Food4.jpg, Food5.jpg

3. **Upload to GitHub** (or your server):
   - In the same directory as index.html

4. **Update HTML paths**:
   ```html
   Find: <img src="https://via.placeholder.com/400x400?text=Interior+1"
   Replace with: <img src="Interior1.jpg"
   ```

### Quick Replace Script
For all interior images:
```
Find: https://via.placeholder.com/400x400?text=Interior+1
Replace: Interior1.jpg

Find: https://via.placeholder.com/400x400?text=Interior+2
Replace: Interior2.jpg

Find: https://via.placeholder.com/400x400?text=Interior+3
Replace: Interior3.jpg

Find: https://via.placeholder.com/400x400?text=Interior+4
Replace: Interior4.jpg
```

For all food images:
```
Find: https://via.placeholder.com/300x300?text=Coffee+1
Replace: Food1.jpg

Find: https://via.placeholder.com/300x300?text=Coffee+2
Replace: Food2.jpg

Find: https://via.placeholder.com/300x300?text=Food+1
Replace: Food3.jpg

Find: https://via.placeholder.com/300x300?text=Food+2
Replace: Food4.jpg

Find: https://via.placeholder.com/300x300?text=Food+3
Replace: Food5.jpg
```

---

## ⭐ Reviews

### Add Customer Reviews

Find the "What Our Guests Say" section and add new reviews:

```html
<div class="review-card">
    <div class="flex items-center mb-4">
        <div class="text-2xl font-bold text-forest mr-3">👤</div>
        <div>
            <p class="font-bold text-forest">CUSTOMER_NAME</p>
            <div class="rating-stars">★ ★ ★ ★ ★</div>
        </div>
    </div>
    <p class="text-gray-600">"REVIEW_TEXT"</p>
    <p class="text-sm text-gray-500 mt-3">Verified Guest • TIME_AGO</p>
</div>
```

**Example:**
```html
<div class="review-card">
    <div class="flex items-center mb-4">
        <div class="text-2xl font-bold text-forest mr-3">👤</div>
        <div>
            <p class="font-bold text-forest">John Doe</p>
            <div class="rating-stars">★ ★ ★ ★ ★</div>
        </div>
    </div>
    <p class="text-gray-600">"Amazing coffee and wonderful ambience! This is my new favorite cafe."</p>
    <p class="text-sm text-gray-500 mt-3">Verified Guest • 5 days ago</p>
</div>
```

---

## 📄 PDF Menu

### Change Menu PDF Link

Find:
```html
<a href="revercafe.menu.pdf" target="_blank"
```

Replace with your PDF file name:
```html
<a href="your-menu-file-name.pdf" target="_blank"
```

### Upload Your Menu

1. Prepare your menu PDF (or image as PDF)
2. Upload to same directory as index.html
3. Update the link above

---

## 🎯 About Section

### Update Your Story

Find the "Our Story" section:

```html
<p class="text-gray-600 mb-4 leading-relaxed">
    [YOUR STORY HERE]
</p>
```

Replace with your cafe's actual story.

### Update Values

Find the values section and customize:

```html
<div class="text-center">
    <div class="text-5xl mb-4">[EMOJI]</div>
    <h4 class="text-xl font-bold text-forest mb-3">[VALUE NAME]</h4>
    <p class="text-gray-600">[VALUE DESCRIPTION]</p>
</div>
```

---

## 🔗 Links to Update

These links should be personalized:

1. **Google Business Profile**
   ```
   https://share.google/wvRI9FFuhkXSADRqG → Your profile link
   ```

2. **Google Maps Location**
   ```
   Get from: https://maps.google.com
   Search your location
   Copy embed code
   Replace the iframe src
   ```

3. **Instagram Profile**
   ```
   Already set to: revercafekolkata
   Update if different
   ```

---

## 📱 Mobile Number for WhatsApp

### Current Setup
- Number: +91 99033 15530
- Format for links: 919903315530 (no +, no spaces)

### To Update

Find all instances of:
- `919903315530` (for links)
- `099033 15530` (for display)
- `+91 99033 15530` (for formal display)

Replace with your number in the same formats.

---

## 🔤 Typography

### Font Sizes (Tailwind CSS)

```
Headings:
- H1: text-5xl (mobile) → text-7xl (desktop)
- H2: text-3xl → text-4xl
- H3: text-2xl → text-3xl
- Body: text-base (16px)

To change:
text-5xl → text-3xl (makes heading smaller)
text-5xl → text-6xl (makes heading larger)
```

### Font Families

```
Currently using: System fonts (no external fonts)
- Sans-serif: "Segoe UI", Tahoma, etc.
- Serif: Georgia (for quotes/special text)

To use custom fonts:
1. Add Google Fonts to <head>
2. Update tailwind config
3. Use in classes
```

---

## 🎪 Hero Section Customization

### Main Headline

Find:
```html
<h1 class="text-5xl md:text-7xl font-bold mb-6 leading-tight">
    Modern Heritage<br>Meets Specialty Coffee
</h1>
```

Change to your tagline.

### Hero Subtitle

Find:
```html
<p class="text-xl md:text-2xl text-cream mb-8 max-w-2xl mx-auto">
    Experience contemporary elegance...
</p>
```

Update with your message.

### Hero Stats

Find:
```html
<div class="flex justify-center gap-6 text-gold text-sm">
    <div>⭐ 4.8/5 Rating</div>
    <div>📍 Kolkata</div>
    <div>☕ Premium Quality</div>
</div>
```

Update your stats/highlights.

---

## 🎨 Button Customization

### Button Colors

Primary Button (Gold background):
```css
.btn-primary {
    background: #d4af37;  /* Change this */
    color: #1b3022;       /* Change this */
}
```

Secondary Button (Transparent with border):
```css
.btn-secondary {
    color: #d4af37;       /* Change this */
    border: 2px solid #d4af37;  /* Change this */
}
```

### Button Text

Find buttons and change text:
```html
📅 Book a Table → Change to your CTA
📖 View Menu → Change text
```

---

## 🚀 Quick Testing Checklist

After making changes:

- [ ] Open in Chrome
- [ ] Open in Firefox
- [ ] Open on mobile phone
- [ ] Test all links
- [ ] Test WhatsApp button
- [ ] Test booking form
- [ ] Check image loading
- [ ] Verify menu prices
- [ ] Check contact info

---

## 💾 File Backup

**Before making changes:**
1. Download original index.html
2. Save as backup: `index.html.backup`
3. Keep in safe location
4. Edit the working copy

**In Git:**
```bash
git checkout index.html  # Revert to last saved version
git diff index.html     # See all changes
```

---

## 🔍 Finding Code Sections

Use Ctrl+F (Cmd+F on Mac) to find:

| What | Search for |
|------|-----------|
| Hero Section | "Modern Heritage" |
| Menu Section | "Our Menu" |
| About Section | "Our Story" |
| Gallery Section | "Our Vibe" |
| Contact Section | "Get In Touch" |
| Reviews | "What Our Guests Say" |
| Hours | "Mon-Fri: 8 AM" |
| Phone | "099033 15530" |
| Instagram | "revercafekolkata" |
| WhatsApp | "919903315530" |

---

## 🆘 If Something Breaks

1. **Check browser console** (F12)
2. **Verify all tags are closed** properly
3. **Check for syntax errors**
4. **Restore from backup**
5. **Clear browser cache** (Ctrl+Shift+Delete)
6. **Try different browser**

---

## 📞 Common Support

**For issues with**:
- **GitHub Pages**: https://github.com/support
- **HTML/CSS**: https://www.w3schools.com
- **Tailwind CSS**: https://tailwindcss.com/docs
- **Images**: Use optimized JPG/PNG files
- **Forms**: Test with actual phone/email

---

**Quick Tip**: Keep your original index.html safe. Always test changes in a backup copy first before uploading to your live website.

**Last Updated**: May 2024
