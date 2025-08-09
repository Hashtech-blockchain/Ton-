# Overview

This is a real-time multiplayer poker application built with React, Express, and PostgreSQL. The application features live poker games with TON blockchain integration for cryptocurrency transactions. Players can join poker tables, participate in Texas Hold'em games, and manage their digital wallet balances through TON cryptocurrency deposits and withdrawals.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **React with TypeScript**: Modern component-based UI with type safety
- **Vite**: Fast development server and optimized production builds
- **Tailwind CSS + shadcn/ui**: Utility-first styling with pre-built accessible components
- **TanStack Query**: Server state management and caching for API calls
- **Wouter**: Lightweight client-side routing

## Backend Architecture
- **Express.js**: RESTful API server with TypeScript support
- **WebSocket Integration**: Real-time game state synchronization using native WebSocket server
- **Drizzle ORM**: Type-safe database operations with PostgreSQL
- **Modular Services**: Separate poker engine and TON service for game logic and blockchain interactions

## Database Design
- **PostgreSQL**: Relational database with comprehensive schema for users, poker tables, games, participants, transactions, and chat messages
- **Drizzle Schema**: Type-safe database schema with relations between entities
- **Migration Support**: Database versioning through Drizzle Kit

## Real-time Communication
- **WebSocket Server**: Custom WebSocket implementation for live game updates
- **Game State Management**: Centralized game state with real-time synchronization across all connected players
- **Connection Management**: User and game-specific connection tracking

## Game Engine
- **Texas Hold'em Implementation**: Complete poker game logic with betting rounds, hand evaluation, and winner determination
- **Player State Management**: Comprehensive tracking of chip counts, positions, actions, and game participation
- **Multi-table Support**: Concurrent poker games with isolated state management

## Authentication & User Management
- **User Profiles**: Basic user system with balance tracking and game statistics
- **Session Management**: User connection mapping for real-time features
- **Transaction History**: Complete audit trail of deposits, withdrawals, and game transactions

## Styling System
- **Design System**: Consistent component library using shadcn/ui
- **Responsive Design**: Mobile-first approach with Tailwind CSS breakpoints
- **Theme Support**: CSS custom properties for consistent theming

# External Dependencies

## Blockchain Integration
- **@neondatabase/serverless**: Neon PostgreSQL serverless database connection
- **TON Blockchain**: Cryptocurrency wallet integration for deposits and withdrawals (simulated in current implementation)

## UI Framework
- **@radix-ui/react-***: Accessible, unstyled UI primitives for components like dialogs, dropdowns, and form controls
- **@tanstack/react-query**: Server state management for API interactions
- **cmdk**: Command palette and search functionality

## Development Tools
- **Drizzle Kit**: Database schema management and migrations
- **tsx**: TypeScript execution for development server
- **esbuild**: Fast JavaScript bundling for production builds

## Real-time Communication
- **ws**: WebSocket library for real-time game state updates

## Styling Dependencies
- **tailwindcss**: Utility-first CSS framework
- **class-variance-authority**: Type-safe variant styling
- **tailwind-merge**: Utility for merging Tailwind classes

## Utility Libraries
- **date-fns**: Date manipulation and formatting
- **nanoid**: Unique ID generation
- **zod**: Runtime type validation and schema parsing