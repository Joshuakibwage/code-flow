# CodeFlow AI 🚀

A modern, feature-rich landing page for CodeFlow AI – an intelligent development tool powered by advanced AI that accelerates your coding workflow.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![React](https://img.shields.io/badge/React-19.2.0-blue)
![Vite](https://img.shields.io/badge/Vite-7.2.4-646cff)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-4.1.18-06b6d4)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Available Scripts](#available-scripts)
- [Components](#components)
- [Development](#development)
- [Build & Deployment](#build--deployment)
- [Customization](#customization)
- [License](#license)

## 🎯 Overview

CodeFlow AI is a next-generation development assistant that leverages artificial intelligence to enhance your coding experience. This landing page showcases the platform's capabilities, pricing options, customer testimonials, and features in a modern, interactive design.

Built with cutting-edge web technologies, the site delivers a smooth user experience with:
- **Interactive hero section** with live code examples
- **Responsive design** optimized for all devices
- **Smooth animations** and visual feedback
- **Performance-optimized** with Vite
- **Modern styling** using TailwindCSS

## ✨ Features

### Core Features
- **AI Code Completion** – Intelligent suggestions powered by advanced AI that learns from your coding patterns
- **Automated Testing** – Generate comprehensive test suites automatically with edge case coverage
- **Smart Debugging** – AI-powered error detection and resolution suggestions
- **Real-time Assistance** – Syntax, logic, and best practice guidance built into your workflow

### Website Features
- 📱 **Fully Responsive Design** – Works seamlessly on desktop, tablet, and mobile
- ✨ **Smooth Animations** – Interactive elements with engaging transitions
- 🎨 **Modern UI/UX** – Beautiful gradient effects and glassmorphism designs
- 📊 **Pricing Plans** – Three-tier pricing structure (Starter, Professional, Enterprise)
- 💬 **Testimonials Section** – Real user feedback and success stories
- 🔗 **Sticky Navigation** – Smart navbar that adapts on scroll
- 🌙 **Dark Theme** – Eye-friendly dark mode with blue/cyan accents

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Framework** | [React 19.2.0](https://react.dev) |
| **Build Tool** | [Vite 7.2.4](https://vitejs.dev) |
| **Styling** | [TailwindCSS 4.1.18](https://tailwindcss.com) |
| **Icons** | [Lucide React 0.563.0](https://lucide.dev) |
| **Code Highlighting** | [react-syntax-highlighter 16.1.0](https://github.com/react-syntax-highlighter) |
| **Linting** | ESLint 9.39.1 |
| **Package Manager** | npm |

## 🚀 Getting Started

### Prerequisites
- **Node.js** – Version 16 or higher
- **npm** – Version 7 or higher (or yarn, pnpm)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Joshuakibwage/code-flow.git
   cd code-flow
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:5173`

### Quick Start
```bash
# Install dependencies
npm install

# Run development server with HMR
npm run dev

# Build for production
npm build

# Preview production build
npm run preview

# Run ESLint
npm run lint
```

## 📂 Project Structure

```
code-flow/
├── src/
│   ├── components/
│   │   ├── Navbar.jsx          # Navigation header with scroll detection
│   │   ├── Hero.jsx             # Hero section with code examples
│   │   ├── Features.jsx         # Feature showcase with code snippets
│   │   ├── Pricing.jsx          # Pricing plans comparison
│   │   ├── Testimonials.jsx     # User testimonials carousel
│   │   └── Footer.jsx           # Footer with links and info
│   ├── data/
│   │   └── CodeExamples.js      # Code examples and floating cards data
│   ├── App.jsx                  # Main app component
│   ├── main.jsx                 # Entry point
│   └── index.css                # Global styles
├── public/                       # Static assets
├── package.json                 # Project dependencies
├── vite.config.js               # Vite configuration
├── eslint.config.js             # ESLint configuration
├── index.html                   # HTML template
└── README.md                    # This file
```

## 📜 Available Scripts

### Development
```bash
npm run dev
```
Starts the development server with Hot Module Replacement (HMR) enabled. Changes are reflected instantly in the browser.

### Build
```bash
npm run build
```
Creates an optimized production build in the `dist/` directory. Includes minification and code splitting.

### Preview
```bash
npm run preview
```
Previews the production build locally before deployment.

### Linting
```bash
npm run lint
```
Runs ESLint to check code quality and formatting issues.

## 🧩 Components

### Navbar
- Sticky navigation that adapts based on scroll position
- Links to all sections
- Responsive mobile menu support

### Hero
- Interactive background with mouse position tracking
- Live code examples with syntax highlighting
- Animated badges and call-to-action buttons

### Features
- Three main feature cards with code snippets
- Alternating left/right layout
- Syntax-highlighted code examples

### Pricing
- Three pricing tiers with feature comparison
- "Most Popular" highlight for Professional plan
- Feature lists with checkmarks

### Testimonials
- Customer success stories and feedback
- Carousel-style presentation

### Footer
- Links and company information
- Contact details
- Social media links (configurable)

## 🎨 Development

### Styling Approach
The project uses **TailwindCSS** for utility-first styling:
- Dark theme with slate-950 background
- Blue and cyan accent colors
- Responsive spacing and sizing

### Color Scheme
```css
Primary Background: slate-950
Primary Accent: blue-400 to blue-500
Secondary Accent: cyan-400 to cyan-500
Text: white with opacity variants
```

### Adding New Sections
To add a new section to the landing page:

1. Create a new component in `src/components/`
2. Import it in [App.jsx](src/App.jsx)
3. Add it to the render chain
4. Style using TailwindCSS utilities

Example:
```jsx
// src/components/YourSection.jsx
export default function YourSection() {
  return (
    <section className="relative py-20 px-4 sm:px-6 lg:px-8">
      {/* Your content */}
    </section>
  );
}
```

### Modifying Code Examples
Code examples are stored in [src/data/CodeExamples.js](src/data/CodeExamples.js). Update this file to change displayed code snippets throughout the site.

## 🏗️ Build & Deployment

### Production Build
```bash
npm run build
```

This creates an optimized build in the `dist/` directory ready for deployment.

### Deployment Options

#### Vercel (Recommended)
```bash
npm install -g vercel
vercel
```

#### Netlify
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod --dir=dist
```

#### Traditional Hosting
Upload the contents of the `dist/` directory to your web server.

### Performance Optimizations
- Code splitting via Vite
- TailwindCSS purging unused styles
- Image optimization (use WebP format)
- Lazy loading components (can be added)

## 🔧 Customization

### Updating Content
- **Copy**: Edit component JSX files directly
- **Code Examples**: Modify [src/data/CodeExamples.js](src/data/CodeExamples.js)
- **Colors**: Update TailwindCSS class names (search for `blue-` and `cyan-`)
- **Fonts**: Configure in TailwindCSS or import custom fonts in [src/index.css](src/index.css)

### Environment Variables
Create a `.env.local` file for environment-specific configuration:
```env
VITE_API_URL=https://api.codeflow.ai
VITE_APP_NAME=CodeFlow AI
```

Access in components:
```jsx
const apiUrl = import.meta.env.VITE_API_URL;
```

### TypeScript Migration
To convert to TypeScript:
1. Rename `.jsx` files to `.tsx`
2. Add type annotations
3. Install TypeScript: `npm install -D typescript`
4. Create `tsconfig.json`

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License – see the LICENSE file for details.

## 📞 Support

For questions or issues:
- Open an issue on GitHub
- Check existing documentation
- Review code comments for implementation details

## 🔗 Resources

- [React Documentation](https://react.dev)
- [Vite Documentation](https://vitejs.dev)
- [TailwindCSS Documentation](https://tailwindcss.com)
- [Lucide Icons](https://lucide.dev)

---

**Built with ❤️ by the Joshua Kibwage**
