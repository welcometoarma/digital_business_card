# 🌊 Mondello Beach Vitamin Sea — Digital Business Card

A stunning, mobile-first digital business card for the **Mondello Beach Vitamin Sea** Airbnb property in Mondello, Sicily. This single-page application combines a beautiful beach-themed design with practical functionality, allowing guests to view property details, save contact information, and share the property with friends.

[Property logo](https://logo.jpg)

## 📱 Live Demo

[View Live Demo](https://welcometoarma.github.io/digital_business_card/)

## ✨ Features

### 🎨 Design & Theme

- **Sky, Sea & Beach Theme:** Gradient background transitioning from deep ocean blue to golden sandy shores.
- **Animated Elements:** Pulsing sun, drifting clouds, and gentle wave animations.
- **Glass-morphism Effect:** Frosted glass card design with backdrop blur for a modern aesthetic.
- **Fully Responsive:** Optimized for all screen sizes, from desktop to mobile devices.

### 📋 Property Showcase

- **Key Amenities:** 2 beds, 1 bath, and kitchen.
- **Host Information:** “Superhost” badge with host name.
- **Photo Slideshow:** Six property images with automatic rotation every 3.5 seconds.
- **Manual Controls:** Click dots to navigate and tap images for fullscreen viewing.

### 🔗 Quick Actions

- **Book Now:** Direct link to the Airbnb listing.
- **Add Contact:** One-tap saving to phone contacts using vCard format.
  - **Android:** Opens directly in the Contacts app.
  - **iOS:** Downloads a `.vcf` file for easy import.
  - **Desktop:** Downloads a `.vcf` file.

## 📞 Contact Methods

| Method | Details |
|---|---|
| WhatsApp | [+39 389 559 2579](https://wa.me/393895592579), opens the WhatsApp app |
| Email | [katkaockovicova@yahoo.co.uk](mailto:katkaockovicova@yahoo.co.uk), opens the default mail client |
| Instagram | [@mondello_beach_vitamin_sea](https://instagram.com/mondello_beach_vitamin_sea), opens the profile |

## 📍 Location & Reviews

- **Google Maps:** Direct link with the property address.
- **Address:** Via Carbone, 73 · 90151 Palermo PA.
- **Guest Reviews:** 5.0 rating with a “Guest favorite” badge.
- **Airbnb Reviews:** Direct link to all reviews.

## 📤 Share Options

- WhatsApp share.
- Telegram share.
- Twitter/X share.
- Copy URL to the clipboard.

## 🔙 Smart Navigation

- **Persistent “Back to Main” Button:** Always visible so users can return to the card.
- **External Links:** Open in a new tab to preserve the card page.
- **Universal Link Prevention:** Helps prevent iOS and Android from hijacking the current tab.
- **History Support:** Smart back navigation when browser history is available.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Semantic markup structure |
| CSS3 | Custom properties, animations, flexbox, and grid |
| Vanilla JavaScript | Slideshow, contact saving, and clipboard operations |
| Google Fonts | Fraunces serif and Manrope sans-serif fonts |
| SVG Icons | Custom scalable vector icons |
| Progressive Web App features | Mobile-friendly meta tags and theme-color support |

## 📁 File Structure

```text
digital_business_card/
├── index.html          # Main application file
├── logo.jpg            # Property logo image
├── salon.jpg           # Living room photo
├── kitchen.jpg         # Kitchen photo
├── bagno.jpg           # Bathroom photo
├── balcony.jpg         # Balcony photo
├── bed1.jpg            # Bedroom 1 photo
├── bed2.jpg            # Bedroom 2 photo
├── manifest.json       # PWA manifest (optional)
└── README.md           # This file
```

## 🎨 Color Palette

| Color | Name | Usage |
|---|---|---|
| `#0B4F6C` | Deep Ocean | Primary text and sky-top gradient |
| `#1A8F9E` | Ocean Mid | Sky gradient and accent color |
| `#6BC2D0` | Sky Blue | Sky-bottom gradient |
| `#F5E6D3` | Sand | Background gradient and warmth |
| `#FDF5E6` | Sand Light | Background gradient end |
| `#FFD93D` | Sun Yellow | Highlights and button gradients |
| `#FFB347` | Sunset Orange | Gradients and active states |
| `#E07A5F` | Terracotta | Secondary accents |

## 📱 Mobile Optimization

| Feature | Implementation |
|---|---|
| Full height | Uses `100dvh` for the dynamic viewport height |
| Touch-friendly controls | Larger touch targets and smooth scrolling |
| iOS Safari | `viewport-fit=cover` for notch support |
| Android Chrome | `theme-color` meta tag support |
| Home screen | Apple touch icon support |
| Status bar | `black-translucent` for an immersive feel |

## 🔧 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/welcometoarma/digital_business_card.git
cd digital_business_card
```

### 2. Replace placeholder images

- Update `logo.jpg` with the property logo.
- Replace the property photo files with your own photos, keeping the existing filenames or updating the HTML references.

### 3. Update content

Modify the following values in `index.html`:

```html
<!-- Phone number -->
<a href="https://wa.me/YOUR_PHONE_NUMBER">

<!-- Email -->
<a href="mailto:YOUR_EMAIL">

<!-- Instagram -->
<a href="https://instagram.com/YOUR_USERNAME">

<!-- Airbnb URL -->
<a href="https://airbnb.com/h/YOUR_LISTING">

<!-- Google Maps address -->
<a href="https://www.google.com/maps?q=YOUR_ADDRESS">
```

### 4. Deploy to GitHub Pages

```bash
git add .
git commit -m "Update business card content"
git push origin main
```

### 5. Enable GitHub Pages

1. Open **Settings → Pages**.
2. Select the `main` branch and the `/ (root)` directory.
3. Click **Save**.
4. Wait approximately 1–2 minutes for deployment.

## 📦 Customization Guide

### Changing Colors

Edit the CSS custom properties in the `:root` selector:

```css
:root {
  --sky-top: #0B4F6C;
  --sky-mid: #1A8F9E;
  --sky-bottom: #6BC2D0;
  --sand: #F5E6D3;
  --sand-light: #FDF5E6;
  --sun: #FFD93D;
  --sun-glow: #FFB347;
  --terracotta: #E07A5F;
  --terracotta-lt: #F4A261;
}
```

### Updating Contact Information

| Field | Value |
|---|---|
| Phone | `393895592579` |
| Email | [katkaockovicova@yahoo.co.uk](mailto:katkaockovicova@yahoo.co.uk) |
| Instagram | `mondello_beach_vitamin_sea` |
| Address | `Via Carbone, 73 · 90151 Palermo PA` |
| Airbnb URL | `mondellobeachvitaminsea` |

### Modifying Images

Replace image files in the project root and update the image tags in the slideshow section:

```html
<img src="your-photo.jpg" alt="Description" />
```

Recommended image specifications:

- **Logo:** 512 × 512 pixels, square.
- **Property photos:** 800 × 600 pixels, landscape.
- **Format:** JPG or WebP.
- **File size:** Under 200 KB per image for faster loading.

### Adding More Photos

Add new image files to the root directory and include additional `<img>` tags inside the hero container:

```html
<div class="hero-image" id="heroContainer">
  <img src="photo1.jpg" alt="Description" class="active" />
  <img src="photo2.jpg" alt="Description" />
  <img src="photo3.jpg" alt="Description" />
  <!-- Add more photos here -->
</div>
```

The slideshow automatically detects and includes new images.

## 🌐 Browser Support

| Browser | Support |
|---|---|
| Chrome | ✅ Full support on desktop and mobile |
| Safari | ✅ Full support on iOS and macOS |
| Firefox | ✅ Full support |
| Edge | ✅ Full support |
| Samsung Internet | ✅ Full support |
| Opera | ✅ Full support |

## 📝 SEO & Metadata

The page includes comprehensive meta tags for improved search visibility:

```html
<!-- Basic metadata -->
<title>Mondello Beach Vitamin Sea — Digital Card</title>
<meta name="description" content="Digital business card for Mondello Beach Vitamin Sea Airbnb property" />

<!-- Social media metadata -->
<meta property="og:title" content="Mondello Beach Vitamin Sea" />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://welcometoarma.github.io/digital_business_card/" />

<!-- Mobile metadata -->
<meta name="apple-mobile-web-app-capable" content="yes" />
<meta name="apple-mobile-web-app-status-bar-style" content="black-translucent" />
<meta name="apple-mobile-web-app-title" content="Mondello Beach Vitamin Sea" />
```

## 📋 Changelog

### v2.0 — Current

- ✨ Redesigned sky, sea, and beach theme.
- ✨ Animated sun, clouds, and waves.
- ✨ Glass-morphism card design.
- ✨ Persistent “Back to Main” button.
- ✨ Improved universal-link handling.
- ✨ Android Contacts integration.
- 📱 Enhanced mobile responsiveness.
- 🎨 New color palette.

### v1.0 — Initial Release

- Basic business card layout.
- Contact buttons for WhatsApp, email, and Instagram.
- Photo slideshow.
- vCard download support.

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/AmazingFeature
   ```

3. Commit your changes:

   ```bash
   git commit -m 'Add some AmazingFeature'
   ```

4. Push the branch:

   ```bash
   git push origin feature/AmazingFeature
   ```

5. Open a pull request.

### Guidelines

- Follow the existing code style.
- Test on mobile and desktop devices.
- Update the README when necessary.
- Keep changes focused and well documented.

## 🐛 Known Issues & Solutions

| Issue | Solution |
|---|---|
| vCard does not open directly on iOS | The `.vcf` file downloads; tap it to import the contact into Contacts. |
| Photos do not load | Check that filenames match the references in the HTML. |
| Google Maps does not open | Update the address in the `href` attribute. |
| Instagram link does not work | Verify that the Instagram username is correct. |
| Back button does not work | Ensure that `MAIN_URL` is correct in the JavaScript. |

## 📧 Contact & Support

- **Property:** [Airbnb listing](https://airbnb.com/h/mondellobeachvitaminsea)
- **Host:** Katie
- **Email:** [katkaockovicova@yahoo.co.uk](mailto:katkaockovicova@yahoo.co.uk)
- **WhatsApp:** [+39 389 559 2579](https://wa.me/393895592579)
- **Instagram:** [@mondello_beach_vitamin_sea](https://instagram.com/mondello_beach_vitamin_sea)

## 📄 License

This project is open source and available under the MIT License.

Copyright (c) 2024 Mondello Beach Vitamin Sea

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## 🙏 Acknowledgments

- **Fonts:** Google Fonts — Fraunces and Manrope.
- **Icons:** Material Design icons.
- **Design inspiration:** Beach and coastal aesthetics.
- **Testing:** Community feedback.

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐ on GitHub.

Made with ❤️ for Mondello Beach Vitamin Sea.

> Where the sun meets the sea 🌅🏖️
