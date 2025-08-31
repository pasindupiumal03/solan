# Solana Tracker - Deployment Guide

## 🚀 Vercel Deployment

### Repository Information
**GitHub Repository:** https://github.com/pasindupiumal03/solan.git

### Prerequisites
1. **Vercel Account**: Sign up at [vercel.com](https://vercel.com)
2. **GitHub Repository**: Already set up at `pasindupiumal03/solan`
3. **Solana Tracker API Key**: Get from [solanatracker.io](https://solanatracker.io)

### Step 1: Environment Variables
Set up these environment variables in your Vercel dashboard:

```bash
SOLANA_TRACKER_API_KEY=your_api_key_here
NEXT_PUBLIC_APP_URL=https://your-vercel-domain.vercel.app
```

### Step 2: Deploy to Vercel

#### Option A: Via Vercel Dashboard
1. Go to [vercel.com/dashboard](https://vercel.com/dashboard)
2. Click "New Project"
3. Import your GitHub repository
4. Add environment variables
5. Click "Deploy"

#### Option B: Via Vercel CLI
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

### Step 3: Verify Deployment
1. Check all pages load correctly
2. Test wallet search functionality
3. Verify trading data displays
4. Check error handling works

## 🔧 Configuration Files

### vercel.json
- Node.js 20.x runtime
- Security headers
- CORS configuration
- API caching strategies

### next.config.mjs
- Image optimization for Solana assets
- Production optimizations
- Console removal in production

### .vercelignore
- Excludes unnecessary files from deployment
- Reduces bundle size

## 🎯 Features Included

✅ **Real-time Token Tracking**
- Trending tokens display
- Price and volume data
- Token address search

✅ **Wallet Analysis**
- Wallet information lookup
- Trading history
- Activity monitoring

✅ **Error Handling**
- Rate limiting protection
- 404 error recovery
- Graceful API failures

✅ **Performance**
- Image optimization
- Code splitting
- Responsive design

## 🛠 Development Commands

```bash
# Install dependencies
npm install

# Development server
npm run dev

# Production build
npm run build

# Start production server
npm start

# Type checking
npm run type-check
```

## 📊 API Endpoints

- `GET /api/wallet/[address]` - Wallet information
- `GET /api/wallet/[address]/trades` - Trading history
- Rate limiting: Built-in protection with exponential backoff

## 🔒 Security Features

- CSP headers
- Rate limiting
- CORS protection
- Environment variable validation
- Error sanitization

## 🌐 Domain Configuration

After deployment, update:
1. `NEXT_PUBLIC_APP_URL` in Vercel environment variables
2. Any hardcoded URLs in the codebase
3. CORS origins if needed

## 📱 Mobile Optimization

- Responsive design
- Touch-friendly interface
- Optimized images
- Fast loading times

---

**Need Help?** Check the Vercel documentation or create an issue in the repository.
