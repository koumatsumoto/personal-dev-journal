# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal development journal application built with Remix + Vite and TypeScript. The application is designed to run as a GitHub-integrated SPA with GitHub authentication, repository-based data storage, and GitHub Pages hosting. The project uses Tailwind CSS for styling and follows Remix v3 patterns with future flags enabled.

## Development Commands

- **Start development server**: `npm run dev`
- **Build for production**: `npm run build`
- **Start production server**: `npm start`
- **Type checking**: `npm run typecheck`
- **Linting**: `npm run lint`
- **Formatting**: `npm run fmt`

## Architecture

- **Remix Application**: Uses Vite as the bundler with future flags enabled (v3_singleFetch, v3_lazyRouteDiscovery, etc.)
- **TypeScript Configuration**: Strict mode enabled with path mapping (`~/*` -> `./app/*`)
- **Styling**: Tailwind CSS with PostCSS, includes Inter font from Google Fonts
- **Entry Points**:
  - Client: `app/entry.client.tsx`
  - Server: `app/entry.server.tsx`
  - Root: `app/root.tsx` (Layout component with global styles)
- **Routes**: File-based routing in `app/routes/` directory
- **Static Assets**: Served from `public/` directory

## Build Output

Production builds generate:

- `build/server/` - Server-side code
- `build/client/` - Client-side assets

## Key Configuration Files

- `vite.config.ts` - Vite and Remix configuration with future flags
- `tsconfig.json` - TypeScript configuration with path mapping
- `tailwind.config.ts` - Tailwind CSS configuration
- `postcss.config.js` - PostCSS configuration for Tailwind

## Workflow Rules

- **Always run formatting after code edits**: Execute `npm run fmt` whenever code editing is completed to maintain consistent code formatting throughout the project.
