# Modern Portfolio Website

A beautiful, responsive personal resume and portfolio website built with HTML, CSS, and JavaScript. Perfect for showcasing your work and connecting with potential clients or employers.

## 📋 Features

- **Responsive Design**: Fully optimized for mobile, tablet, and desktop displays
- **Modern Aesthetics**: Clean, minimal design with professional color scheme (white, blue, red)
- **Smooth Animations**: Fade-in effects and hover animations for engaging interactions
- **Dark Mode**: Built-in dark mode toggle with local storage persistence
- **Sticky Navigation**: Smooth scrolling with active link highlighting
- **Mobile Menu**: Hamburger menu for mobile devices
- **Contact Form**: Functional contact form with validation
- **Social Media Links**: Easy-to-update social media integration
- **Performance Optimized**: Lightweight and fast-loading
- **Accessibility**: Semantic HTML and keyboard navigation support

## 🎨 Color Scheme

- **Primary**: Blue (#0066ff) - Used for links, buttons, and highlights
- **Secondary**: Red (#ff0033) - Used for accents and hover effects
- **Background**: White (#ffffff) - Clean, professional background
- **Dark Mode**: Automatically adapts text and backgrounds for dark mode

## 📁 File Structure

```
portfolio/
├── index.html        # Main HTML file with all sections
├── styles.css        # Complete CSS styling and layouts
├── script.js         # JavaScript for interactivity
└── README.md         # This documentation file
```

## 🚀 Quick Start

### 1. **Download and Open**

- Extract the files to a folder on your computer
- Open `index.html` in your web browser
- No installation or server setup required!

### 2. **Customize Your Information**

Open `index.html` in a text editor and update:

**Hero Section:**

```html
<h1 class="hero-title">Your Name</h1>
<p class="hero-subtitle">Your Title/Profession</p>
<p class="hero-description">Your short introduction...</p>
```

**Profile Picture:**

```html
<img src="https://via.placeholder.com/250" alt="Profile Picture" />
```

Replace with your image URL

**Certificates Section:**

- Edit certificate titles, descriptions, and years
- Update certificate images

**Projects Section:**

- Add your project information
- Update project images and links
- Modify technologies/tags

**Contact Information:**

```html
<a href="mailto:john@example.com">john@example.com</a>
<a href="tel:+1234567890">+1 (234) 567-8900</a>
```

**Social Media Links:**
Update the social media URLs in the contact section

## 🎯 Sections Overview

### 1. **Header / Navigation Bar**

- Sticky navigation with smooth scrolling
- Mobile hamburger menu
- Dark mode toggle
- Active link highlighting

### 2. **Hero Section**

- Profile picture with blue border
- Name and professional title
- Short introduction
- Call-to-action button

### 3. **Certificates Section**

- Grid layout (3 columns on desktop, 1 on mobile)
- Certificate images
- Titles, descriptions, and years
- Hover effects with upward translation

### 4. **Projects Section**

- Featured project showcase
- Project images with zoom on hover
- Descriptions and tags
- Links to view projects

### 5. **My Work Section**

- Gallery grid layout
- Image overlay on hover
- Project titles and categories
- Responsive to all screen sizes

### 6. **Contact Section**

- Contact form with validation
- Contact information display
- Social media integration
- Form success/error messages

## 💻 Customization Guide

### Change Colors

Edit the CSS variables in `styles.css`:

```css
:root {
  --primary-color: #0066ff; /* Blue */
  --secondary-color: #ff0033; /* Red */
  --white: #ffffff; /* Main background */
  --text-dark: #2c3e50; /* Dark text */
  --text-light: #7f8c8d; /* Light gray text */
}
```

### Update Fonts

Fonts are loaded from Google Fonts. To change:

1. Go to [Google Fonts](https://fonts.google.com/)
2. Select your preferred fonts
3. Copy the import link
4. Replace in `index.html`:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=..." rel="stylesheet" />
   ```

### Add/Remove Sections

Simply add or remove `<section>` blocks in `index.html`. Make sure to update navigation links accordingly.

### Modify Button Styles

All buttons use the `.primary-btn` class. Customize in `styles.css`:

```css
.primary-btn {
  background: linear-gradient(
    135deg,
    var(--primary-color),
    var(--secondary-color)
  );
  /* Modify styles as needed */
}
```

## 🌙 Dark Mode

Dark mode is automatically enabled based on system preferences but can be toggled using the moon/sun icon in the navigation bar. Preference is saved to local storage.

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

## 🔧 JavaScript Features

1. **Mobile Menu Toggle**: Hamburger menu for mobile navigation
2. **Smooth Scrolling**: All internal links use smooth scroll behavior
3. **Dark Mode**: Toggle with local storage persistence
4. **Form Validation**: Email validation and required field checking
5. **Intersection Observer**: Fade-in animations as elements come into view
6. **Active Link Highlighting**: Navigation links highlight based on scroll position
7. **Scroll to Top Button**: Appears when scrolling down
8. **Tilt Effect**: Subtle 3D rotation on project cards (desktop only)

## 📧 Contact Form

The contact form includes:

- Name, email, subject, and message fields
- Email validation
- Required field checking
- Success/error messaging
- Form reset after submission

**Note:** Currently, the form displays a success message but doesn't send emails. To enable email functionality, you'll need to:

1. Set up a backend service (Node.js, PHP, etc.)
2. Use a form service like Formspree, EmailJS, or Netlify Forms
3. Update the JavaScript to send data to your service

Example with EmailJS (free service):

```javascript
emailjs.send("service_id", "template_id", {
  from_name: name,
  email: email,
  subject: subject,
  message: message,
});
```

## 🚀 Deployment

### Option 1: GitHub Pages (Free)

1. Create a GitHub repository
2. Push your files to the repository
3. Enable GitHub Pages in repository settings
4. Your site will be available at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free)

1. Go to [Netlify](https://netlify.com)
2. Drag and drop your folder or connect your Git repository
3. Your site is deployed instantly

### Option 3: Vercel (Free)

1. Push your code to GitHub
2. Go to [Vercel](https://vercel.com)
3. Import your GitHub repository
4. Automatic deployment on every push

### Option 4: Traditional Hosting

1. Use providers like Bluehost, SiteGround, or Godaddy
2. Upload files via FTP
3. Access your site via your domain

## 🎬 Animation Details

- **Fade-in**: 0.6s ease-out animation on scroll
- **Hover Lift**: 10-15px upward movement with shadow
- **Tilt Effect**: Subtle 3D rotation on mouse movement
- **Scale Transform**: 1.1x scale on image hover
- **Heartbeat**: Heart icon pulses in footer

## ⚡ Performance Tips

1. **Optimize Images**: Use tools like TinyPNG to compress images
2. **Lazy Loading**: Implement for below-fold images
3. **Minify CSS/JS**: Use minifiers for production
4. **Caching**: Enable browser caching for better performance
5. **CDN**: Use a CDN for faster content delivery

## 🐛 Troubleshooting

### Images Not Showing

- Check that image URLs are correct and accessible
- Placeholder service may have rate limits; use your own images

### Form Not Working

- Check browser console for JavaScript errors
- Ensure all required fields are filled
- Check email format validation

### Dark Mode Not Working

- Ensure JavaScript is enabled
- Check browser local storage isn't cleared
- Try clearing browser cache

### Responsive Issues

- Clear browser cache (Ctrl+Shift+Delete)
- Check viewport meta tag is present
- Test in different browsers

## 📚 Browser Support

- Chrome/Edge: Latest 2 versions
- Firefox: Latest 2 versions
- Safari: Latest 2 versions
- Mobile browsers: iOS Safari 12+, Chrome Mobile

## 📄 License

Free to use and modify for personal or commercial projects.

## 🤝 Contributing

Feel free to fork and modify this template for your needs!

## 📞 Support

For issues or questions, check the code comments in each file or refer to this documentation.

---

**Made with ❤️ using HTML, CSS & JavaScript**

Happy customizing! 🎉
