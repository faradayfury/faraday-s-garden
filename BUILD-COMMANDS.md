# 🔄 Jekyll Build Commands

## Development Server (Recommended)

```bash
cd "digital-garden-jekyll-template"
bundle exec jekyll serve --livereload
```

**What this does:**

- Builds your site automatically
- Serves it locally at http://localhost:4000
- Auto-refreshes when you make changes
- Perfect for development and testing

## Production Build

```bash
cd "digital-garden-jekyll-template"
bundle exec jekyll build
```

**What this does:**

- Generates static files in `_site/` folder
- Optimized for deployment
- Use this for hosting platforms

## Quick Commands

**Start development server:**

```bash
bundle exec jekyll serve
```

**Build once:**

```bash
bundle exec jekyll build
```

**Clean and rebuild:**

```bash
bundle exec jekyll clean && bundle exec jekyll build
```

## Troubleshooting

**If you get dependency errors:**

```bash
bundle install
```

**If changes aren't showing:**

1. Stop server (Ctrl+C)
2. Run: `bundle exec jekyll clean`
3. Restart: `bundle exec jekyll serve`

## Your Photo System

After running any build command, your 4 photos should appear automatically on the homepage photography section:

- DSFC3855.jpg
- DSFC3911.jpg
- DSFC3925.jpg
- DSFC3929.jpg

The remaining 12 slots will show as placeholders until you add more photos.
