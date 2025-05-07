# KizunaMexico (絆メキシコ)

![KizunaMexico Logo](public/favicon.svg)

[KizunaMexico](https://www.kizunamexico.com/) is a Japanese-language blog dedicated to sharing interesting facts, culture, and stories about Mexico. The site serves a dual purpose: helping the author practice Japanese writing skills while providing valuable information about Mexican culture to Japanese speakers.

## 🌮 Project Overview

KizunaMexico (絆メキシコ) aims to build cultural bridges ("kizuna" means "bond" in Japanese) between Mexico and Japan through engaging content written in Japanese. Topics include Mexican traditions, food, travel destinations, history, and contemporary culture.

## 🚀 Technology

This blog is built with [Astro](https://astro.build/), a modern static site generator that provides:

- ✅ Excellent performance (100/100 Lighthouse score)
- ✅ SEO-friendly structure with canonical URLs and OpenGraph data
- ✅ Sitemap and RSS feed support
- ✅ Markdown & MDX support for easy content creation

## 📂 Project Structure

```text
├── public/           # Static assets (images, favicon, etc.)
├── src/
│   ├── components/   # Reusable UI components
│   ├── content/      # Blog posts and content collections
│   ├── layouts/      # Page layout templates
│   └── pages/        # Page routes and templates
├── astro.config.mjs  # Astro configuration
└── package.json      # Project dependencies
```

## 🧞 Development Commands

| Command | Action |
| :------ | :----- |
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start development server at `localhost:4321` |
| `pnpm build` | Build production site to `./dist/` |
| `pnpm preview` | Preview production build locally |

## ✍️ Content Creation

Blog posts are written in Markdown or MDX format and stored in the `src/content/blog/` directory. Each post includes frontmatter with metadata such as title, publication date, and tags.

## 🌐 Visit the Site

Explore Mexican culture in Japanese at [https://www.kizunamexico.com/](https://www.kizunamexico.com/)

## 📝 Contributing

Interested in contributing? Feel free to:
- Submit corrections for Japanese language content
- Suggest topics about Mexico that might interest Japanese readers
- Report bugs or technical issues

## 📄 License

This project is licensed under the [MIT License](LICENSE).