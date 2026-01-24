# BloGsmith

A personal notes-taking site built with Jekyll using the Chirpy theme. Hosted at [https://anky209e.github.io](https://anky209e.github.io).

## 📝 About This Site

This is a static blog/notes platform focused on cloud computing, AWS, and technical documentation. It serves as a personal knowledge base for learning and reference.

- **Theme**: Jekyll Chirpy v5.2+
- **Content**: Technical notes, AWS tutorials, cloud computing concepts
- **Language**: English
- **Deployment**: GitHub Pages (automatic)

## 🚀 Quick Start

### Prerequisites

Ensure you have the following installed:
- Ruby 2.7+ 
- RubyGems
- Jekyll
- Bundler

For detailed installation instructions, see the [Jekyll Docs](https://jekyllrb.com/docs/installation/).

### Local Development Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Anky209e/anky209e.github.io.git
   cd anky209e.github.io
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Start the local development server**
   ```bash
   bundle exec jekyll serve
   ```

4. **View your site**
   Navigate to `http://localhost:4000` in your browser.

### Alternative Local Development

For development with live reload:
```bash
bundle exec jekyll serve --livereload
```

To build the site locally without serving:
```bash
bundle exec jekyll build
```

## 📂 Project Structure

```
.
├── _config.yml              # Jekyll configuration
├── _data/                   # Site data files
│   ├── locales/            # Translation files
│   ├── contact.yml         # Contact information
│   └── share.yml           # Social sharing settings
├── _posts/                  # Blog posts and notes
├── _tabs/                   # Navigation pages
├── _plugins/                # Jekyll plugins
├── assets/                  # Static assets (CSS, JS, images)
├── tools/                   # Deployment and build scripts
├── .github/workflows/       # GitHub Actions workflows
├── Gemfile                  # Ruby dependencies
├── index.html              # Homepage
└── README.md               # This file
```

## ✍️ Content Management

### Creating New Posts

1. Create a new file in `_posts/` with the naming convention: `YYYY-MM-DD-title.md`
2. Add front matter with required fields:
   ```yaml
   ---
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM +/-TTTT
   categories: [Category1, Category2]
   tags: [tag1, tag2, tag3]
   ---
   ```

### Supported Formats

- Markdown with GitHub Flavored Markdown
- HTML embedding
- Syntax highlighting for code blocks
- MathJax support for mathematical expressions

## 🔧 Configuration

### Site Settings

Edit `_config.yml` to customize:
- Site title and description
- Author information
- Social links
- Theme settings
- Google Analytics
- Comments system

### Theme Customization

The Chirpy theme supports:
- Light/dark mode toggle
- Table of contents
- PWA features
- Responsive design
- Search functionality

For advanced customization options, see the [Chirpy Theme Documentation](https://github.com/cotes2020/jekyll-theme-chirpy).

## 🚀 Deployment

### Automatic Deployment

This site uses GitHub Actions for automatic deployment:

1. Push changes to the `main` branch
2. GitHub Actions automatically builds and deploys to GitHub Pages
3. Site is live at `https://anky209e.github.io`

### Manual Testing

To test the build locally before pushing:
```bash
# Build and test (but don't deploy)
bash tools/deploy.sh --dry-run
```

### Build Process

The deployment script (`tools/deploy.sh`) performs:
1. Jekyll site building
2. HTML validation with html-proofer
3. Deployment to `gh-pages` branch
4. GitHub Pages publication

## 🧪 Development Commands

```bash
# Install dependencies
bundle install

# Start development server
bundle exec jekyll serve

# Start with live reload
bundle exec jekyll serve --livereload

# Build site
bundle exec jekyll build

# Test site build
bundle exec html-proofer _site --disable-external --check-html

# Deploy (GitHub Actions only)
bash tools/deploy.sh
```

## 🔍 Available Features

- **Responsive Design**: Works on all devices
- **Dark/Light Mode**: Toggle between themes
- **Search**: Built-in site search
- **Categories & Tags**: Organized content structure
- **Table of Contents**: Auto-generated for posts
- **Social Sharing**: Integrated sharing buttons
- **PWA Support**: Progressive Web App features
- **Comments**: Configurable comment system
- **Analytics**: Google Analytics integration

## 🌐 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 📄 License

This work is published under [MIT License](LICENSE).

## 🤝 Contributing

This is a personal blog, but feel free to:
- Report issues or typos
- Suggest improvements
- Fork for your own use

## 📚 Additional Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Chirpy Theme Documentation](https://github.com/cotes2020/jekyll-theme-chirpy)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 🐛 Troubleshooting

### Common Issues

1. **Bundle install fails**
   ```bash
   gem install --user-install bundler
   bundle install --path vendor/bundle
   ```

2. **Jekyll serve doesn't work**
   ```bash
   bundle exec jekyll clean
   bundle exec jekyll serve
   ```

3. **Permission denied on deploy.sh**
   ```bash
   chmod +x tools/deploy.sh
   ```

### Getting Help

- Check [Jekyll Troubleshooting](https://jekyllrb.com/docs/troubleshooting/)
- Review [GitHub Pages Status](https://www.githubstatus.com/)
- Open an issue in this repository

---

**Built with ❤️ using Jekyll and Chirpy theme**