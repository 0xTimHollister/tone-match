# System Patterns

## Architecture Overview

Tone Match follows a standard browser extension architecture with the following components:

1. **Popup UI (React + TypeScript)**

   - Main user interface that appears when the extension icon is clicked
   - Provides controls for tone analysis and settings

2. **Background Script**

   - Manages state across browser sessions
   - Handles API requests and data processing
   - Coordinates between different parts of the extension

3. **Content Script**
   - Interacts with web page content
   - Captures selected text for analysis
   - Injects UI elements for in-context suggestions

## Design Patterns

### Component Structure

- React functional components with hooks
- TypeScript interfaces for type safety
- CSS modules for component-specific styling

### State Management

- React state for local component state
- Context API for shared state across components
- Browser storage for persisting settings

### Communication Flow

```
User → Content Script → Background Script → API/Processing → UI Updates
```

## Data Flow

1. **Text Selection**:

   - User selects text on a webpage
   - Content script captures the selection

2. **Tone Analysis**:

   - Selected text is sent to the background script
   - Background script processes or sends to external API
   - Results are stored and accessible through the popup

3. **Suggestions**:
   - Based on analysis, suggestions are generated
   - User can apply suggestions directly

## Extension Integration

The extension integrates with the browser using standard Web Extension APIs, leveraging WXT for cross-browser compatibility.
