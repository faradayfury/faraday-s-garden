# Deploying to Vercel

This guide will walk you through deploying your Jekyll site to Vercel.

## Prerequisites

1. **GitHub Account**: Your code should be in a GitHub repository
2. **Vercel Account**: Sign up at [vercel.com](https://vercel.com)

## Step 1: Push Your Code to GitHub

If you haven't already, push your Jekyll site to a GitHub repository:

```bash
cd digital-garden-jekyll-template
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git push -u origin main
```

## Step 2: Deploy on Vercel

### Option A: Deploy via Vercel Dashboard (Recommended)

1. Go to [vercel.com](https://vercel.com) and sign in
2. Click "New Project"
3. Import your GitHub repository
4. Vercel will automatically detect it's a Jekyll site
5. Configure your project settings:
   - **Framework Preset**: Jekyll
   - **Build Command**: `bundle exec jekyll build`
   - **Output Directory**: `_site`
   - **Install Command**: `bundle install`
6. Click "Deploy"

### Option B: Deploy via Vercel CLI

1. Install Vercel CLI:

   ```bash
   npm i -g vercel
   ```

2. Deploy from your project directory:

   ```bash
   cd digital-garden-jekyll-template
   vercel
   ```

3. Follow the prompts to configure your deployment

## Step 3: Configure Custom Domain (Optional)

1. In your Vercel dashboard, go to your project
2. Click on "Settings" → "Domains"
3. Add your custom domain
4. Update your DNS settings as instructed by Vercel

## Step 4: Environment Variables (If Needed)

If you have any environment variables or API keys, add them in:

- Vercel Dashboard → Project Settings → Environment Variables

## Step 5: Automatic Deployments

Vercel will automatically deploy your site whenever you push changes to your main branch.

## Troubleshooting

### Common Issues:

1. **Build Failures**: Check the build logs in Vercel dashboard
2. **Ruby Version**: Ensure `.ruby-version` file is present and correct
3. **Dependencies**: Make sure `Gemfile` and `Gemfile.lock` are committed
4. **Build Time**: Jekyll builds can take time; be patient

### Build Commands:

- **Build**: `bundle exec jekyll build`
- **Serve Locally**: `bundle exec jekyll serve`
- **Clean**: `bundle exec jekyll clean`

## File Structure for Vercel

The following files are essential for Vercel deployment:

- `vercel.json` - Vercel configuration
- `package.json` - Build scripts and metadata
- `.ruby-version` - Ruby version specification
- `Gemfile` - Ruby dependencies
- `_config.yml` - Jekyll configuration

## Performance Tips

1. **Image Optimization**: Use WebP format for images
2. **Minification**: CSS and JS are already minified in your setup
3. **Caching**: Vercel handles caching automatically
4. **CDN**: Vercel provides global CDN distribution

## Support

If you encounter issues:

1. Check Vercel build logs
2. Review Jekyll build output locally
3. Consult Vercel documentation
4. Check Jekyll documentation

Your site should now be live on Vercel! 🚀
