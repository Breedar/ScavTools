# ScavTools

A developer utilities platform built for Web3 and StarkNet developers. ScavTools bundles a collection of everyday developer tools into a single, clean interface — from JSON formatting and JWT decoding to StarkNet address shortening and PDF generation.

## What It Does

ScavTools gives developers quick access to tools they reach for repeatedly, without switching between tabs or third party sites. All tools are available from a unified dashboard with authentication and access logging.

## Tools Available

| Tool | Description |
|------|-------------|
| Address Shortener | Shortens StarkNet wallet addresses for easier sharing |
| Base64 Encoder / Decoder | Encode and decode Base64 strings |
| Box Shadow Generator | Visually build CSS box shadow values |
| Code Snippet Saver | Save and retrieve reusable code snippets |
| Hash Generator | Generate SHA and other hash values from input |
| JSON Formatter | Prettify and validate JSON payloads |
| JWT Decoder | Decode and inspect JWT token headers and payloads |
| PDF Generator | Convert HTML or Markdown content to downloadable PDFs |
| Regex Tester | Test and debug regular expressions in real time |
| StarkNet Reader | Read on chain data from StarkNet contracts |
| Uptime Monitor | Monitor URLs and track availability |
| Web Screenshot Tool | Capture screenshots of web pages |

## Tech Stack

### Frontend
- **Framework:** Next.js 14 (App Router, TypeScript)
- **Styling:** Tailwind CSS + shadcn/ui
- **Auth:** JWT with refresh token support

### Backend
- **Framework:** NestJS (TypeScript)
- **Database:** Prisma ORM
- **Auth:** JWT, OTP verification, email service, refresh tokens
- **Features:** Tool access logging, StarkNet address shortener, PDF generation (HTML and Markdown)

### Contract
- StarkNet smart contract layer (in progress)

## Project Structure

```
ScavTools/
├── frontend/        # Next.js web app (tools UI, dashboard, auth)
├── backend/         # NestJS API (auth, tools, PDF, address shortener)
└── contract/        # StarkNet smart contracts
```

## Getting Started

### Backend

```bash
cd backend
npm install
cp .env.example .env.development
npx prisma migrate dev
npm run start:dev
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## License

MIT