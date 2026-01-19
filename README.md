# Little Gem Cafe Website

A modern, responsive website for Little Gem Cafe in Vero Beach, Florida.

## Features

- **React-based SPA** - Single-page application with client-side routing
- **Fully Responsive** - Mobile-first design optimized for all devices
- **Modern UI** - Built with Tailwind CSS and custom animations
- **Fast Performance** - Lightweight with CDN-hosted dependencies

## Project Structure

```
little-gems/
├── index.html          # Main HTML file with embedded React app
├── littlegem-logo.png  # Cafe logo
├── littlegem-storefront.png  # Storefront image
├── download.webp       # Background image
├── vercel.json         # Vercel deployment configuration
└── README.md          # This file
```

## Deployment to Vercel

### Option 1: Deploy via Vercel CLI

1. Install Vercel CLI (if not already installed):
   ```bash
   npm i -g vercel
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy:
   ```bash
   vercel
   ```

4. For production deployment:
   ```bash
   vercel --prod
   ```

### Option 2: Deploy via GitHub Integration

1. Push your code to GitHub (already done)
2. Go to [vercel.com](https://vercel.com)
3. Click "Add New Project"
4. Import the `little-gems` repository
5. Vercel will auto-detect the configuration from `vercel.json`
6. Click "Deploy"

### Option 3: Deploy via Vercel Dashboard

1. Go to [vercel.com/dashboard](https://vercel.com/dashboard)
2. Click "Add New Project"
3. Select "Import Git Repository"
4. Choose `little-gems`
5. Configure settings (already set in `vercel.json`):
   - Framework Preset: Other
   - Build Command: (leave empty)
   - Output Directory: `.`
6. Click "Deploy"

## Configuration

The `vercel.json` file contains:
- **SPA Routing**: All routes redirect to `index.html` for client-side routing
- **Cache Headers**: Optimized caching for static assets and HTML
- **No Build Step**: Static site, no build command needed

## Custom Domain

After deployment, you can add a custom domain:
1. Go to your project settings in Vercel
2. Navigate to "Domains"
3. Add your custom domain
4. Follow DNS configuration instructions

## Local Development

Simply open `index.html` in a browser or use a local server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Technologies Used

- **React 18** (via CDN)
- **Tailwind CSS** (via CDN)
- **Babel Standalone** (for JSX transformation)
- **Google Fonts** (Inter & Playfair Display)

## License

All rights reserved - Little Gem Cafe
