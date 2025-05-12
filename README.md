# Tone Match

A browser extension for analyzing and matching the tone of written text, built with WXT, React, and TypeScript.

## Features

- Analyze the tone of selected text on web pages
- Compare against predefined tone profiles
- Get suggestions for tone adjustments
- Seamlessly integrate with common writing platforms
- Privacy-focused design

## Tech Stack

- [WXT](https://wxt.dev) (Web Extension Tools)
- [React](https://react.dev)
- [TypeScript](https://www.typescriptlang.org/)
- [Bun](https://bun.sh) (Package Manager)

## Development

### Prerequisites

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [Bun](https://bun.sh) package manager
- Git

### Setup

```bash
# Clone the repository
git clone [repository-url]

# Navigate to project directory
cd tone-match

# Install dependencies
bun install

# Start development server
bun run dev

# Build for Chrome
bun run build

# Build for Firefox
bun run build:firefox

# Create distribution ZIP files
bun run zip         # For Chrome
bun run zip:firefox # For Firefox
```

## Project Structure

```
tone-match/
├── .wxt/             # Generated WXT files
├── assets/           # Static assets
├── entrypoints/      # Extension entry points
│   ├── popup/        # Popup UI components
│   ├── background.ts # Background script
│   └── content.ts    # Content script
├── public/           # Public files
├── memory-bank/      # Project documentation
├── package.json      # Dependencies and scripts
├── tsconfig.json     # TypeScript configuration
└── wxt.config.ts     # WXT configuration
```

## Documentation

See the [memory-bank](./memory-bank) directory for detailed project documentation.

## License

[MIT](LICENSE)
