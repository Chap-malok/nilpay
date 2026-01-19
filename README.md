# NilPay Landing Page

A modern, responsive landing page for NilPay - a unified payment wallet for South Sudan.

## Features

✅ **Fully Responsive** - Works on mobile, tablet, and desktop
✅ **SEO Optimized** - Meta tags, Open Graph, Twitter Card support
✅ **Smooth Interactions** - Smooth scrolling, hover effects, form validation
✅ **Accessible** - ARIA labels, semantic HTML, keyboard navigation
✅ **Form Storage** - Email waitlist saves locally with LocalStorage
✅ **Performance Optimized** - Lazy loading images, minimal CSS
✅ **Modern Design** - Clean gradient hero, feature cards, smooth animations

## Files

- `index.html` - Main HTML structure with improved SEO and accessibility
- `styles.css` - Comprehensive styling with responsive design (mobile-first)
- `assets/nilpay-logo.jpeg` - Logo image

## Improvements Made

1. **HTML Enhancements**
   - Added meta tags for SEO and social sharing
   - Added form validation and success messages
   - Improved accessibility with ARIA labels
   - Added smooth scrolling behavior
   - LocalStorage integration for waitlist emails

2. **CSS Improvements**
   - Responsive grid layouts with `clamp()` for fluid typography
   - Mobile-first approach with breakpoints at 768px and 480px
   - Smooth transitions and hover effects
   - Sticky navigation
   - Better spacing and typography
   - Optimized buttons and form elements

3. **JavaScript Features**
   - Smooth scroll navigation
   - Email validation
   - Form submission handling with feedback
   - LocalStorage for persistent email storage

## How to Use Locally

1. Open `index.html` in any modern web browser
2. Test the form - emails are stored in your browser's local storage
3. All links are fully functional with smooth scrolling

## Deployment Options

### Option 1: Netlify (Recommended - Free & Easy)
1. Go to [netlify.com](https://netlify.com)
2. Sign up with GitHub or email
3. Create a new project and connect your repository OR drag and drop the `NilPay` folder
4. Deploy! Your site will be live instantly

### Option 2: Vercel (Free & Fast)
1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub or email
3. Import the project or drag and drop the folder
4. Click Deploy
5. Get a live URL immediately

### Option 3: GitHub Pages (Free)
1. Create a GitHub repository
2. Upload your files
3. Go to Settings → Pages
4. Select `main` branch as source
5. Your site is live at `yourusername.github.io/nilpay`

### Option 4: Traditional Web Host (Bluehost, GoDaddy, etc.)
1. Upload files via FTP
2. Ensure `index.html` is in the root directory
3. Access via your domain

## Browser Support

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile browsers: ✅ Fully responsive

## Performance Tips

- Images are lazy-loaded
- CSS is minified and optimized
- No external dependencies
- Fast load time

## Customization

- Update colors in `styles.css` `:root` variables
- Modify content directly in `index.html`
- Change the logo in `assets/` folder
- Update social media links in meta tags

## Analytics & Tracking

To add Google Analytics:
```html
<!-- Add to <head> in index.html -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR_GA_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR_GA_ID');
</script>
```

## Next Steps

1. Test the form by entering your email
2. Check browser console for any errors (F12)
3. Test on mobile devices
4. Deploy to Netlify or Vercel
5. Set up a backend service to handle emails (Firebase, Mailchimp, etc.)

## License

© 2026 NilPay. All rights reserved.
