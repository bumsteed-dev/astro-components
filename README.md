# Astro Components

A curated collection of beautiful, copy-paste components for [Astro](https://astro.build). Built by and for the community. ✨

> [!NOTE]
> This project is in its early stages. The first components are on their way, and contributions are welcome!

## Why

Inspired by [shadcn/ui](https://ui.shadcn.com), this is **not a component library** you install as a dependency. It's a collection of well-crafted components you copy into your project and make your own.

- **Copy, paste, own it.** No packages to install and no versions to keep up with. The code lives in your project.
- **Astro-first.** Built as native `.astro` components, zero JavaScript by default, and interactive only when it's needed.
- **Easy to customize.** Scoped styles and typed props, so you can adapt each component without fighting it.
- **Community-driven.** Anyone can suggest, improve, or contribute a component.

## Usage

1. Browse the collection and pick a component.
2. Copy its `.astro` file into your project (for example, `src/components/`).
3. Import it and use it:

```astro
---
import MyComponent from "../components/MyComponent.astro";
---

<MyComponent />
```

## Running locally

Requirements: Node.js `>=22.12.0` and [pnpm](https://pnpm.io).

```bash
git clone https://github.com/bumsteed-dev/astro-components.git
cd astro-components
pnpm install
pnpm dev
```

| Command        | Action                                          |
| :------------- | :---------------------------------------------- |
| `pnpm install` | Install dependencies                            |
| `pnpm dev`     | Start the dev server at `localhost:4321`        |
| `pnpm build`   | Build the site to `./dist/`                     |
| `pnpm preview` | Preview the production build locally            |

## Contributing

Contributions are welcome, whether it's a new component, a bug fix, or an idea. Check out the [contributing guide](CONTRIBUTING.md) to get started.

## License

[MIT](LICENSE) © Jesús Cedeño Vélez
