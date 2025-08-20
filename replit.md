# replit.md

## Overview

This is a Facebook Login Server - a lightweight Express.js application that serves a Facebook login interface with a clean, responsive design. The project provides a standalone implementation extracted from the Niceplace application, featuring a simple server that serves static HTML content mimicking Facebook's login page design and functionality.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Static HTML Interface**: Single-page application using vanilla HTML, CSS, and JavaScript
- **Responsive Design**: Mobile-first approach with viewport meta tags and CSS media queries
- **Facebook UI Replication**: Authentic Facebook styling using custom CSS that mimics Facebook's color scheme (#1877f2 blue, #f0f2f5 background)
- **Form Handling**: Client-side form validation and submission handling

### Backend Architecture
- **Express.js Server**: Lightweight Node.js web server running on port 5000
- **Static File Serving**: Serves HTML, CSS, and other static assets from the root directory
- **CORS Configuration**: Cross-origin resource sharing enabled for all origins
- **Request Logging**: Comprehensive logging middleware for debugging and monitoring
- **Health Check Endpoint**: `/health` endpoint for deployment platform monitoring

### Server Configuration
- **Port Management**: Configurable port via environment variable (defaults to 5000)
- **Static Asset Serving**: Express static middleware serving files from project root
- **JSON Body Parsing**: Built-in middleware for handling JSON and URL-encoded request bodies
- **Development vs Production**: Environment-aware configuration

### Deployment Architecture
- **Multi-Platform Support**: Configured for Vercel, Heroku, Digital Ocean, and AWS deployment
- **Docker Ready**: Includes deployment package structure for containerization
- **Dual Package Configuration**: Separate package.json files for Replit vs external deployments
- **Health Monitoring**: Built-in health check endpoint for platform monitoring

## External Dependencies

### Core Dependencies
- **express**: Version 5.1.0 - Web application framework for Node.js
- **cors**: Version 2.8.5 - Cross-origin resource sharing middleware
- **tsx**: Version 4.19.3 - TypeScript execution and build tool

### Development Tools
- **Node.js**: Runtime environment (minimum version 14.x required)
- **npm**: Package manager (minimum version 6.x required)

### Deployment Platforms
- **Vercel**: Configured with vercel.json for serverless deployment
- **Heroku**: Ready for Heroku deployment with Procfile configuration
- **Digital Ocean**: Manual server deployment support
- **AWS Elastic Beanstalk**: Cloud platform deployment ready
- **Docker**: Container deployment support

### External Services Integration
- **Telegram Integration**: Mentioned in README for login notifications (implementation details not visible in current codebase)

### File System Dependencies
- Static asset serving from local file system
- Runtime file existence checks for index.html
- Path resolution using Node.js path module