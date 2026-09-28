# Vectorless Document Intelligence

An AI-powered document intelligence application built with Next.js and TypeScript for processing, understanding, and navigating PDF documents.

## Overview

Vectorless Document Intelligence explores a structure-aware approach to document intelligence. Instead of relying primarily on vector embeddings for document retrieval, the application focuses on extracting document content, indexing pages, and building hierarchical representations of documents.

The project combines PDF processing, document structure analysis, and browser-based AI capabilities into an interactive web application.

## Features

- PDF document processing using PDF.js
- Document text extraction
- Page-level indexing
- Hierarchical document structure generation
- Tree-based document representation
- Browser-based LLM integration using WebLLM
- Interactive document interface
- Client-side document processing
- Responsive user interface
- Type-safe development with TypeScript

## Tech Stack

### Frontend

- Next.js 16
- React 19
- TypeScript
- Tailwind CSS
- Lucide React

### AI

- WebLLM
- Browser-based Large Language Models

### Document Processing

- PDF.js
- Custom PDF parsing
- Page indexing
- Tree-based document structure

### Development

- ESLint
- TypeScript
- npm
- Git

## Project Structure

```text
intelli/
├── public/
│
├── src/
│   ├── app/
│   │   ├── favicon.ico
│   │   ├── globals.css
│   │   ├── layout.tsx
│   │   └── page.tsx
│   │
│   └── lib/
│       ├── llm.ts
│       ├── pageIndexEngine.ts
│       ├── pdfParser.ts
│       └── treeBuilder.ts
│
├── .gitignore
├── eslint.config.mjs
├── next.config.ts
├── package.json
├── package-lock.json
├── postcss.config.mjs
└── tsconfig.json
```

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js
- npm
- Git

### Clone the Repository

```bash
git clone https://github.com/manisai026/intelli.git
cd intelli
```

### Install Dependencies

```bash
npm install
```

### Run the Development Server

```bash
npm run dev
```

Open your browser and visit:

```text
http://localhost:3000
```

## Available Scripts

### Development

```bash
npm run dev
```

Starts the Next.js development server.

### Production Build

```bash
npm run build
```

Creates a production build of the application.

### Production Server

```bash
npm run start
```

Starts the production server after building the application.

### Lint

```bash
npm run lint
```

Runs ESLint against the project.

## Document Processing Pipeline

```text
PDF Document
     │
     ▼
PDF Parsing
     │
     ▼
Text Extraction
     │
     ▼
Page Indexing
     │
     ▼
Document Structure
     │
     ▼
Tree Representation
     │
     ▼
AI / LLM Processing
     │
     ▼
Intelligent Document Interaction
```

## Design Approach

The project explores a vectorless approach to document intelligence.

Rather than making a vector database the central component of document retrieval, the application focuses on document structure, page indexing, and hierarchical relationships between sections.

This structure-aware representation can help preserve the organization and context of complex documents while supporting intelligent document interaction.

## Configuration

The project uses TypeScript with the following path alias:

```text
@/* → ./src/*
```

This allows imports such as:

```typescript
import { example } from "@/lib/example";
```

## Development Workflow

To contribute or modify the project:

1. Clone the repository.
2. Install dependencies with `npm install`.
3. Create a feature branch.
4. Make your changes.
5. Run linting and build checks.
6. Commit your changes.
7. Push the branch to GitHub.

Example:

```bash
git checkout -b feature/my-feature

npm install
npm run lint
npm run build

git add .
git commit -m "Add document processing feature"
git push origin feature/my-feature
```

## Dependencies

The core dependencies include:

- `next`
- `react`
- `react-dom`
- `pdfjs-dist`
- `@mlc-ai/web-llm`
- `lucide-react`

Development dependencies include TypeScript, ESLint, Tailwind CSS, and related Next.js tooling.

## License

This project currently does not specify a license.

## Author

**Mani Sai Gandra**

GitHub: [manisai026](https://github.com/manisai026)
