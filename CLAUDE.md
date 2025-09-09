# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Modi landing page** - a product landing site for a multi-store e-commerce management platform. Modi allows users to manage multiple online stores from a unified interface with analytics, automation, and real-time monitoring capabilities.

## Technology Stack

- **Framework**: Astro 5.13+ with TypeScript (strict mode)
- **Styling**: Tailwind CSS 4.1+ (via Vite plugin)
- **Language**: Spanish (primary market)
- **Architecture**: Component-based Astro architecture

## Development Commands

| Command | Purpose |
|---------|---------|
| `npm install` | Install dependencies |
| `npm run dev` | Start development server at localhost:4321 |
| `npm run build` | Build production site to ./dist/ |
| `npm run preview` | Preview production build locally |
| `npm run astro ...` | Run Astro CLI commands |

## Project Structure

- `src/pages/index.astro` - Main landing page (imports all sections)
- `src/components/` - Modular landing page sections:
  - `Header.astro` - Sticky navigation with brand colors
  - `HeroSection.astro` - Main hero with video fallback
  - `FeaturesSection.astro` - Product features showcase
  - `AnalyticsSection.astro` - Analytics capabilities
  - `AutomationSection.astro` - Automation features
  - `FAQSection.astro` - Frequently asked questions
  - `WaitlistCTA.astro` - Call-to-action for waitlist signup
  - `Footer.astro` - Site footer
- `src/styles/global.css` - Global styles with brand variables

## Design System

- **Brand Color**: `#eb6517` (orange) - defined as CSS variable `--brand`
- **Typography**: Uses system fonts with antialiasing
- **Styling Approach**: Utility-first with Tailwind CSS
- **Visual Effects**: Subtle shadows via `.card-shadow` utility class
- **Responsive**: Mobile-first design patterns

## Key Implementation Details

- **Video Handling**: Hero section includes JavaScript for video autoplay with fallback image
- **Navigation**: Smooth scroll behavior with anchor links to sections
- **Accessibility**: Proper semantic HTML, focus styles using brand color
- **Performance**: Backdrop blur effects, optimized loading

## Content & Business Context

The landing page targets Spanish-speaking e-commerce businesses and showcases Modi's capabilities for:
- Multi-store management and product linking
- Real-time analytics and monitoring  
- Price automation and inventory planning
- Unified order management across platforms

## No Testing Framework

This project currently has no test setup or linting configuration beyond TypeScript strict mode.