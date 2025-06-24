# AJP Stone & Services Website

Professional website for AJP Stone & Services, a high-end construction company specializing in marble, quartz, granite, and porcelain installation in Miami.

## Features

- **Trilingual Support**: Spanish, English, and Portuguese
- **PWA Optimized**: Offline functionality and fast loading
- **Custom Animations**: Construction-themed cursor and rotating service icons
- **SEO Optimized**: Google Analytics, Facebook Pixel, and schema markup
- **Responsive Design**: Mobile-first approach with modern UI
- **Real Portfolio**: Authentic project images and testimonials

## Deployment to Vercel

### Prerequisites
1. Create a [Vercel account](https://vercel.com)
2. Install Vercel CLI: `npm i -g vercel`

### Steps to Deploy

1. **Clone/Download the project**
2. **Set up environment variables in Vercel dashboard:**
   - `VITE_GA_TRACKING_ID` - Google Analytics tracking ID
   - `VITE_FACEBOOK_PIXEL_ID` - Facebook Pixel ID
   - `DATABASE_URL` - PostgreSQL database URL (if using database features)

3. **Deploy using Vercel CLI:**
   ```bash
   vercel
   ```
   Or connect your GitHub repository to Vercel dashboard for automatic deployments.

4. **Custom Domain (Optional):**
   - Add your custom domain in Vercel dashboard
   - Configure DNS records as instructed

### Build Configuration

The project uses:
- **Framework**: React with Vite
- **Build Command**: `npm run vercel-build`
- **Output Directory**: `client/dist`

### Environment Variables

Copy `.env.example` to `.env.local` and fill in your values:

```bash
VITE_GA_TRACKING_ID=G-XXXXXXXXXX
VITE_FACEBOOK_PIXEL_ID=123456789
```

## Local Development

```bash
npm install
npm run dev
```

Visit `http://localhost:5000`

## Project Structure

- `client/` - React frontend application
- `server/` - Express.js backend (for full-stack features)
- `shared/` - Shared types and schemas
- `api/` - Vercel serverless functions

## Technologies Used

- React 18 + TypeScript
- Vite for build tooling
- Tailwind CSS + shadcn/ui
- TanStack Query for state management
- Framer Motion for animations
- Lucide React for icons

## Support

For questions about the website, contact AJP Stone & Services directly through the contact form or WhatsApp integration on the site.