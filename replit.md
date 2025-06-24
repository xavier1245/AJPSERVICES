# AJP Stone & Services - High-End Construction Website

## Overview

This is a full-stack web application for AJP Stone & Services, a high-end construction company specializing in marble, quartz, granite, and porcelain installation in Miami. The application is built as a modern single-page application with a React frontend and Express.js backend, featuring a professional landing page with contact forms and project showcases.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter (lightweight client-side routing)
- **State Management**: TanStack Query (React Query) for server state
- **UI Framework**: Tailwind CSS with shadcn/ui components
- **Build Tool**: Vite for fast development and optimized production builds
- **Component Library**: Radix UI primitives for accessibility

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Runtime**: Node.js 20
- **Database ORM**: Drizzle ORM with PostgreSQL dialect
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **Session Management**: PostgreSQL session store
- **Development**: tsx for TypeScript execution in development

## Key Components

### Database Schema
The application uses a simple user authentication schema:
- **Users Table**: Contains id (serial), username (unique), and password fields
- **Validation**: Zod schemas for type-safe data validation
- **Migrations**: Drizzle Kit for database schema management

### Frontend Components
- **Landing Page**: Professional showcase with hero section, services, projects, and contact
- **UI Components**: Complete shadcn/ui component library for consistent design
- **Form Handling**: React Hook Form with Zod validation
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Toast Notifications**: User feedback system for form submissions

### Backend Services
- **Storage Interface**: Abstracted storage layer with in-memory implementation
- **API Routes**: RESTful endpoints (to be implemented in /api namespace)
- **Error Handling**: Centralized error middleware
- **Request Logging**: Comprehensive request/response logging for API calls

## Data Flow

1. **Client Requests**: Frontend makes API calls through TanStack Query
2. **API Processing**: Express.js routes handle business logic
3. **Data Storage**: Drizzle ORM interfaces with PostgreSQL database
4. **Response**: JSON responses sent back to client
5. **State Management**: TanStack Query caches and manages server state
6. **UI Updates**: React components re-render based on state changes

## External Dependencies

### Core Dependencies
- **Database**: Neon Database (serverless PostgreSQL)
- **UI Components**: Radix UI primitives
- **Styling**: Tailwind CSS framework
- **Icons**: Lucide React icon library
- **Date Handling**: date-fns library

### Development Tools
- **TypeScript**: Type safety across the entire stack
- **ESBuild**: Fast bundling for production backend
- **PostCSS**: CSS processing with Tailwind
- **Drizzle Kit**: Database schema management

## Deployment Strategy

### Development Environment
- **Runtime**: Replit with Node.js 20 and PostgreSQL 16 modules
- **Dev Server**: Vite dev server with HMR at port 5000
- **Database**: Automatic PostgreSQL provisioning via DATABASE_URL

### Production Build
- **Frontend**: Vite builds static assets to `dist/public`
- **Backend**: ESBuild bundles server code to `dist/index.js`
- **Deployment**: Replit autoscale deployment target
- **Port Configuration**: Internal port 5000 mapped to external port 80

### Build Process
1. `npm run build` - Builds both frontend and backend
2. Frontend assets compiled to `dist/public`
3. Backend bundled as ESM module
4. Static file serving handled by Express in production

## Changelog

```
Changelog:
- June 23, 2025. Initial setup
- June 23, 2025. Updated with official AJP Services logo and real project images from company website
- June 23, 2025. Replaced all images with authentic project photos from AJP Services portfolio including kitchen, bathroom, and commercial projects
- June 23, 2025. Added project detail pages with complete information for each project
- June 23, 2025. Updated social media links with real Instagram and added WhatsApp contact button
- June 24, 2025. Fixed corrupted files and translation system issues
- June 24, 2025. Implemented comprehensive technical optimizations:
  * PWA functionality with service worker and manifest
  * Advanced lazy loading and image optimization
  * Custom cursor with hover effects
  * Exit-intent modal for lead capture
  * Enhanced animations with intersection observer
  * Google Analytics and Facebook Pixel integration
  * Comprehensive SEO with schema markup
  * Intelligent caching strategies
  * Offline functionality
- June 24, 2025. Final optimizations and content curation:
  * Removed unwanted projects ("Cocina Residencial Elegante", "Baño Principal - Mármol Premium", project IDs 6 and 12)
  * Implemented custom construction tool cursors for header (hammer and wrench icons)
  * Added rotating animations to service icons (marble, quartz, granite, porcelain)
  * Fixed cursor z-index conflicts with modals
  * Cleaned up translation files and removed unused project references
  * Conducted comprehensive code review and error cleanup
  * Replaced globe icon with wrench tool in language selector for visual consistency
  * READY FOR PRODUCTION DEPLOYMENT
- June 24, 2025. Vercel deployment preparation:
  * Created vercel.json configuration for static site deployment
  * Added comprehensive deployment guide in Spanish
  * Set up environment variables template
  * Configured build commands for Vercel platform
  * READY FOR VERCEL DEPLOYMENT
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```