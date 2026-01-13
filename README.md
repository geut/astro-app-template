# Astro + React + shadcn/ui Template

A modern, full-featured template for building web applications with Astro, React, and shadcn/ui components. Features a comprehensive sidebar navigation system with user management, projects, and secondary actions. Perfect for SaaS applications, dashboards, and admin panels.

## ✨ Features

- **Astro**: Static site generation with component islands
- **React**: Interactive components with React 19
- **shadcn/ui**: Beautiful, accessible UI components
- **Tailwind CSS v4**: Modern utility-first CSS framework
- **TypeScript**: Type-safe development
- **Advanced Sidebar**: Inset-style sidebar with header, collapsible navigation, and user footer
- **User Management**: Built-in user profile dropdown with account actions
- **Project Navigation**: Organized project sections with action menus
- **Modular Navigation**: Separate components for main nav, projects, secondary actions, and user profile
- **Dark Mode**: Built-in light/dark theme support
- **Lucide Icons**: Beautiful, consistent iconography

## 🚀 Quick Start

```bash
# Clone this template
bunx degit your-username/astro-shadcn-template my-project
cd my-project

# Install dependencies
bun install

# Start development server
bun run dev
```

Open [http://localhost:4321](http://localhost:4321) to see your application.

## 📁 Project Structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── ui/              # shadcn/ui components (avatar, dropdown-menu, collapsible, etc.)
│   │   ├── nav-user.tsx     # User profile dropdown navigation
│   │   ├── nav-main.tsx     # Main navigation with collapsible sections
│   │   ├── nav-secondary.tsx # Secondary navigation items
│   │   ├── nav-projects.tsx # Projects navigation with action menus
│   │   ├── app-layout.tsx   # Main layout with sidebar
│   │   └── app-sidebar.tsx  # Complete sidebar implementation
│   ├── layouts/
│   │   └── Layout.astro     # Root layout
│   ├── pages/
│   │   └── index.astro      # Home page
│   ├── styles/
│   │   └── global.css       # Global styles with Tailwind
│   ├── hooks/
│   │   └── use-mobile.ts    # Mobile detection hook
│   └── lib/
│       └── utils.ts         # Utility functions
├── astro.config.mjs          # Astro configuration
├── components.json           # shadcn/ui configuration
├── package.json
├── tailwind.config.js
└── tsconfig.json
```

## 🛠️ Tech Stack

- **Framework**: [Astro](https://astro.build/)
- **UI Components**: [shadcn/ui](https://ui.shadcn.com/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Primitives**: [Radix UI](https://www.radix-ui.com/)
- **Language**: TypeScript

## 🎨 Customization

### Adding New UI Components

Add new shadcn/ui components:

```bash
bunx shadcn@latest add button input card
```

### Theming

The template includes a comprehensive design system with CSS variables. Modify colors in `src/styles/global.css` or use the built-in theme configuration.

### Navigation Components

The template includes modular navigation components that can be easily customized:

- **NavMain**: Primary navigation with collapsible sections - edit the `data.navMain` array in `app-sidebar.tsx`
- **NavProjects**: Project-based navigation with action menus - customize the `data.projects` array
- **NavSecondary**: Secondary actions like support and feedback - modify the `data.navSecondary` array
- **NavUser**: User profile dropdown with account actions - update the `data.user` object

### Layout

The inset sidebar layout provides a professional application feel. The sidebar includes:

- Header with branding/logo
- Main content area with organized navigation sections
- Footer with user profile and actions

Modify `src/components/app-sidebar.tsx` for sidebar content and `src/components/app-layout.tsx` for the main layout structure.

## 📝 Scripts

| Command               | Description              |
| --------------------- | ------------------------ |
| `bun run dev`         | Start development server |
| `bun run build`       | Build for production     |
| `bun run preview`     | Preview production build |
| `bun run astro check` | Type check Astro files   |

## 🚀 Deployment

### Netlify

```bash
bun run build
# Upload the `dist` folder to Netlify
```

### Other Platforms

This template works with any static hosting service. Build with `bun run build` and deploy the `dist` folder.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

MIT License - see the [LICENSE](LICENSE) file for details.