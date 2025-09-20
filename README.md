# DreamHouse 🏠

A modern real estate platform built with Next.js, featuring property listings, user authentication, and interactive maps.

## ✨ Features

- 🏡 Property listings and search
- 🔐 User authentication with NextAuth.js
- 🗺️ Interactive maps with Mapbox
- 💳 Payment integration with Stripe
- 📸 Image uploads with UploadThing
- 🎨 Modern UI with Tailwind CSS and Radix UI
- 📱 Responsive design
- 🌙 Dark mode support

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: Tailwind CSS, Radix UI components
- **Database**: Prisma ORM
- **Authentication**: NextAuth.js
- **Payments**: Stripe
- **Maps**: Mapbox GL
- **File Uploads**: UploadThing
- **Email**: Resend

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- npm, yarn, pnpm, or bun
- Database (PostgreSQL, MySQL, or SQLite)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/Amddah21/dreamhouse.git
cd dreamhouse
```

2. Install dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
```

3. Set up environment variables:

```bash
cp .env.example .env.local
```

Fill in your environment variables in `.env.local`:

```env
# Database
DATABASE_URL="your_database_url"

# NextAuth
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your_nextauth_secret"

# Mapbox
NEXT_PUBLIC_MAPBOX_ACCESS_TOKEN="your_mapbox_token"

# Stripe
STRIPE_SECRET_KEY="your_stripe_secret_key"
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY="your_stripe_publishable_key"

# UploadThing
UPLOADTHING_SECRET="your_uploadthing_secret"
UPLOADTHING_APP_ID="your_uploadthing_app_id"

# Resend
RESEND_API_KEY="your_resend_api_key"
```

4. Set up the database:

```bash
npm run db:generate
npm run db:push
npm run db:seed
```

5. Run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## 📁 Project Structure

```
dreamhouse/
├── src/
│   ├── app/                 # Next.js app router
│   ├── components/          # Reusable components
│   │   └── ui/             # UI components (Radix UI)
│   └── lib/                # Utility functions
├── prisma/                 # Database schema and migrations
└── public/                 # Static assets
```

## 🗄️ Database Commands

- `npm run db:generate` - Generate Prisma client
- `npm run db:push` - Push schema changes to database
- `npm run db:migrate` - Create and apply migrations
- `npm run db:seed` - Seed the database with sample data
- `npm run db:studio` - Open Prisma Studio

## 🚀 Deployment

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

## 📝 License

This project is licensed under the MIT License.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](../../issues).

## 📞 Support

If you have any questions or need help, please open an issue or contact us.
