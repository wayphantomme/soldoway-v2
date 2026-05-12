# ⚡️ Soldoway V2

> **Modern Decentralized Sales Marketplace.**  
> A premium, on-chain platform for businesses to create high-conversion sales campaigns with automated rewards, trustless meeting verification, and real-time yield simulation.

Demo:
https://www.loom.com/share/8e28b7695c3949bd9f89e895fc710d0d

Pitch:
https://www.loom.com/share/34c7a04a41c34af0af7e79a21137acdd

---

## ✨ Features

- **🛡️ Escrow-Protected Campaigns**: Businesses deposit SOL into a secure PDA (Program Derived Address) to fund their sales campaigns.
- **💸 Automated Payouts**: Reward sales representatives instantly for verified meetings via on-chain instructions.
- **📈 Mock Yield Simulation**: Escrowed funds "earn" a simulated 5% APY, demonstrating the potential for integrated yield protocols (like Kamino or Marinade).
- **🔗 Referral Engine**: Built-in referral system for organic growth and viral sales loops.
- **💅 Premium UI/UX**: Built with a "Clean Bauhaus" aesthetic—white base, bold black elements, and warm yellow accents. Responsive and motion-heavy.
- **🔐 Unified Auth**: Seamless onboarding via Privy (Social, Email, and Web3 wallets).

---

## 🛠️ Tech Stack

### Frontend & Core
- **Framework**: [Next.js 15](https://nextjs.org/) (App Router)
- **Styling**: [Tailwind CSS 4](https://tailwindcss.com/)
- **Components**: [shadcn/ui](https://ui.shadcn.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)
- **State Management**: [Zustand](https://github.com/pmndrs/zustand)
- **Auth**: [Privy](https://www.privy.io/)

### Blockchain (Solana)
- **Language**: [Rust](https://www.rust-lang.org/)
- **Framework**: [Anchor](https://www.anchor-lang.com/)
- **Wallet Integration**: [Solana Wallet Adapter](https://solana.com/developers/guides/wallets/add-solana-wallet-adapter-to-nextjs) & [Privy Embedded Wallets](https://docs.privy.io/guide/react/wallets/embedded-wallets)

### Backend & Database
- **Database**: PostgreSQL (via [Supabase](https://supabase.com/))
- **ORM**: [Prisma](https://www.prisma.io/)
- **API**: Next.js Serverless Functions

---

## 🚀 Getting Started

### 1. Prerequisites
- [Node.js](https://nodejs.org/) (v20+)
- [Rust & Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools)
- [Anchor CLI](https://www.anchor-lang.com/docs/installation)
- [Prisma CLI](https://www.prisma.io/docs/getting-started)

### 2. Installation
```bash
# Clone the repository
git clone https://github.com/wayphantomme/soldoway-v2.git
cd soldoway-v2

# Install dependencies
npm install
```

### 3. Environment Setup
Create a `.env` file in the root directory (refer to `.env.example` if available):
```env
DATABASE_URL="your-postgresql-url"
NEXT_PUBLIC_PRIVY_APP_ID="your-privy-app-id"
PRIVY_APP_SECRET="your-privy-secret"
# ... other vars
```

### 4. Database Setup
```bash
npx prisma generate
npx prisma db push
```

### 5. Running the App
```bash
# Start development server
npm run dev

# For Anchor (Local Test Validator)
anchor build
anchor test
```

---

## 🎨 Design Philosophy

Soldoway follows a **Modern Consumer Marketplace** aesthetic:
- **Base**: Clean white (`#FFFFFF`) for clarity.
- **Contrast**: Bold black (`#000000`) for structure and Bauhaus-inspired elements.
- **Accent**: Warm yellow (`#F8D94F`) for CTAs and highlights.
- **Feel**: Approachable, image-forward, and smooth interactions.

---

## 📂 Project Structure

- `anchor/`: Solana smart contract (Anchor program).
- `app/`: Next.js frontend and API routes.
- `components/`: Reusable UI components (shadcn/ui + custom).
- `prisma/`: Database schema and migrations.
- `lib/`: Shared utility functions and database clients.
- `hooks/`: Custom React hooks for Solana and auth logic.

---

## 📄 License

This project is proprietary. All rights reserved.

...
