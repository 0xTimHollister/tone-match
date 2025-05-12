# Technical Context

## Technology Stack

### Core Technologies

- **WXT (Web Extension Tools)**: Framework for building browser extensions
- **React**: UI library for building component-based interfaces
- **TypeScript**: JavaScript with strong type checking
- **Bun**: Package manager and build tool

### Development Tools

- **VSCode/Cursor**: Recommended editor for development
- **ESLint**: Static code analysis for identifying problems
- **Prettier**: Code formatter for consistent code style

## Development Environment Setup

### Prerequisites

- Node.js (v18+ recommended)
- Bun package manager
- Git for version control

### Installation

```bash
# Clone the repository
git clone [repository-url]

# Navigate to project directory
cd tone-match

# Install dependencies
bun install

# Start development server
bun run dev
```

## Browser Extension APIs

The extension uses the following browser APIs:

- `tabs`: For accessing and manipulating browser tabs
- `storage`: For saving user preferences and data
- `runtime`: For background script communication
- `scripting`: For injecting content scripts

## Testing Strategy

- Manual testing on Chrome and Firefox
- Unit tests for utility functions and components
- End-to-end testing for critical user flows

## Build and Deployment

WXT is configured to build for multiple browsers:

```bash
# Build for Chrome
bun run build

# Build for Firefox
bun run build:firefox

# Create distribution ZIP files
bun run zip         # For Chrome
bun run zip:firefox # For Firefox
```

## Dependencies

- React and React DOM for UI components
- TypeScript for type checking
- WXT and related modules for extension development

## Technical Constraints

- Browser-specific limitations and API differences
- Processing limitations for client-side analysis
- Security restrictions imposed by browser extension models
