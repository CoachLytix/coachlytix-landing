# CoachLytics - Early Access Landing Page

A single-page static website built to capture early access sign-ups for the CoachLytics golf coaching platform.

## 🎯 Purpose

This landing page validates early interest for the upcoming CoachLytics platform. Visitors can quickly understand what CoachLytics does and join the early-access waitlist by submitting their name and email address.

## 🚀 Quick Start

1. **Clone or download** this repository
2. **Replace the Formspree endpoint** in `index.html` with your own:
   - Sign up at [Formspree.io](https://formspree.io)
   - Create a new form and get your endpoint URL
   - Replace `YOUR_FORM_ID` in the form action
3. **Deploy to GitHub Pages** (see deployment instructions below)

## 🛠️ Tech Stack

- **HTML5** - Semantic markup
- **TailwindCSS** - Utility-first CSS framework (via CDN)
- **Vanilla JavaScript** - Minimal JS for smooth scrolling and theme toggle
- **Formspree** - Form handling service
- **GitHub Pages** - Static hosting

## 📁 Project Structure

```
/
├── index.html          # Main landing page
├── README.md          # This file
└── assets/            # Optional assets folder
    ├── icons/         # Custom icons (if needed)
    └── styles.css     # Additional custom styles (if needed)
```

## 🎨 Features

- **Responsive Design** - Mobile-first approach
- **CSS Variables** - Flexible theming system with light/dark mode support
- **Modern UI** - Clean, professional design with golf-themed green color palette
- **SEO Optimized** - Complete meta tags and Open Graph support
- **Fast Loading** - Optimized for GitHub Pages static hosting
- **Form Integration** - Ready-to-use Formspree integration

## 🌐 Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Create a new repository on GitHub (e.g., `coachlytics-landing`)
2. Upload your files to the repository

### Step 2: Enable GitHub Pages

1. Go to your repository **Settings**
2. Scroll down to **Pages** section
3. Under **Source**, select:
   - **Deploy from a branch**: `main` (or `master`)
   - **Folder**: `/ (root)`
4. Click **Save**

### Step 3: Access Your Site

Your site will be available at:
```
https://yourusername.github.io/coachlytics-landing/
```

### Step 4: Custom Domain (Optional)

1. Purchase a domain (e.g., `coachlytics.com`)
2. In GitHub Pages settings, add your custom domain
3. Update your DNS with a CNAME record pointing to `yourusername.github.io`
4. Wait for DNS propagation (up to 24 hours)

## 📧 Formspree Setup

### Step 1: Create Account
1. Visit [Formspree.io](https://formspree.io)
2. Sign up for a free account
3. Verify your email address

### Step 2: Create Form
1. Click "New Form"
2. Choose "Email" as the form type
3. Copy your form endpoint URL (e.g., `https://formspree.io/f/mabcdxyz`)

### Step 3: Update HTML
Replace `YOUR_FORM_ID` in `index.html` with your actual form ID:
```html
<form action="https://formspree.io/f/YOUR_ACTUAL_FORM_ID" method="POST">
```

### Step 4: Verify Domain
1. Add your domain to Formspree
2. Verify ownership when prompted
3. Test the form submission

## 🎨 Customization

### Colors
The site uses CSS variables for easy theming. Modify the `:root` section in `index.html`:

```css
:root {
    --color-bg: #f9fafb;
    --color-text: #111827;
    --color-subtext: #4b5563;
    --color-primary: #16a34a;        /* Main green */
    --color-primary-hover: #15803d;  /* Darker green */
    --color-accent-bg: #dcfce7;      /* Light green background */
}
```

### Content
Update the following sections in `index.html`:
- Hero headline and subheadline
- Problem section text
- Feature descriptions
- Footer contact information

### Dark Mode
The site includes dark mode support. Users can toggle themes, and the preference is saved in localStorage.

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Development

### Local Development
1. Open `index.html` in your browser
2. Use a local server for testing forms:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (if you have http-server installed)
   npx http-server
   ```

### Testing
- Test form submissions with your Formspree endpoint
- Verify responsive design on different screen sizes
- Check SEO meta tags with browser dev tools
- Test dark mode toggle functionality

## 📊 Analytics (Optional)

To add Google Analytics:
1. Get your GA4 measurement ID
2. Add the tracking code before `</head>` in `index.html`:
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

## 🆘 Troubleshooting

### Form Not Working
- Check Formspree endpoint URL
- Verify domain is added to Formspree
- Check browser console for errors
- Ensure form fields have `name` attributes

### GitHub Pages Not Updating
- Check repository settings for Pages configuration
- Verify files are in the correct branch
- Wait 5-10 minutes for changes to propagate
- Check for any build errors in repository Actions

### Styling Issues
- Clear browser cache
- Check TailwindCSS CDN is loading
- Verify CSS variables are properly defined
- Test in different browsers

## 📄 License

This project is created for CoachLytics. All rights reserved.

## 📞 Support

For questions or issues:
- Email: hello@coachlytics.com
- GitHub Issues: Create an issue in this repository

---

**Built with ❤️ for golf coaches**
