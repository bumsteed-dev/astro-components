# Astro Components

A curated collection of beautiful, accessible, copy-paste components for [Astro](https://astro.build). Built by and for the community.

**Website:** [ui.bumsteed.dev](https://ui.bumsteed.dev)

> [!IMPORTANT]
> **This project is just getting started.** There are no components available yet, and the structure, guidelines, and conventions described here may change as the project takes shape. Feedback, ideas, and early contributions are very welcome.

## Table of contents

- [About](#about)
- [Principles](#principles)
- [How it works](#how-it-works)
- [Using a component](#using-a-component)
- [Customizing components](#customizing-components)
- [Local development](#local-development)
- [Project structure](#project-structure)
- [Tech stack](#tech-stack)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [FAQ](#faq)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## About

Astro Components is an open collection of UI components designed specifically for Astro projects. The goal is to offer a place where the community can find, share, and improve components that are genuinely useful in real-world sites: landing pages, blogs, portfolios, documentation, and more.

Inspired by [shadcn/ui](https://ui.shadcn.com), this is **not a component library you install as a dependency**. Each component is a standalone file that you copy into your project and adapt as you see fit. Once it's in your codebase, it's yours.

## Principles

Every component in this collection aims to be:

| Principle           | What it means                                                                                           |
| :------------------ | :------------------------------------------------------------------------------------------------------ |
| **Self-contained**  | A single `.astro` file with no hidden dependencies. Copy it and it works.                               |
| **Astro-first**     | Built as native Astro components. Zero client-side JavaScript by default, interactive only when needed. |
| **Accessible**      | Semantic HTML, keyboard support, and the right ARIA attributes where they apply.                        |
| **Typed**           | Props are declared with TypeScript and have sensible defaults.                                          |
| **Customizable**    | Scoped styles and CSS custom properties, so you can adapt a component without fighting it.              |
| **Responsive**      | Designed to look good on any screen size.                                                               |

## How it works

Traditional component libraries are distributed as packages. That makes them easy to install but hard to customize: you depend on their API, their styling decisions, and their release cycle.

This project takes a different approach:

1. **Browse** the collection on the website and preview each component.
2. **Copy** the source code of the component you need.
3. **Paste** it into your project.
4. **Adapt** it however you like. There's nothing to update and nothing to break.

## Using a component

1. Pick a component from the [website](https://ui.bumsteed.dev) or from the source in this repository.
2. Copy its `.astro` file into your project, for example into `src/components/`.
3. Import it and use it in any page or layout:

```astro
---
import Card from "../components/Card.astro";
---

<Card title="Hello, Astro">
  <p>Any content you want inside the card.</p>
</Card>
```

> `Card` is used here only as an example of the usage pattern. See the website for the components that are actually available.

## Customizing components

Since the code lives in your project, you can change anything. For quick adjustments, components are designed to expose their main design values as CSS custom properties:

```astro
<Card title="Custom card" style="--card-radius: 1rem; --card-padding: 2rem;" />
```

For deeper changes, edit the component file directly: its markup, styles, and props are all yours.

## Local development

To run the website and work on components locally.

### Requirements

- [Node.js](https://nodejs.org) `>=22.12.0`
- [pnpm](https://pnpm.io)

### Setup

```bash
git clone https://github.com/bumsteed-dev/astro-components.git
cd astro-components
pnpm install
pnpm dev
```

The site will be available at `http://localhost:4321`.

### Commands

| Command        | Action                                                   |
| :------------- | :------------------------------------------------------- |
| `pnpm install` | Install dependencies                                     |
| `pnpm dev`     | Start the dev server at `localhost:4321`                 |
| `pnpm build`   | Build the production site to `./dist/`                   |
| `pnpm preview` | Preview the production build locally                     |
| `pnpm astro`   | Run Astro CLI commands (`astro add`, `astro check`, ...) |

## Project structure

```text
astro-components/
├── docs/               # Additional project documentation
├── public/             # Static assets served as-is
├── src/
│   ├── layouts/        # Shared page layouts
│   └── pages/          # Website pages (file-based routing)
├── astro.config.mjs    # Astro configuration
├── CONTRIBUTING.md     # Contribution guide
├── LICENSE             # MIT license
└── package.json
```

As the project grows, components will live in `src/components/` and each one will have its own demo page on the website.

## Tech stack

- [Astro](https://astro.build) for the components and the website
- [TypeScript](https://www.typescriptlang.org) for typed props
- [pnpm](https://pnpm.io) as the package manager
- [Vercel](https://vercel.com) for hosting and deployments
- [Vercel Web Analytics](https://vercel.com/docs/analytics) for privacy-friendly, cookie-free page view statistics on the website

## Roadmap

- [x] Project setup, license, and contribution guide
- [ ] Base layout and design for the website
- [ ] First set of components
- [ ] Gallery page with previews of every component
- [ ] Individual demo page for each component, with its source code ready to copy
- [ ] Light and dark mode support
- [ ] Search and filtering by category

Have an idea for the roadmap? [Open an issue](https://github.com/bumsteed-dev/astro-components/issues).

## Contributing

Contributions of all sizes are welcome: new components, bug fixes, accessibility improvements, documentation, or simply ideas.

- **Suggest a component** or **report a bug** by [opening an issue](https://github.com/bumsteed-dev/astro-components/issues).
- **Contribute code** by opening a pull request. Please read the [contributing guide](CONTRIBUTING.md) first; it explains the component guidelines and the workflow.

## FAQ

**Is this an npm package?**
No. There is nothing to install. You copy the components you need into your own project.

**Can I use these components in commercial projects?**
Yes. Everything is released under the MIT license. Attribution is appreciated but not required.

**Do I need React, Vue, or another framework?**
No. Components are written as native `.astro` files. If a component ever requires a framework or extra dependency, it will be clearly stated.

**Which versions of Astro are supported?**
Components are built and tested against the latest version of Astro. Most of them should also work with recent previous versions.

## Acknowledgements

- [shadcn/ui](https://ui.shadcn.com) for popularizing the copy-paste approach to components.
- The [Astro](https://astro.build) team and community for building such a great framework.

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 Jesús Cedeño Vélez.
