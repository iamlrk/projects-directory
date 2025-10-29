# Projects Showcase

A clean, minimal projects showcase website built with Jekyll, using the theme from [iamlrk.github.io](https://github.com/iamlrk/iamlrk.github.io).

Hosted at: [projects.iamlrk.com](https://projects.iamlrk.com)

## Features

- **6 Unique Themes**: Switch between Default, Neobrutalism, Neomorphism, Techno/Cyberpunk, Mission Control, and Retro Space Program
- **Real-time Theme Switching**: Change themes instantly from the navigation bar
- **Theme Persistence**: Your theme choice is saved across sessions
- Clean, minimal design consistent with main personal website
- Fully responsive (mobile, tablet, desktop)
- Fast loading and optimized for performance
- Easy to update and add new projects

### Available Themes

1. **Default** - Clean, professional light theme
2. **Neobrutalism (Brutal)** - Bold, raw design with thick borders and stark colors
3. **Neomorphism (Neomorph)** - Soft, elegant with subtle shadows and depth
4. **Techno/Cyberpunk (Techno)** - Neon colors, glowing effects, futuristic
5. **Mission Control (Mission)** - Aerospace command center aesthetic
6. **Retro Space Program (Retro)** - Vintage NASA/Soviet space program styling

See [THEMES.md](THEMES.md) for detailed theme descriptions.

## Local Development

### Prerequisites

- Ruby (2.7 or higher)
- Jekyll
- Bundler

### Setup

1. Clone this repository:
```bash
git clone <your-repo-url>
cd projects-directory
```

2. Install dependencies:
```bash
gem install bundler jekyll
bundle install
```

3. Run the development server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to `http://localhost:4000`

## Deployment to Cloudflare Pages

### Option 1: GitHub Integration (Recommended)

1. Push your code to a GitHub repository
2. Log in to [Cloudflare Dashboard](https://dash.cloudflare.com/)
3. Go to **Pages** > **Create a project**
4. Select **Connect to Git**
5. Choose your GitHub repository
6. Configure the build settings:
   - **Framework preset**: Jekyll
   - **Build command**: `jekyll build`
   - **Build output directory**: `_site`
   - **Environment variables**: 
     - `JEKYLL_ENV`: `production`
7. Click **Save and Deploy**

### Option 2: Direct Upload

1. Build the site locally:
```bash
JEKYLL_ENV=production bundle exec jekyll build
```

2. Log in to [Cloudflare Dashboard](https://dash.cloudflare.com/)
3. Go to **Pages** > **Create a project**
4. Select **Upload assets**
5. Upload the contents of the `_site` directory
6. Configure your custom domain `projects.iamlrk.com`

### Custom Domain Setup

1. In Cloudflare Pages, go to your project
2. Click on **Custom domains**
3. Add `projects.iamlrk.com`
4. Follow the DNS configuration instructions
5. Add a CNAME record pointing to your Cloudflare Pages deployment

## Adding New Projects

Edit `index.html` and add a new project card:

```html
<div class="project-card">
    <div class="project-header">
        <h3>Your Project Name</h3>
        <div class="project-links">
            <a href="https://github.com/yourusername/project" target="_blank" class="project-link">GitHub</a>
            <a href="https://demo-url.com" target="_blank" class="project-link">Demo</a>
        </div>
    </div>
    <p class="project-description">
        Describe your project here. What does it do? What problem does it solve?
    </p>
    <div class="project-tech">
        <span class="tech-tag">Technology 1</span>
        <span class="tech-tag">Technology 2</span>
        <span class="tech-tag">Technology 3</span>
    </div>
</div>
```

## File Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/
│   └── default.html     # Main layout template
├── css/
│   └── main.css        # Styles (consistent with main site)
├── index.html          # Projects showcase page
├── README.md           # This file
└── .gitignore          # Git ignore rules
```

## Customization

### Colors and Theme

The theme uses CSS variables defined in `css/main.css`. You can customize colors by modifying the `:root` and `[data-theme="dark"]` sections.

### Navigation Links

Edit the Quick Links section in `index.html` to update navigation links.

### Site Information

Update site title, description, and URL in `_config.yml`.

## License

This project uses the same theme as [iamlrk.github.io](https://github.com/iamlrk/iamlrk.github.io).

## Contact

- **Email**: lepakshiramkiran@duck.com
- **GitHub**: [@iamlrk](https://github.com/iamlrk)
- **Website**: [dev.iamlrk.com](https://dev.iamlrk.com)

