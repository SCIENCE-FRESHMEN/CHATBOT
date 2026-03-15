# CHATBOT - Next.js Project Template

A modern, production-ready Next.js template for building chatbot applications, featuring a robust engineering setup with TypeScript, Tailwind CSS, Drizzle ORM, and React Query.

## 🚀 Key Features
- **Framework**: Next.js (App Router) with React Server Components support
- **Type Safety**: Full TypeScript integration
- **Styling**: Tailwind CSS + PostCSS (atomic CSS approach)
- **Data Management**: React Query for async state management
- **Database**: Drizzle ORM (lightweight TypeScript ORM)
- **Code Quality**: ESLint configuration for consistent code style
- **Deployment**: Optimized for Vercel (native Next.js platform)
- **UI Component System**: Pre-configured for shadcn/ui integration

## 🛠️ Prerequisites
- Node.js 18.x or later
- npm/yarn/pnpm/bun (package manager)
- A database instance (compatible with Drizzle ORM: PostgreSQL, MySQL, SQLite, etc.)

## 📦 Installation

1. Clone the repository
   ```bash
   git clone <repository-url>
   cd CHATBOT
   ```

2. Install dependencies
   ```bash
   # Using npm
   npm install

   # Using yarn
   yarn install

   # Using pnpm
   pnpm install

   # Using bun
   bun install
   ```

3. Configure environment variables
   Create a `.env.local` file in the root directory and add your environment variables (e.g., database credentials):
   ```env
   # Database URL (example for SQLite)
   DATABASE_URL="sqlite://./db.sqlite"

   # Optional: API keys for chatbot/AI services
   # AI_API_KEY="your-api-key-here"
   ```

4. Set up the database
   ```bash
   # Run database migrations (Drizzle ORM)
   npm run db:migrate
   ```

## 🏃‍♂️ Development

Start the development server:
```bash
# Using npm
npm run dev

# Using yarn
yarn dev

# Using pnpm
pnpm dev

# Using bun
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application. The page auto-updates as you edit files (hot reloading).

## 🏗️ Build for Production

Generate a production build:
```bash
# Using npm
npm run build

# Using yarn
yarn build

# Using pnpm
pnpm build

# Using bun
bun build
```

Start the production server:
```bash
# Using npm
npm start

# Using yarn
yarn start

# Using pnpm
pnpm start

# Using bun
bun start
```

## 🚢 Deployment

### Vercel Deployment (Recommended)
1. Connect your repository to Vercel
2. Vercel automatically detects the Next.js project and configures build settings
3. Deploy with a single click

### Other Deployment Options
Follow the [official Next.js deployment documentation](https://nextjs.org/docs/deployment) for options like AWS, Netlify, Docker, or self-hosting.

## 📁 Project Structure

```
CHATBOT/
├── public/                # Static assets (images, icons, etc.)
├── src/
│   ├── app/               # Next.js App Router (routes, layouts, pages)
│   ├── components/        # Reusable React components
│   ├── db/                # Database logic (migrations, schema, queries)
│   ├── lib/               # Utility functions, helpers, and shared logic
│   └── QueryClientProvider.tsx # React Query configuration
├── .env.local             # Environment variables (gitignored)
├── drizzle.config.ts      # Drizzle ORM configuration
├── next.config.ts         # Next.js core configuration
├── package.json           # Dependencies and scripts
├── postcss.config.mjs     # PostCSS configuration
├── tailwind.config.ts     # Tailwind CSS configuration
└── tsconfig.json          # TypeScript configuration
```

## 📌 Extending the Template
This template provides a solid engineering foundation for chatbot development. To add chatbot-specific functionality:
1. Integrate AI/LLM APIs (OpenAI, Anthropic, etc.) in `src/lib/`
2. Build conversation UI components in `src/components/`
3. Implement chat history persistence using Drizzle ORM
4. Add real-time messaging (WebSockets) if needed
5. Extend React Query hooks for chat data fetching/caching

## 🧪 Testing
Add testing configuration (Jest, React Testing Library, Cypress) based on your project needs:
```bash
# Install testing dependencies (example)
npm install --save-dev jest @testing-library/react @testing-library/jest-dom
```

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 📚 Resources
- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Drizzle ORM Documentation](https://orm.drizzle.team/)
- [React Query Documentation](https://tanstack.com/query/latest)
- [shadcn/ui Documentation](https://ui.shadcn.com/)
