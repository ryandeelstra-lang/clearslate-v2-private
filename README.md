# ClearSlate

A modern debt resolution platform.

## Overview

Web application for managing consumer debt resolution workflows, including payment processing, dispute management, and operations tools.

## Tech Stack

- **Frontend**: Next.js 15 (App Router), React, TailwindCSS
- **Backend**: TypeScript, Next.js API routes
- **Infrastructure**: Vercel
- **Tests**: Jest, TypeScript

## Project Structure

```
app/                # Next.js application
  ├── api/          # API routes
  ├── offer/        # Resolution offer flows
  ├── pay/          # Payment processing
  ├── dispute/      # Dispute management
  ├── verify/       # Verification flows
  └── ops/          # Operations dashboard

core/               # Core business logic (framework-agnostic TypeScript)
  ├── clearance/    # Account clearance logic
  ├── payments/     # Payment processing
  ├── email/        # Email templates & sending
  ├── ledger.ts     # Transaction ledger
  ├── tape.ts       # Data parsing
  └── sol.ts        # Legal logic

docs/               # Documentation (private)
```

## Development

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Run tests
npm test

# Type check
npm run type-check

# Build for production
npm run build
```

## Environment Variables

See `.env.example` for required configuration.

## Testing

```bash
# Run all tests
npm test

# Run tests in watch mode
npm test:watch

# Run specific test file
npm test core/ledger.test.ts
```

## License

Private - All Rights Reserved
