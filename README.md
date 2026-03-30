# LEAD AI Launchpad

A platform to empower founders to launch and scale AI-driven ventures through clear strategy, operational excellence, and transformative leadership.

**Website:** [https://lead-ai-launchpad.com/](https://lead-ai-launchpad.com/)

## About

LEAD AI Launchpad was founded by Anand Vijayachandran to provide a platform for entrepreneurs to connect and build. The platform is dedicated to helping founders navigate the complex landscape of AI-driven business ventures.

### Core Values

- **Integrity** - Showing up consistently and earning trust through reliability
- **Respect** - Treating every person with dignity and fostering healthy collaboration
- **Compassion** - Understanding others' perspectives and being considerate of their needs
- **Excellence** - Maintaining high standards and continuously improving

## 📁 Project Structure

```
├── content/              # Website content
│   ├── about/           # About page
│   ├── posts/           # Blog posts
│   └── newsletters/     # Newsletter archives
├── config/              # Hugo configuration
│   └── _default/        # Default config files
├── themes/              # Hugo themes
│   └── blowfish/        # Blowfish theme
├── layouts/             # Custom layout templates
├── static/              # Static assets
├── assets/              # Asset files (images, etc.)
└── build.sh             # Build script for Cloudflare Workers
```

## 🛠️ Technology Stack

- **Static Site Generator:** [Hugo](https://gohugo.io/) (v0.157.0)
- **Theme:** [Blowfish](https://blowfish.page/)
- **Styling:** Dart Sass (v1.98.0)
- **Runtime:** Node.js (v24.14.0)
- **Deployment:** [Cloudflare Workers](https://workers.cloudflare.com/)
- **Analytics:** Google Analytics

## 🚀 Getting Started

### Prerequisites

- Hugo Extended (v0.157.0 or later)
- Node.js (v24.14.0 or later)
- Dart Sass (v1.98.0 or later)
- Go (v1.26.1 or later)

### Local Development

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd lal-website
   ```

2. Run the Hugo development server:
   ```bash
   hugo server
   ```

3. Open your browser and navigate to `http://localhost:1313`

The site will automatically reload when you make changes to content.

### Build

To build the site for production:

```bash
hugo --minify
```

The built site will be in the `public/` directory.

### Automated Build

The repository includes a build script (`build.sh`) that automates the installation of all dependencies and builds the site. This is used for deployment on Cloudflare Workers:

```bash
./build.sh
```

## 📝 Content

### Blog Posts
Located in `content/posts/`, featuring articles on AI strategy, leadership, entrepreneurship, and more.

### Newsletters
Archive of newsletters available in `content/newsletters/`.

### About
Learn more about the founder and the mission of LEAD AI Launchpad in `content/about/`.

## 🌐 Site Features

- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Search Functionality** - Built-in search capability
- **Dark/Light Mode** - Automatic appearance switching based on system preferences
- **Taxonomy Support** - Content organized by tags, categories, authors, and series
- **Social Sharing** - Easy sharing to social media platforms

## 📊 Deployment

The site is automatically deployed to Cloudflare Workers. The `wrangler.toml` file contains the deployment configuration.

### Deployment Process

1. Push changes to the repository
2. Cloudflare Workers picks up the changes
3. The build script installs dependencies
4. Hugo generates the static site
5. Site is deployed and accessible at https://lead-ai-launchpad.com/

## ⚙️ Configuration

Key configuration files:
- `config/_default/hugo.toml` - Main Hugo settings
- `config/_default/params.toml` - Theme parameters
- `config/_default/languages.en.toml` - Language settings
- `config/_default/module.toml` - Module dependencies
- `config/_default/markup.toml` - Markup processing settings
- `wrangler.toml` - Cloudflare Workers configuration

## 🤝 Contributing

When adding new content:

1. Create a new markdown file in the appropriate content directory
2. Add frontmatter with metadata (title, date, description, categories/tags)
3. Write your content using Markdown
4. Test locally with `hugo server`
5. Commit and push changes

## 📄 License

Please refer to LICENSE file for licensing information.

## 📧 Contact

For inquiries about LEAD AI Launchpad, visit [https://lead-ai-launchpad.com/](https://lead-ai-launchpad.com/)