# Phonetic Formatter Website

This directory contains the website files for Phonetic Formatter, designed to be deployed on GitHub Pages.

## Files

- `index.html` - Main marketing/landing page
- `support.html` - Support and FAQ page
- `privacy.html` - Privacy Policy page
- `terms.html` - Terms of Service page

## GitHub Pages Setup

### Step 1: Create GitHub Repository

1. Create a new repository on GitHub (e.g., `phonetic-formatter-website`)
2. Make sure the repository is public (required for free GitHub Pages)

### Step 2: Upload Files

1. Upload all files from the `docs` folder to the root of your repository
2. Or, if you want to keep them in a `docs` folder, configure GitHub Pages to use `/docs` as the source

### Step 3: Enable GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select:
   - **Option A**: "Deploy from a branch" → Select `main` branch and `/ (root)` folder
   - **Option B**: "Deploy from a branch" → Select `main` branch and `/docs` folder (if files are in docs folder)
4. Click "Save"

### Step 4: Access Your Website

Your website will be available at:
- `https://YOUR_USERNAME.github.io/phonetic-formatter-website/`

Or if you use a custom domain:
- `https://yourdomain.com`

## Customization

### Add Logo Files

1. Create or obtain your logo files:
   - `logo.png` - Main logo (200x60px, transparent background, white/light color)
   - `favicon.png` - Browser icon (32x32px or 64x64px)
2. Place both files in the `docs` folder alongside the HTML files
3. The website will automatically display the logo if files exist

See `LOGO_REQUIREMENTS.md` for detailed logo specifications.

### Update URLs

Before deploying, update these URLs in all HTML files:
1. Replace `YOUR_USERNAME` with your GitHub username in:
   - Open Graph URLs
   - Twitter Card URLs
   - Canonical URLs
   - Structured Data image URLs

2. Update App Store link in `index.html`:
```html
<a href="https://apps.apple.com/app/phonetic-formatter/idYOUR_APP_ID" class="cta-button">
```
Replace `YOUR_APP_ID` with your actual App Store app ID.

### Update Contact Email

All pages use `phoneticformatter@outlook.com`. To change it, search and replace across all HTML files.

### Custom Domain (Optional)

1. Purchase a domain name
2. In your repository settings → Pages, add your custom domain
3. Configure DNS records as instructed by GitHub
4. Update any hardcoded URLs if needed

## Testing Locally

You can test the website locally before deploying:

1. Open any HTML file in a web browser
2. Or use a local server:
   ```bash
   cd docs
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000`

## URLs for App Store Connect

Once deployed, use these URLs in App Store Connect:

- **Marketing URL**: `https://YOUR_USERNAME.github.io/phonetic-formatter-website/`
- **Support URL**: `https://YOUR_USERNAME.github.io/phonetic-formatter-website/support.html`
- **Privacy Policy URL**: `https://YOUR_USERNAME.github.io/phonetic-formatter-website/privacy.html`
- **Terms of Service URL**: `https://YOUR_USERNAME.github.io/phonetic-formatter-website/terms.html`

## Notes

- All pages are responsive and work on mobile devices
- The design uses a modern, clean aesthetic with iOS-inspired colors
- All content is in English only
- Pages are linked together with a consistent navigation menu
