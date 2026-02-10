# Personal Blog

A clean, minimalist blog built with Astro and Tailwind CSS. Inspired by the aesthetics of [Ben Kuhn](https://www.benkuhn.net), [Nate B Jones](https://www.natebjones.com), and [Paul Stamatiou](https://paulstamatiou.com).

## Features

- 🚀 **Fast** - Built with Astro for optimal performance
- 📝 **Clean Design** - Minimalist, readable typography
- 📱 **Responsive** - Works great on all devices
- 🎨 **Tailwind CSS** - Easy to customize
- 📚 **Blog Categories** - Organize posts by topic
- 🔍 **SEO Friendly** - Optimized meta tags and structure

## Stack

- **Framework**: [Astro](https://astro.build)
- **Styling**: [Tailwind CSS](https://tailwindcss.com)
- **Deployment**: Cloudflare Pages
- **Font**: Inter (via Google Fonts)

## Quick Start

### Prerequisites

- Node.js 18+ installed
- npm or yarn

### Installation

1. Clone this repository:
```bash
git clone <your-repo-url>
cd blog-site
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser to `http://localhost:4321`

## Project Structure

```
/
├── src/
│   ├── layouts/
│   │   ├── BaseLayout.astro   # Main layout wrapper
│   │   └── BlogPost.astro     # Blog post layout
│   ├── pages/
│   │   ├── index.astro        # Homepage
│   │   ├── writing.astro      # Blog listing page
│   │   ├── about.astro        # About page
│   │   └── blog/              # Individual blog posts
│   └── styles/
│       └── global.css         # Global styles + Tailwind
├── public/                    # Static assets
└── astro.config.mjs          # Astro configuration
```

## Customization

### Update Site Info

1. **Name and Links**: Edit `src/layouts/BaseLayout.astro`
   - Update "Your Name" in the nav and footer
   - Update social links (Twitter, GitHub, Email)

2. **Homepage**: Edit `src/pages/index.astro`
   - Update the hero section with your info
   - Modify featured posts

3. **About Page**: Edit `src/pages/about.astro`
   - Add your bio and background
   - List your projects
   - Update social links

### Add Blog Posts

Create new `.astro` files in `src/pages/blog/`:

```astro
---
import BlogPost from '../../layouts/BlogPost.astro';
---

<BlogPost
  title="Your Post Title"
  description="A brief description"
  date="Feb 10, 2026"
  category="Tech & AI"
  readTime="5 min read"
>
  <p>Your content here...</p>
</BlogPost>
```

### Categories

Current categories:
- Tech & AI
- Crypto & Web3
- Personal
- Tutorials

To add/modify categories, update the posts in `src/pages/writing.astro`.

### Styling

All styles are in `src/styles/global.css`. The site uses Tailwind CSS, so you can customize:

- Colors
- Typography
- Spacing
- Components

Tailwind configuration: `tailwind.config.mjs`

## Deployment

### Cloudflare Pages

1. Push your code to GitHub

2. Go to [Cloudflare Pages](https://pages.cloudflare.com/)

3. Click "Create a project"

4. Select your repository

5. Configure build settings:
   - **Build command**: `npm run build`
   - **Build output directory**: `dist`
   - **Root directory**: (leave empty)

6. Click "Save and Deploy"

Your site will be live at `<your-project>.pages.dev`!

### Custom Domain

1. In Cloudflare Pages, go to your project

2. Click "Custom domains"

3. Add your domain (must be managed by Cloudflare)

4. Follow the instructions to configure DNS

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run astro` - Run Astro CLI commands

## License

MIT - Feel free to use this template for your own blog!

## Credits

Design inspired by:
- [Ben Kuhn](https://www.benkuhn.net) - Clean, minimal design
- [Nate B Jones](https://www.natebjones.com) - Substack-style writing page
- [Paul Stamatiou](https://paulstamatiou.com) - Beautiful typography

Built with:
- [Astro](https://astro.build)
- [Tailwind CSS](https://tailwindcss.com)
- [Inter Font](https://fonts.google.com/specimen/Inter)

---

Made with ❤️ using Astro and Tailwind CSS
