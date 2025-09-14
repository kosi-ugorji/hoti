# HOTI Website Deployment Guide

## GitHub Pages Setup

This website is ready for deployment on GitHub Pages. Follow these steps to activate it:

### 1. Enable GitHub Pages
1. Go to your repository on GitHub
2. Click on **Settings** tab
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch (or the branch containing your website files)
6. Select **/ (root)** as the folder
7. Click **Save**

### 2. Your Website Will Be Available At:
```
https://kosi-ugorji.github.io/hoti/
```

### 3. Custom Domain (Optional)
If you want to use a custom domain:
1. Add a `CNAME` file to the root directory with your domain name
2. Configure your domain's DNS to point to GitHub Pages
3. Update the **Custom domain** setting in GitHub Pages settings

## Website Features

### Responsive Design
- Mobile-first approach
- Tablet and desktop optimized
- Accessible navigation with hamburger menu

### Interactive Elements
- FAQ accordion functionality
- Contact form with validation
- Newsletter signup
- Program enrollment notifications
- Smooth scrolling navigation

### SEO Optimized
- Meta tags for search engines
- Semantic HTML structure
- OpenGraph tags for social sharing
- Sitemap generation via Jekyll

### Performance Features
- CSS Grid and Flexbox for efficient layouts
- Lazy loading capabilities
- Optimized images and assets
- Minimal JavaScript for fast loading

## Content Management

### Adding New Programs
Edit the `index.html` file and add new program cards in the Programs section. Follow the existing structure:

```html
<div class="program-card">
    <div class="program-icon">
        <i class="fas fa-icon-name"></i>
    </div>
    <h3>Program Name</h3>
    <p>Program description...</p>
    <div class="program-details">
        <span class="duration">X weeks</span>
        <span class="spots">Y spots available</span>
    </div>
    <button class="btn btn-outline">Enroll Now</button>
</div>
```

### Adding Blog Posts
Add new blog cards in the Blog & Resources section:

```html
<article class="blog-card">
    <div class="blog-image">
        <i class="fas fa-icon-name"></i>
    </div>
    <div class="blog-content">
        <h3>Blog Post Title</h3>
        <p>Brief description...</p>
        <a href="#" class="read-more">Read More</a>
    </div>
</article>
```

### Updating FAQ
Add new FAQ items in the FAQ section:

```html
<div class="faq-item">
    <div class="faq-question">
        <h3>Your question here?</h3>
        <i class="fas fa-chevron-down"></i>
    </div>
    <div class="faq-answer">
        <p>Your answer here...</p>
    </div>
</div>
```

## Customization

### Colors
Update CSS custom properties in `assets/css/style.css`:

```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #f59e0b;
    --accent-color: #10b981;
    /* ... other colors */
}
```

### Fonts
The website uses Inter font from Google Fonts. To change:
1. Update the Google Fonts link in `index.html`
2. Update the font-family in CSS

### Contact Information
Update contact details in the Contact section of `index.html`:
- Address
- Phone number
- Email
- Business hours

## Browser Support

The website supports:
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome Mobile)

## File Structure

```
/
├── index.html              # Main website file
├── 404.html               # Custom 404 error page
├── _config.yml            # Jekyll configuration
├── .gitignore             # Git ignore rules
├── DEPLOYMENT.md          # This file
├── README.md              # Project documentation
└── assets/
    ├── css/
    │   └── style.css      # Main stylesheet
    └── js/
        └── script.js      # Interactive functionality
```

## Support

For any issues or questions about the website:
1. Check the browser console for JavaScript errors
2. Verify all files are properly uploaded
3. Ensure GitHub Pages is enabled in repository settings
4. Allow up to 10 minutes for GitHub Pages to build and deploy changes

## Future Enhancements

Consider adding:
- Content Management System (CMS) integration
- E-commerce for program fees (if needed)
- Multi-language support
- Advanced analytics tracking
- Blog post management system
- User registration and login system