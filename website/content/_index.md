---
title: "AI Code Terminal: Self-Hosted Development Environment"
description: "A lightweight, terminal-centric web IDE with integrated file explorer, code editor, advanced terminal multiplexing, process management, and AI assistance. Self-hosted for complete privacy and control."
hero:
  title: "Terminal-First Web IDE"
  subtitle: "Lightweight development environment combining the power of a full-featured IDE with terminal simplicity. Integrated file explorer, CodeMirror editor, split-pane terminals, and AI assistance—all self-hosted for complete control."
  cta_primary:
    text: "Get Started"
    url: "/docs/getting-started/"
    icon: "book-open"
  cta_secondary:
    text: "View Source Code"
    url: "https://github.com/drmhse/ai-code-terminal"
    icon: "code"
---

# Terminal-First Development Environment

AI Code Terminal bridges the gap between a simple shell and a full-featured IDE, providing essential development tools without the bloat. Professional-grade terminal multiplexing, integrated file management, built-in code editor, and AI assistance—all while maintaining complete privacy through self-hosting.

## Core Features

### Integrated File Explorer & Code Editor
**Visual code navigation with built-in editing.** Full-featured file browser in the sidebar for intuitive project navigation. Built-in CodeMirror 6 editor with syntax highlighting for 15+ languages (JavaScript, Python, Go, Rust, Java, CSS, HTML, SQL, and more). Edit code directly in the browser with modern editor features.

### Advanced Terminal Multiplexing
**Professional terminal management.** Create multiple terminal tabs per workspace with sophisticated split-pane layouts (horizontal, vertical, grid). Advanced session management includes command history, process tracking, and synchronized file operations. Each session persists across browser refreshes and network disconnections, ensuring your work never gets interrupted.

### Long-Running Process Management
**Intelligent process supervision.** Automatically detect and track long-running commands like development servers and build processes. View, stop, and restart processes through the integrated interface with optional auto-recovery for crashed processes.

### System Resource Monitoring
**Real-time development insights.** Status bar displays active sessions, CPU usage, memory consumption, and workspace storage. Container-aware monitoring shows Docker resource utilization and limits for complete environment visibility.

### Enterprise-Grade Security
**Secure, isolated development.** Full shell access within security-hardened Docker containers running as non-root user. Single-tenant GitHub OAuth authentication ensures only authorized users can access your environment.

### Mobile-First Experience
**Professional development on any device.** Advanced mobile terminal interface with modifier key support, command presets, and touch-optimized controls. Transform tablets and phones into viable development machines.

### AI-Native Workflow
**Seamless AI integration.** Claude Code comes pre-installed and ready to use. Perfect integration with CLI-based AI tools while maintaining complete control over your API keys and interactions.

### Enhanced Session Recovery
**Uninterrupted development flow.** Advanced session management survives network interruptions and browser refreshes. Persistent workspaces maintain your development state across connections.

### Professional Theme Selection
**Customizable visual environment.** Choose from 18 carefully crafted terminal themes with live preview in an elegant modal interface. Themes include popular options like Tokyo Night, Dracula, and custom variants, ensuring consistent styling across terminals, file explorer, code editor, and all interface elements.

## Privacy and Control

### Self-Hosted Architecture
This is not a cloud service—it's software you run on your own infrastructure. Every component runs locally under your control, ensuring your code, credentials, and AI interactions remain completely private.

### Single-Tenant Security
Designed for individual developers. Each installation serves exactly one authorized GitHub user, eliminating multi-user complexity and security concerns. Your development environment is yours alone.

### Open Source Transparency
The entire codebase is open source and auditable. No hidden features, no secret data collection, no vendor lock-in. You can inspect, modify, and extend every aspect of the system.

## Technical Advantages

### Container Isolation
Runs in secure Docker containers with resource limits, read-only filesystems, and non-root execution. Your development environment is isolated from the host system for maximum security.

### Real-Time Performance
WebSocket-powered terminal sessions provide near-native performance with real-time input/output. Advanced terminal features like resizing, scrollback, and session recovery work seamlessly.

### Modern Web Technologies
Built with Vue.js 3, Express.js, Socket.IO, and CodeMirror 6 for reliability and performance. Uses Prisma with SQLite for lightweight data persistence, node-pty for terminal sessions, and modern JavaScript throughout.

## Deployment Options

### Local Development
Perfect for personal use on your laptop or desktop. Quick Docker setup gets you running in minutes. Access your local development environment from mobile devices on the same network.

### VPS Deployment
Deploy to any VPS provider for true anywhere development. Full mobile accessibility with advanced touch controls makes it practical to code from tablets and phones while maintaining professional-grade capabilities.

### Corporate/Team Use
Self-hosted architecture makes it ideal for organizations requiring complete control over their development infrastructure and data.

## Quick Start

### Using Docker Hub (Recommended)
1. **Download configuration files** from the repository
2. **Set up GitHub OAuth** application for authentication  
3. **Configure your environment** with GitHub credentials and authorized username
4. **Start with pre-built image** - `docker-compose up -d`
5. **Access via browser** at `http://your-server:3014`

### Building from Source (Advanced)
1. **Clone repository** - `git clone https://github.com/drmhse/ai-code-terminal.git`
2. **Configure environment** - Copy `env.example` to `.env` and edit
3. **Build and start** - `docker-compose -f app/docker-compose-dev.yml up -d --build`

Setup takes about 5 minutes with Docker Hub or 10 minutes building from source. Provides a complete development environment accessible from any device while maintaining complete privacy and control.