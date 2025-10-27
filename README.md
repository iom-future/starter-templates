# Frontend Starter Template 🚀

A production-ready HTML/CSS starter template with comprehensive CSS variables, reset and SEO-optimized meta tags. This template provides developers with a solid foundation to build modern, accessible, and search-engine-friendly websites.

## 📋 Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [CSS Reset Documentation](#css-reset-documentation)
- [HTML Template Setup](#html-template-setup)
- [SEO Meta Tags Configuration](#seo-meta-tags-configuration)
- [Customization Guide](#customization-guide)
- [Best Practices](#best-practices)
- [Browser Support](#browser-support)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features

### CSS Reset
- ✅ Comprehensive cross-browser reset
- ✅ Modern box-sizing and spacing normalization
- ✅ Responsive media elements by default
- ✅ Accessibility-first approach
- ✅ Motion preference support
- ✅ Mobile-optimized form inputs

### CSS Variables System

- ✅ Complete color system (primary, secondary, semantic colors)
- ✅ 6-shade color scales for both primary and secondary brands
- ✅ Pre-built gradients and shadow colors
- ✅ 8px-based spacing system with 13 sizes
- ✅ Responsive typography with mobile/tablet/desktop scales
- ✅ Component-specific variables (buttons, cards, sections)
- ✅ Organized z-index layers for UI components
- ✅ Transition timing system for animations

### HTML Template
- ✅ SEO-optimized meta tags
- ✅ Open Graph tags for social sharing
- ✅ Twitter Card integration
- ✅ Structured data (JSON-LD) ready
- ✅ Complete favicon and app icon setup
- ✅ Performance optimization with preloading
- ✅ Semantic HTML5 structure

---

## 🚀 Quick Start

### 1. Clone or Download
```bash
git clone https://github.com/iom-future/starter-template.git your-project
cd your-project
```

### 2. Configure HTML Template
Update the placeholder values in `index.html` with your actual content (see [HTML Template Setup](/html/index.html)).

### 3. Start Development
Open `index.html` in your browser or use a local development server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js with npx
npx serve

# Using VS Code Live Server extension
# Right-click index.html > Open with Live Server
```

---

## 📁 Project Structure

```
starter-template/
|
├── animation/
│   └── gsap/ 
|                      
│
├── css/
│   ├── style.css          # contains CSS reset and variables
│  
├── html/
│   └── index.js  # Main HTML boilerplate with SEO tags     
|
├── icons/           # app icons
│    |── icons-dependencies/     
│    └── icon-css/
|
├── js/
│   └── main.js            # Your JavaScript code
|
└── README.md # This documentation file        
```

---

## 🎨 CSS Reset Documentation

### What It Does

The CSS reset provides a consistent baseline across all browsers by:

1. **Box Sizing Reset** - Makes width/height calculations predictable
2. **Spacing Normalization** - Removes default margins and padding
3. **Typography Enhancement** - Improves text rendering and readability
4. **Responsive Media** - Makes images and videos responsive by default
5. **Form Element Reset** - Removes browser-specific form styling
6. **Accessibility Features** - Includes screen reader utilities and motion preferences

### Key Features Explained

#### 1. Screen Reader Only Utility
```css
.sr-only {
  /* Hides content visually but keeps it accessible to screen readers */
}
```

**Usage:**
```html
<a href="#main-content" class="sr-only">Skip to main content</a>
```

#### 2. Motion Preferences
Automatically respects user's motion preferences set in their operating system.

#### 3. Mobile Input Zoom Prevention
Prevents iOS from zooming in on form inputs by setting minimum font size to 16px on mobile.

#### 4. Focus Visible Support
Modern focus indicators that only show when navigating with keyboard, not mouse clicks.

---

## 📄 HTML Template Setup

### Required Replacements

Below is a complete checklist of all placeholder values that **MUST** be replaced with your actual content:

#### 1. Basic Meta Tags

| Tag | Placeholder | Replace With | Example |
|-----|-------------|--------------|---------|
| `<title>` | Your Page Title \| Your Brand Name | Your actual page title | About Us \| Acme Corp |
| `name="description"` | A compelling description... | Your page description (150-160 chars) | Learn about Acme Corp's mission to... |
| `name="keywords"` | keyword1, keyword2... | Your relevant keywords | web development, design, templates |
| `name="author"` | Your Name or Company Name | Your actual name/company | John Doe / Acme Corporation |
| `rel="canonical"` | https://www.yourwebsite.com/page-url | Your actual page URL | https://www.acmecorp.com/about |

#### 2. Open Graph Tags (Facebook/LinkedIn)

| Tag | Placeholder | Replace With | Recommended Size |
|-----|-------------|--------------|------------------|
| `og:title` | Your Page Title \| Your Brand Name | Same as page title | 60-90 characters |
| `og:description` | A compelling description... | Social media description | Up to 300 characters |
| `og:image` | https://www.yourwebsite.com/images/og-image.jpg | Your actual image URL | 1200x630px |
| `og:image:alt` | Description of the image | Actual image description | Acme Corp office building |
| `og:url` | https://www.yourwebsite.com/page-url | Your actual page URL | https://www.acmecorp.com/about |
| `og:site_name` | Your Website Name | Your site name | Acme Corporation |

#### 3. Twitter Card Tags

| Tag | Placeholder | Replace With | Recommended Size |
|-----|-------------|--------------|------------------|
| `twitter:site` | @yourtwitterhandle | Your Twitter handle | @acmecorp |
| `twitter:creator` | @yourtwitterhandle | Content creator handle | @johndoe |
| `twitter:title` | Your Page Title \| Your Brand Name | Same as page title | 70 characters max |
| `twitter:description` | A compelling description... | Twitter description | Up to 200 characters |
| `twitter:image` | https://www.yourwebsite.com/images/twitter-image.jpg | Your actual image URL | 1200x675px |
| `twitter:image:alt` | Description of the image | Actual image description | Acme Corp team photo |

#### 4. Favicon and Icon Files

| File | Purpose | Size | Required? |
|------|---------|------|-----------|
| `favicon.ico` | Browser tab icon | 16x16, 32x32 | Yes |
| `favicon-16x16.png` | Small favicon | 16x16px | Recommended |
| `favicon-32x32.png` | Standard favicon | 32x32px | Recommended |
| `apple-touch-icon.png` | iOS home screen | 180x180px | Recommended |
| `android-chrome-192x192.png` | Android icon | 192x192px | Recommended |
| `android-chrome-512x512.png` | Android splash screen | 512x512px | Recommended |


#### 5. Structured Data (JSON-LD)

```json
{
  "@context": "https://schema.org",  // ← DO NOT CHANGE
  "@type": "WebPage",                 // ← Change based on page type
  "name": "Your Page Title",          // ← Replace with actual title
  "description": "Your page description", // ← Replace with description
  "url": "https://www.yourwebsite.com/page-url", // ← Your page URL
  "publisher": {
    "@type": "Organization",           // ← Or "Person" for personal sites
    "name": "Your Company Name",       // ← Your actual company name
    "logo": {
      "@type": "ImageObject",
      "url": "https://www.yourwebsite.com/images/logo.png" // ← Your logo URL
    }
  }
}
```

**Common `@type` values:**
- `WebPage` - Generic web page
- `Article` - Blog posts, news articles
- `Product` - Product pages
- `LocalBusiness` - Business listings
- `Organization` - Company/organization pages
- `Person` - Personal profiles
- `FAQPage` - FAQ pages
- `Recipe` - Recipe pages

#### 6. Stylesheet and Font Links

| Tag | Placeholder | Replace With |
|-----|-------------|--------------|
| `href="/css/styles.css"` | /css/styles.css | Your actual CSS path |
| `href="/fonts/main-font.woff2"` | /fonts/main-font.woff2 | Your font file path |
| Google Fonts link | Inter font example | Your chosen font |

---

## 🔧 SEO Meta Tags Configuration

### Title Tag Best Practices

```html
<title>Primary Keyword | Secondary Keyword | Brand Name</title>
```

- **Optimal Length:** 50-60 characters
- **Include Keywords:** Place most important keywords first
- **Unique Per Page:** Every page should have a unique title
- **Branding:** Include brand name at the end

**Examples:**
```html
<!-- Good -->
<title>Web Development Services | Custom Solutions | Acme Corp</title>

<!-- Too Long -->
<title>The Best Web Development Services for Small and Medium Businesses in New York | Acme Corp</title>

<!-- Too Short -->
<title>Services</title>
```

### Meta Description Best Practices

```html
<meta name="description" content="Concise, compelling description that includes primary keywords and encourages clicks.">
```

- **Optimal Length:** 150-160 characters
- **Include CTA:** Encourage users to click
- **Unique Per Page:** Different description for each page
- **Natural Language:** Write for humans, not just search engines

**Examples:**
```html
<!-- Good -->
<meta name="description" content="Get custom web development solutions tailored to your business needs. Fast, responsive, and SEO-friendly websites. Free consultation available.">

<!-- Too Short -->
<meta name="description" content="Web development services.">

<!-- Keyword Stuffing (Bad) -->
<meta name="description" content="Web development web design web dev websites website design custom websites web developers website development">
```

### Robots Meta Tag Options

```html
<!-- Allow indexing and following links (default) -->
<meta name="robots" content="index, follow">

<!-- Don't index this page but follow links -->
<meta name="robots" content="noindex, follow">

<!-- Index page but don't follow links -->
<meta name="robots" content="index, nofollow">

<!-- Don't index or follow links -->
<meta name="robots" content="noindex, nofollow">
```

**When to use each:**
- `index, follow` - Most pages (default)
- `noindex, follow` - Thank you pages, internal search results
- `index, nofollow` - Pages with untrusted user content
- `noindex, nofollow` - Login pages, admin pages

### Canonical URL

```html
<link rel="canonical" href="https://www.yoursite.com/page-url">
```

**Purpose:** Prevents duplicate content issues

**When to use:**
- Always specify the preferred version of a page
- Use for pages accessible via multiple URLs
- Include HTTPS and www (or non-www) as preferred
- Use absolute URLs, not relative

---

## 🎯 Customization Guide

### Adding Custom CSS Variables

Edit your CSS variables(especially colors) or add new once, in `style.css` to fit your project needs:

```css
:root {
  /* Colors */
  --color-primary: #3b82f6;
  --color-secondary: #8b5cf6;
  --color-accent: #f59e0b;
  --color-text: #1f2937;
  --color-background: #ffffff;
  
  /* Typography */
  --font-primary: 'Inter', sans-serif;
  --font-secondary: 'Merriweather', serif;
  
  /* Spacing */
  --space-xs: 0.25rem;
  --space-sm: 0.5rem;
  --space-md: 1rem;
  --space-lg: 2rem;
  --space-xl: 4rem;
  
  /* Border Radius */
  --radius-sm: 0.25rem;
  --radius-md: 0.5rem;
  --radius-lg: 1rem;
  
  /* Shadows */
  --shadow-sm: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  --shadow-md: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  --shadow-lg: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}
```

### Creating a Web App Manifest

Create a `site.webmanifest` file:

```json
{
  "name": "Your App Name",
  "short_name": "App",
  "description": "Your app description",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#ffffff",
  "theme_color": "#3b82f6",
  "icons": [
    {
      "src": "/android-chrome-192x192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "/android-chrome-512x512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
```

### Generating Favicons

Use online tools to generate all required favicon sizes:

**Recommended Tools:**
- [Favicon.io](https://favicon.io/) - Free favicon generator
- [RealFaviconGenerator](https://realfavicongenerator.net/) - Comprehensive favicon generator

**Upload a single high-resolution image (at least 512x512px) and download all sizes.**

### Adding Google Analytics

Add before the closing `</head>` tag:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your actual Google Analytics ID.

---

## 📚 Best Practices

### Performance

1. **Optimize Images**
   - Use modern formats (WebP, AVIF)
   - Compress images (TinyPNG, ImageOptim)
   - Use appropriate sizes for different devices
   - Implement lazy loading for below-fold images

2. **Minify Assets**
   - Minify CSS and JavaScript for production
   - Use tools like cssnano or Terser

3. **Reduce HTTP Requests**
   - Combine CSS files
   - Use CSS sprites for small icons
   - Implement font subsetting

### Accessibility

1. **Use Semantic HTML**
   ```html
   <header>, <nav>, <main>, <article>, <section>, <aside>, <footer>
   ```

2. **Add Alt Text to Images**
   ```html
   <img src="photo.jpg" alt="Descriptive text about the image">
   ```

3. **Ensure Keyboard Navigation**
   - All interactive elements must be keyboard accessible
   - Test navigation using only Tab and Enter keys

4. **Use ARIA Labels When Needed**
   ```html
   <button aria-label="Close menu">×</button>
   ```

### SEO

1. **One H1 Per Page**
   - Use only one `<h1>` tag per page
   - Make it descriptive and include primary keyword

2. **Logical Heading Hierarchy**
   ```html
   <h1>Main Title</h1>
     <h2>Section Title</h2>
       <h3>Subsection Title</h3>
   ```

3. **Internal Linking**
   - Link to related pages on your site
   - Use descriptive anchor text

4. **Mobile-First Design**
   - Test on real mobile devices
   - Ensure touch targets are at least 44x44px

---

## 🌐 Browser Support

This template supports all modern browsers:

- ✅ Chrome (last 2 versions)
- ✅ Firefox (last 2 versions)
- ✅ Safari (last 2 versions)
- ✅ Edge (last 2 versions)
- ✅ iOS Safari (last 2 versions)
- ✅ Chrome Android (last 2 versions)

**Note:** Internet Explorer is not supported.

---

## 📖 Additional Resources

### CSS Reset
- [Normalize.css](https://necolas.github.io/normalize.css/)
- [Modern CSS Reset](https://piccalil.li/blog/a-modern-css-reset/)

### SEO
- [Google Search Central](https://developers.google.com/search)
- [Moz Beginner's Guide to SEO](https://moz.com/beginners-guide-to-seo)
- [Schema.org Documentation](https://schema.org/)

### Accessibility
- [WCAG Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
- [WebAIM](https://webaim.org/)
- [A11y Project](https://www.a11yproject.com/)

### Tools
- [Google PageSpeed Insights](https://pagespeed.web.dev/)
- [WAVE Accessibility Tool](https://wave.webaim.org/)
- [Open Graph Debugger](https://www.opengraph.xyz/)
- [Twitter Card Validator](https://cards-dev.twitter.com/validator)

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Test thoroughly
5. Commit your changes (`git commit -m 'Add some improvement'`)
6. Push to the branch (`git push origin feature/improvement`)
7. Open a Pull Request

### Guidelines

- Follow existing code style
- Add comments for complex logic
- Update documentation for new features
- Test across multiple browsers

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Inspired by modern web development best practices
- CSS Reset inspired by Andy Bell's Modern CSS Reset
- SEO guidelines from Google Search Central
- Accessibility guidelines from WCAG and WebAIM

---

## 📝 Changelog

### Version 1.0.0 (2025-10-25)
- Initial release
- Complete CSS reset and variables
- SEO-optimized HTML template
- Comprehensive documentation

---

**Made with ❤️ for developers by developers**

⭐ Star this repository if you find it helpful!