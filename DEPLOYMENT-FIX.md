# Vercel Deployment Fix

## What Was Fixed

The deployment issue was caused by conflicting build configurations between `package.json` and `vercel.json`. Here's what was changed:

### 1. Updated `vercel.json`

- Simplified the configuration to focus on Jekyll build
- Removed conflicting `installCommand` and `functions` sections
- Kept the essential `buildCommand` that installs Ruby gems and builds Jekyll

### 2. Updated `package.json`

- Removed the `build` script that was conflicting with Vercel
- Removed the `engines` section (this is a Ruby project, not Node.js)
- Kept only the local development scripts (`serve` and `clean`)

### 3. Added `.vercelignore`

- Excludes unnecessary files from deployment
- Prevents build artifacts and development files from being uploaded

## How to Redeploy

1. **Commit and push your changes:**

   ```bash
   git add .
   git commit -m "Fix Vercel deployment configuration"
   git push origin main
   ```

2. **Vercel will automatically redeploy** when it detects the push

3. **If you need to manually redeploy:**
   - Go to your Vercel dashboard
   - Find your project
   - Click "Redeploy" or wait for the automatic deployment

## What the Build Process Now Does

1. **Installs Bundler**: `gem install bundler`
2. **Installs Ruby gems**: `bundle install`
3. **Builds Jekyll site**: `bundle exec jekyll build`
4. **Outputs to**: `_site` directory

## Expected Result

The build should now complete successfully and your Jekyll site should be deployed to Vercel without the "command not found" error.

## Troubleshooting

If you still encounter issues:

1. **Check Vercel build logs** for specific error messages
2. **Verify Ruby version** - your `.ruby-version` file specifies Ruby 3.2.0
3. **Ensure all files are committed** - especially `Gemfile`, `Gemfile.lock`, and `.ruby-version`
4. **Check Vercel project settings** - make sure the framework is set to "Jekyll"

Your site should now deploy successfully! 🚀
