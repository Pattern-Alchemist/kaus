# The Pattern Alchemist Landing Page

## Overview

A modern, mystical landing page for "The Pattern Alchemist" - a transformational coaching system that helps users decode karmic patterns, heal emotional trauma, and rewire mind-body-spirit blocks. The application is built as a full-stack solution with React frontend and Express backend, designed to capture leads and provide value through interactive components.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter for client-side routing
- **Styling**: Tailwind CSS with custom theme for mystical aesthetic (charcoal, burnt gold, cosmic indigo)
- **UI Components**: Radix UI primitives with shadcn/ui component library
- **Animations**: Framer Motion for scroll-based animations and microinteractions
- **State Management**: TanStack Query for server state management
- **Form Handling**: React Hook Form with Zod validation

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Runtime**: Node.js with ES modules
- **API Design**: RESTful endpoints for lead capture and PDF downloads
- **Data Storage**: In-memory storage with interface for future database integration
- **Session Management**: Prepared for connect-pg-simple integration

### Build System
- **Bundler**: Vite for frontend development and building
- **TypeScript**: Strict mode enabled with path mapping
- **Development**: Hot module replacement with Vite dev server
- **Production**: ESBuild for server bundling, Vite for client building

## Key Components

### Lead Capture System
- **Lead Capture Form**: Validates and captures user information (firstName, email, intention)
- **Database Schema**: Drizzle ORM with PostgreSQL schema (leads and users tables)
- **API Endpoints**: 
  - `POST /api/leads` - Create new lead
  - `GET /api/leads` - Retrieve leads (admin)
  - `GET /api/download-pdf` - PDF download trigger

### Interactive Elements
- **Karma Pattern Generator**: Interactive tool that generates personalized karma patterns
- **Countdown Timer**: Creates urgency with daily reset countdown
- **Floating WhatsApp Button**: Persistent CTA for WhatsApp engagement
- **Value Points Section**: Three-tier benefit presentation

### UI/UX Features
- **Dark Mode First**: Custom theme with mystical color palette
- **Mobile Responsive**: Mobile-first design approach
- **Glass Morphism Effects**: Modern UI with glass-effect styling
- **Scroll Animations**: Framer Motion powered interactions
- **Toast Notifications**: User feedback system

## Data Flow

1. **User Interaction**: Users interact with the landing page components
2. **Lead Capture**: Form submissions are validated client-side with Zod
3. **API Communication**: TanStack Query manages server communication
4. **Data Storage**: Currently in-memory, prepared for PostgreSQL migration
5. **User Feedback**: Toast notifications confirm successful actions

## External Dependencies

### Frontend Dependencies
- **UI Framework**: React, Radix UI, shadcn/ui components
- **Styling**: Tailwind CSS, class-variance-authority, clsx
- **Animation**: Framer Motion
- **Forms**: React Hook Form, Hookform resolvers
- **HTTP Client**: TanStack Query
- **Validation**: Zod

### Backend Dependencies
- **Server**: Express.js
- **Database**: Drizzle ORM, @neondatabase/serverless (prepared)
- **Session**: connect-pg-simple (prepared)
- **Payment**: Stripe integration (placeholder)

### Development Dependencies
- **Build Tools**: Vite, ESBuild, TypeScript
- **Replit Integration**: Vite plugins for Replit environment

## Deployment Strategy

### Development
- **Environment**: Replit-optimized with development banners and error overlays
- **Hot Reload**: Vite dev server with HMR
- **Database**: In-memory storage for development

### Production
- **Build Process**: 
  1. Frontend built with Vite to `dist/public`
  2. Backend bundled with ESBuild to `dist/index.js`
- **Environment Variables**: `DATABASE_URL` required for production
- **Database**: PostgreSQL via Neon (configured but not implemented)
- **Static Assets**: Served through Express in production

### Database Migration
- **Current**: In-memory storage with interface abstraction
- **Target**: PostgreSQL with Drizzle ORM
- **Migration**: `npm run db:push` command ready for schema deployment

## Changelog

```
Changelog:
- June 29, 2025: Initial setup with basic landing page structure
- June 29, 2025: Enhanced with advanced conversion optimization features:
  * Urgency banner with live visitor counter
  * Social proof counter with animated statistics
  * Exit-intent popup with discount offer
  * Video testimonial components
  * FAQ section with accordion interface
  * Risk reversal guarantees section
  * Bonus stack highlighting ₹13,497 value
  * Scarcity timer for limited offers
  * Sticky CTA for persistent conversion
  * Enhanced testimonials with before/after format
- June 29, 2025: Payment integration and admin dashboard implementation:
  * Google Pay payment integration for Indian market
  * Admin dashboard with lead analytics and conversion tracking
  * ConvertKit email marketing automation (fully configured)
  * Mobile navigation with responsive design optimization
  * Real-time lead capture with automatic email list integration
  * Payment processing endpoints for coaching packages
- June 29, 2025: SEO optimization and comprehensive analytics system:
  * Complete SEO meta tags, structured data, and Open Graph implementation
  * Advanced analytics tracking system with conversion funnel monitoring
  * Real-time user behavior tracking (page views, time on page, scroll depth)
  * WhatsApp click tracking and PDF download analytics
  * Payment conversion tracking with Google Pay integration
  * Analytics dashboard with performance insights and revenue tracking
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```