# CSRGO Blog - Modern Hugo Theme

A completely custom, modern, responsive, and user-friendly Hugo blog theme built from scratch. Perfect for tech-focused blogs with AI tools, development roadmaps, and cutting-edge technology content.

## ✨ Features

- **🎨 Modern Design** : Clean, minimal, and professional design with dark/light mode support
- **📱 Fully Responsive**: Mobile-first design that works perfectly on all devices
- **⚡ Fast Performance**: Built with Hugo for lightning-fast static site generation
- **🎯 SEO Optimized**: Proper meta tags, structured data, and semantic HTML
- **🔍 Search Ready**: Modular design ready for search functionality
- **📝 Markdown Support**: Write content in Markdown with syntax highlighting
- **🏷️ Tag System**: Organize posts with tags and categories
- **📊 Reading Time**: Automatic reading time calculation
- **🖼️ Image Support**: Optional thumbnail images for posts
- **🔗 Social Sharing**: Built-in social media sharing buttons
- **📱 Mobile Menu**: Responsive navigation with mobile-friendly menu

## 🚀 Quick Start

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (version 0.80.0 or higher)
- Git

### Installation

1. **Clone or download this repository**
   ```bash
   git clone <your-repo-url>
   cd blog
   ```

2. **Start the Hugo development server**
   ```bash
   hugo server -D
   ```

3. **Open your browser**
   Navigate to `http://localhost:1313` to see your blog

## 📁 Project Structure

```
blog/
├── admin/
│   └── config.yml          # Netlify CMS configuration
├── content/
│   └── posts/              # Blog posts (Markdown files)
├── layouts/
│   ├── _default/
│   │   ├── baseof.html     # Base template
│   │   ├── list.html       # Homepage template
│   │   └── single.html     # Single post template
│   └── posts/
│       └── list.html       # All posts page template
├── static/                 # Static assets (images, CSS, JS)
├── config.toml            # Hugo configuration
├── CNAME                  # Custom domain for GitHub Pages
└── README.md              # This file
```

## 📝 Creating Content

### Adding New Posts

1. **Create a new Markdown file** in `content/posts/`
2. **Add frontmatter** with the following fields:

```yaml
---
title: "Your Post Title"
description: "A brief description of your post"
date: 2024-01-15
author: "Your Name"
tags: ["tag1", "tag2", "tag3"]
thumbnail: "https://images.unsplash.com/photo-xxx?w=800&h=400&fit=crop"
readingTime: 8
draft: false
---

Your content here...
```

### Frontmatter Fields

- **title**: The post title (required)
- **description**: Brief description for SEO and previews (required)
- **date**: Publication date (required)
- **author**: Author name (optional, defaults to site author)
- **tags**: Array of tags for categorization (optional)
- **thumbnail**: Featured image URL (optional)
- **readingTime**: Estimated reading time in minutes (optional)
- **draft**: Set to true to hide from public (optional)

## 🎨 Customization

### Site Configuration

Edit `config.toml` to customize your site:

```toml
title = "Your Blog Title"
baseURL = "https://yourdomain.com/"

[params]
  description = "Your site description"
  author = "Your Name"
  github = "https://github.com/yourusername"
  linkedin = "https://linkedin.com/in/yourusername"
  twitter = "https://twitter.com/yourusername"
```

### Styling

The theme uses Tailwind CSS via CDN. You can customize the design by:

1. **Modifying the base template** (`layouts/_default/baseof.html`)
2. **Adding custom CSS** in the `<style>` section
3. **Updating Tailwind classes** throughout the templates

### Adding New Pages

1. Create a new Markdown file in `content/`
2. Add frontmatter with `title` and `description`
3. The theme will automatically create a page using the base template

## 🌐 Deployment

### GitHub Pages

1. **Push your code to GitHub**
2. **Enable GitHub Pages** in your repository settings
3. **Set the source** to your main branch
4. **Add your custom domain** (if using CNAME)

### Netlify

1. **Connect your repository** to Netlify
2. **Set build command**: `hugo`
3. **Set publish directory**: `public`
4. **Deploy**

### Other Platforms

The theme works with any static site hosting service:
- Vercel
- Cloudflare Pages
- AWS S3 + CloudFront
- Any web server

## 🔧 Advanced Features

### Netlify CMS Integration

The theme includes Netlify CMS configuration for easy content management:

1. **Access the admin panel** at `yourdomain.com/admin`
2. **Create and edit posts** through the web interface
3. **Upload images** directly from the CMS

### Search Functionality

To add search functionality:

1. **Add a search template** in `layouts/partials/`
2. **Include search scripts** in the base template
3. **Create a search results page**

### Categories and Tags

The theme supports Hugo's built-in taxonomy system:

- **Tags**: Automatically displayed on posts
- **Categories**: Can be added for broader organization
- **Tag pages**: Available at `/tags/tagname/`

## 🎯 Performance Optimization

### Built-in Optimizations

- **Static generation**: All pages are pre-built
- **Minimal JavaScript**: Only essential scripts loaded
- **Optimized images**: Responsive image handling
- **Fast loading**: CDN-based CSS and icons

### Further Optimizations

1. **Image optimization**: Use WebP format and proper sizing
2. **Lazy loading**: Implement for images
3. **Caching**: Set up proper cache headers
4. **CDN**: Use a CDN for global distribution

## 🐛 Troubleshooting

### Common Issues

1. **Posts not showing**: Check if `draft: false` in frontmatter
2. **Images not loading**: Verify image URLs are accessible
3. **Styling issues**: Clear browser cache and check Tailwind CDN
4. **Build errors**: Ensure Hugo version is 0.80.0+

### Getting Help

- Check the [Hugo documentation](https://gohugo.io/documentation/)
- Review the theme templates for customization
- Test locally before deploying

## 📄 License

This theme is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 🙏 Acknowledgments

- [Hugo](https://gohugo.io/) - Static site generator
- [Tailwind CSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Lucide Icons](https://lucide.dev/) - Beautiful icons
- [Unsplash](https://unsplash.com/) - Stock photos

---

**Built with ❤️ for the developer community** 
