# Next.js App Starter

A modern, production-ready Next.js starter template with TypeScript, Tailwind
CSS, and essential development tools pre-configured.

---

## Tech Stack

- **Framework:** [Next.js](https://nextjs.org) 15+ with App Router
- **Language:** TypeScript
- **Styling:** [Tailwind CSS](https://tailwindcss.com/) v4
- **Fonts:** [Geist](https://vercel.com/font) (Sans & Mono)
- **Linting & Formatting:** ESLint, Prettier
- **Git Hooks:** Husky + lint-staged

---

## Getting Started

**Prerequisites:**

- Node.js v22.13+
- yarn (recommended)

**Quick Start:**

1. **Clone the repository:**
```bash
git clone https://github.com/manask-pradhan/next-app-starter.git my-next-app
```

2. **Navigate to the project:**
```bash
cd my-next-app
```

3. **Install dependencies:**
```bash
yarn install
```

4. **Start development server:**
```bash
yarn dev
```

5. **Open your browser:**
Visit [http://localhost:3000](http://localhost:3000) to see your app!

Open [http://localhost:3000](http://localhost:3000) in your browser. The page
auto-updates as you edit `src/app/page.tsx`.

---

## Project Structure / Architecture

```
src
├── app               # Next.js app directory
│   ├── page.tsx      # Root home page, URL: /
│   ├── dashboard     # Dashboard page
│   │   └── page.tsx  # URL: /dashboard
│   ├── profile       # Profile page
│   │   └── page.tsx  # URL: /profile
│   └── api           # API routes (Next.js serverless functions)
│       └── products.ts # URL: /api/products
├── components        # All React components
│   ├── commons        # Reusable components (Button, Header, Input, etc.)
│   └── PageSpecific   # Page-specific components
├── hooks             # Custom hooks
├── utils             # Utility functions used across the project
├── constants         # Project-level constants
├── translations      # Translation files (en.json, etc.)
└── lib               # Third-party library initialization or overrides
```

**Best Practices:**

- Keep files at the closest scope to their usage.
- Name components and folders semantically using PascalCase.
- Use `index.ts` or `index.tsx` in component folders to consolidate exports.
- Default export single components, use named exports for multiple exports.
- Group multiple related states inside objects; update them functionally.
- Keep `useState` hooks at the top, followed by other hooks.
- Destructure props and API responses for cleaner, maintainable code.
- Avoid unnecessary `div`s and return single components directly.
- Use template literals, self-closing tags, and object literals for conditional
  rendering.
- Place API routes inside `app/api` folder per Next.js conventions.
- Check this
  [article](https://courses.bigbinaryacademy.com/learn-react/miscellaneous/structuring-code/)
  for more details.

---

## Available Scripts

| Script         | Description                          |
| -------------- | ------------------------------------ |
| `dev`          | Runs the app in development mode     |
| `build`        | Builds the app for production        |
| `start`        | Runs the production server           |
| `lint`         | Runs ESLint to check code style      |
| `format`       | Formats code using Prettier          |
| `format:check` | Checks if code is properly formatted |

---

## Editor & Tooling Setup

- **VSCode Extensions:** ESLint, Prettier, Tailwind CSS IntelliSense
- **Pre-commit hooks:** Husky + lint-staged
- **EditorConfig:** Enforces consistent editor settings
- **Node Version & Package Manager:** Specified in `.nvmrc` / `.node-version`
  and lockfile

---

## Contributing

Please refer to [CONTRIBUTING.md](CONTRIBUTING.md) for coding standards, PR
guidelines, and contribution workflow.

---

## Deployment

- **Vercel** (Recommended): Zero-config deployment for Next.js
- **Netlify**: Great for static sites and SSG
- **Railway/Render**: For full-stack applications
- See
  [Next.js deployment docs](https://nextjs.org/docs/app/building-your-application/deploying)
  for more options

---

## Useful Resources

- [Next.js Documentation](https://nextjs.org/docs) - Learn about Next.js
  features and API
- [Learn Next.js](https://nextjs.org/learn) - Interactive Next.js tutorial
- [Tailwind CSS](https://tailwindcss.com/docs) - Utility-first CSS framework
- [TypeScript](https://www.typescriptlang.org/docs) - JavaScript with syntax for
  types
