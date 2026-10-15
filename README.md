# Astro Tailwind Starter

A minimal, production-ready starter for building static sites with Astro and Tailwind CSS.

## Features

- Astro 7
- Tailwind CSS 4 through the official Vite plugin
- A reusable, typed page layout
- Prettier formatting for Astro files
- Automatic Tailwind class sorting
- Project-level VS Code formatting settings
- pnpm with a committed lockfile

## Requirements

- Node.js 22.12 or later
- pnpm 10.33.0

## Getting Started

Create a repository from this template using **Use this template** on GitHub, then clone your new repository.

```sh
corepack enable
pnpm install
pnpm dev
```

The development server will be available at `http://localhost:4321`.

## Commands

Run all commands from the project root:

| Command                | Action                                  |
| :--------------------- | :-------------------------------------- |
| `pnpm install`         | Install dependencies                    |
| `pnpm dev`             | Start the local development server      |
| `pnpm build`           | Build the production site to `dist/`    |
| `pnpm preview`         | Preview the production build locally    |
| `pnpm format`          | Format the project with Prettier        |
| `pnpm format:check`    | Check formatting without changing files |
| `pnpm astro -- --help` | Display the Astro CLI commands          |

## Project Structure

```text
/
├── public/
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
└── pnpm-lock.yaml
```

Astro creates routes from files in `src/pages/`. Shared document markup and metadata live in `src/layouts/Layout.astro`, while Tailwind is loaded from `src/styles/global.css`.

## Formatting

The repository includes Prettier, the Astro Prettier plugin, and the Tailwind CSS Prettier plugin. Saving an Astro file in VS Code formats the document and sorts Tailwind classes automatically.

Install the workspace's recommended extensions when VS Code prompts you, or install these extensions manually:

- [Astro](https://marketplace.visualstudio.com/items?itemName=astro-build.astro-vscode)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

`prettier-plugin-astro` is currently pinned to `0.14.1` to preserve Tailwind class sorting compatibility. Verify Astro and Tailwind Prettier plugin compatibility before upgrading it.

## Customize the Starter

Before deploying your site:

1. Update the title and description in `src/pages/index.astro`.
2. Replace the example page content.
3. Replace the favicon files in `public/`.
4. Update the package name in `package.json`.

## Documentation

- [Astro documentation](https://docs.astro.build)
- [Tailwind CSS documentation](https://tailwindcss.com/docs)
- [Prettier documentation](https://prettier.io/docs/)

## License

This project is available under the [MIT License](LICENSE).
