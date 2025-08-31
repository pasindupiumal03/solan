# Solana Tracker - Modern Web3 Portfolio Dashboard

A modern, glassmorphic Solana portfolio tracker with Phantom wallet integration, real-time token data, and comprehensive wallet analytics.

## ✨ Features

- 🔗 **Phantom Wallet Integration** - Connect/disconnect with seamless wallet management
- 💰 **Portfolio Tracking** - Real-time balance and token holdings display
- 🔍 **Wallet Address Search** - Analyze any Solana wallet address
- 📈 **Trending Tokens** - Discover popular Solana tokens with market data
- 🎨 **Modern Glassmorphic UI** - Beautiful glass effects and smooth animations
- 🌙 **Dark/Light Theme** - Toggle between themes with system preference detection
- 📱 **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- ⚡ **Real-time Data** - Live updates for balances and token prices

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ 
- npm, yarn, or pnpm
- Phantom Wallet browser extension

### Installation

1. **Clone the repository**
   \`\`\`bash
   git clone https://github.com/yourusername/solana-tracker.git
   cd solana-tracker
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   \`\`\`

3. **Set up environment variables**
   \`\`\`bash
   cp .env.example .env.local
   \`\`\`
   
   Edit `.env.local` with your configuration:
   \`\`\`env
   NEXT_PUBLIC_SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
   NEXT_PUBLIC_APP_URL=http://localhost:3000
   \`\`\`

4. **Run the development server**
   \`\`\`bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   \`\`\`

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🏗️ Project Structure

\`\`\`
solana-tracker/
├── app/                    # Next.js 13+ App Router
│   ├── api/               # API routes (server-side)
│   │   ├── tokens/        # Token-related API endpoints
│   │   │   ├── search/    # Token search functionality  
│   │   │   └── [type]/    # Token lists (trending, latest, etc.)
│   │   ├── token/         # Individual token endpoints
│   │   │   └── [address]/ # Get specific token information
│   │   └── wallet/        # Wallet API endpoints
│   │       └── [address]/ # Dynamic wallet data endpoint
│   ├── dashboard/         # Dashboard pages
│   │   ├── wallet/       # Wallet info page
│   │   ├── trending/     # Trending tokens page
│   │   ├── portfolio/    # Portfolio overview
│   │   ├── activity/     # Transaction history
│   │   └── settings/     # User settings
│   ├── globals.css       # Global styles with custom properties
│   ├── layout.tsx        # Root layout with providers
│   └── page.tsx          # Landing page
├── components/            # Reusable React components
│   ├── ui/               # Shadcn/ui components
│   ├── dashboard-layout.tsx
│   ├── wallet-button.tsx
│   └── theme-toggle.tsx
├── hooks/                # Custom React hooks
│   ├── use-phantom-wallet.ts
│   ├── use-wallet-data.ts
│   └── use-trending-tokens.ts
├── lib/                  # Utility functions and wallet integration
│   ├── phantom-wallet.ts # Phantom wallet integration utilities
│   └── utils.ts          # Tailwind CSS utility functions
└── public/               # Static assets
    └── images/           # Token logos and icons
\`\`\`

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `NEXT_PUBLIC_SOLANA_RPC_URL` | Solana RPC endpoint | Yes |
| `NEXT_PUBLIC_APP_URL` | Application URL for redirects | Yes |

### Phantom Wallet Setup

1. Install [Phantom Wallet](https://phantom.app/) browser extension
2. Create or import your Solana wallet
3. Connect to the application using the wallet button

## 🎨 Design System

The application uses a modern glassmorphic design with:

- **Typography**: Inter (headings) + JetBrains Mono (code)
- **Color Palette**: Crypto-themed gradients with purple/blue accents
- **Glass Effects**: Backdrop blur with subtle borders and shadows
- **Animations**: Smooth transitions and hover effects
- **Responsive**: Mobile-first design approach

## 🚀 Deployment

### Deploy to Vercel (Recommended)

1. **Push to GitHub**
   \`\`\`bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   \`\`\`

2. **Deploy to Vercel**
   - Visit [vercel.com](https://vercel.com)
   - Import your GitHub repository
   - Add environment variables in project settings
   - Deploy automatically

### Deploy to Other Platforms

The application is a standard Next.js app and can be deployed to:
- Netlify
- Railway
- DigitalOcean App Platform
- AWS Amplify
- Any Node.js hosting provider

## 🛠️ Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint
- `npm run type-check` - Run TypeScript checks

### Adding New Features

1. Create components in `components/`
2. Add pages in `app/` directory
3. Implement hooks in `hooks/`
4. Add utilities in `lib/`
5. Update types in `types/`

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Phantom Wallet](https://phantom.app/) for wallet integration
- [Solana](https://solana.com/) for the blockchain infrastructure
- [Shadcn/ui](https://ui.shadcn.com/) for the component library
- [Next.js](https://nextjs.org/) for the React framework
- [Tailwind CSS](https://tailwindcss.com/) for styling

## 📞 Support

If you have any questions or need help, please:
- Open an issue on GitHub
- Check the documentation
- Join our community discussions

---

Built with ❤️ for the Solana ecosystem
