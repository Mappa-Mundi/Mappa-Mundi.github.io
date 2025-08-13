# Mappa Mundi Website

A modern, responsive website for the Mappa Mundi mobile app - helping users discover historically significant locations near them.

## 🗺️ About

Mappa Mundi is a mobile application that helps users find and explore historically significant locations, including:
- Historic buildings across thousands of towns and cities
- Castles and forts in Europe and the United States
- Battlefields and historical conflict sites
- Local historical markers and cultural sites

## 🚀 Features

### Website Features
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Performance Optimized**: Fast loading with WebP images, lazy loading, and service worker caching
- **SEO Optimized**: Comprehensive meta tags, structured data, and semantic HTML
- **Accessibility**: WCAG compliant with reduced motion support and proper alt text
- **Blog System**: Jekyll-powered blog with categories and search functionality

### Performance Optimizations
- **Image Optimization**: WebP format with PNG fallbacks (86% size reduction)
- **Resource Hints**: Preload, preconnect, and DNS prefetch for faster loading
- **Service Worker**: Offline functionality and intelligent caching
- **Lazy Loading**: Images load only when needed
- **Deferred JavaScript**: Non-critical scripts load asynchronously

## 🛠️ Technology Stack

- **Static Site Generator**: Jekyll 3.9.3
- **CSS Framework**: Bootstrap 4
- **Styling**: SCSS with custom variables
- **JavaScript**: jQuery, Bootstrap JS
- **Icons**: Font Awesome
- **Performance**: Service Worker, WebP images, Resource hints

## 📁 Project Structure

```
Mappa-Mundi.github.io/
├── _config.yml              # Jekyll configuration
├── _includes/               # Reusable HTML components
├── _layouts/                # Page templates
├── _posts/                  # Blog posts
├── _sass/                   # SCSS stylesheets
│   ├── _home-styles.scss    # Homepage-specific styles
│   ├── _variables.scss      # Custom variables
│   └── bootstrap/           # Bootstrap framework
├── assets/                  # Static assets
│   ├── images/              # Original images
│   ├── images/optimized/    # Optimized WebP/PNG images
│   ├── javascript/          # JavaScript files
│   └── main.scss           # Main stylesheet
├── sw.js                   # Service worker
└── index.html              # Homepage
```

## 🚀 Getting Started

### Prerequisites
- Ruby 2.6+ and Bundler

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Mappa-Mundi/Mappa-Mundi.github.io.git
   cd Mappa-Mundi.github.io
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Build the site**
   ```bash
   bundle exec jekyll build
   ```

4. **Serve locally**
   ```bash
   bundle exec jekyll serve
   ```

## 📝 Content Management

### Adding Blog Posts
1. Create a new file in `_posts/` with format: `YYYY-MM-DD-title.md`
2. Add front matter:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   excerpt: "Brief description"
   categories: [app-updates, travel-guides, historic-spotlights]
   tags: [history, travel, app]
   ---
   ```

### Adding Images
1. Place original images in `assets/images/`
2. Run `./optimize-images.sh` to create optimized versions
3. Use `<picture>` elements in HTML for WebP support

### Updating Content
- **Pages**: Edit HTML files in root directory
- **Styles**: Modify SCSS files in `_sass/` or `assets/`
- **Configuration**: Update `_config.yml` for site-wide settings

## 🔧 Development Tools

### Performance Monitoring
The site includes several performance monitoring tools:
- **Service Worker**: Caches critical resources for offline access
- **Resource Hints**: Preloads critical CSS and images
- **Lazy Loading**: Defers non-critical image loading
- **WebP Support**: Modern image format with fallbacks

### Content Management
- **Blog Posts**: Add new posts in `_posts/` directory
- **Images**: Optimized images are already included in `assets/images/optimized/`
- **Styles**: Modify SCSS files in `_sass/` directory

## 📊 Performance Metrics

Current optimizations provide:
- **86% image size reduction** with WebP format
- **Service worker caching** for offline functionality
- **Resource hints** for faster loading
- **Lazy loading** for improved perceived performance

## 🌐 Deployment

### GitHub Pages
The site is configured for GitHub Pages deployment:
1. Push changes to the `main` branch
2. GitHub Pages automatically builds and deploys
3. Site available at `https://mappamundi.us`

### Manual Deployment
```bash
# Build for production
JEKYLL_ENV=production bundle exec jekyll build

# Deploy to your web server
rsync -av _site/ user@server:/path/to/web/root/
```

## 🔍 SEO & Analytics

### SEO Features
- **Structured Data**: JSON-LD markup for mobile app and organization
- **Meta Tags**: Comprehensive Open Graph and Twitter Card support
- **Sitemap**: Automatic XML sitemap generation
- **Canonical URLs**: Proper canonical link tags

### Analytics Integration
- Google Analytics (add tracking ID to `_config.yml`)
- Google Search Console verification
- Core Web Vitals monitoring

## 🎨 Customization

### Colors & Branding
Edit `_sass/_variables.scss` to customize:
- Primary colors (`#B22222`, `#3D553D`)
- Secondary colors (`#DBC9B0`)
- Typography and spacing

### Layouts
- **Homepage**: `index.html` with hero section and feature carousel
- **Blog**: `blog.html` with post grid and filtering
- **Pages**: Standard Jekyll page layout

## 🐛 Troubleshooting

### Common Issues
1. **Images not loading**: Check that optimized images exist in `assets/images/optimized/`
2. **CSS not updating**: Clear browser cache or run `bundle exec jekyll clean`
3. **Service worker issues**: Check browser console for errors

### Performance Issues
1. Check PageSpeed Insights for specific recommendations
2. Verify image optimization is complete
3. Ensure service worker is properly registered

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Bootstrap Documentation](https://getbootstrap.com/docs/4.6/)
- [Web.dev Performance Guide](https://web.dev/performance/)
- [Google PageSpeed Insights](https://pagespeed.web.dev/)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test the build with `bundle exec jekyll build`
5. Submit a pull request

## 📄 License

This project is proprietary software. All rights reserved.

## 📞 Support

For support or questions:
- Email: contact@mappamundi.us
- Website: https://mappamundi.us
- App Store: [Mappa Mundi on iOS](https://apps.apple.com/us/app/mappa-mundi/id6451006755)

---

*Built with ❤️ for historical discovery*
