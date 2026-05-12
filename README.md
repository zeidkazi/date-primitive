# Natural Language Date Picker

A high-end, open-source React Date Picker library focused on micro-animations, enterprise-grade accessibility, and Natural Language Processing (NLP) input.

## Workspace Architecture
This project is built using a Turborepo monorepo with a strict separation between core logic and shared utilities.

### Packages
- `packages/date-picker`: The core library containing the React components, headless hooks (`useNaturalDatePicker`), and UI interfaces.
- `packages/utils`: Internal shared utilities (e.g. `cn` for `clsx` + `tailwind-merge`).

### Apps
- `apps/playground`: A fast Vite + React playground to test and build the components in isolation.

## Tooling Stack
- **Build Engine**: `tsup` (outputs optimized ESM and CJS bundles)
- **Styling**: Tailwind CSS v4
- **Animations**: Motion
- **Positioning**: Floating UI
- **Linting & Formatting**: Biome
- **Git Hooks**: Lefthook

## Getting Started

1. Install all dependencies:
```sh
npm install
```

2. Start the development server (runs both the package bundler in watch mode and the playground Vite server):
```sh
npm run dev
```

3. Ensure your pre-commit hooks are active:
```sh
npx lefthook install
```
