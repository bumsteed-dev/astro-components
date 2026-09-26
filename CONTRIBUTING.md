# Contributing

Thanks for your interest in contributing! Every component, fix, and idea helps make this collection better for the Astro community.

## Ways to contribute

- **Suggest a component.** Open an issue describing the component and why it's useful.
- **Report a bug.** Open an issue with steps to reproduce it, what you expected, and what happened.
- **Improve an existing component.** Accessibility, performance, styling, or docs.
- **Add a new component.** See the guidelines below.

## Component guidelines

A good component in this collection is:

- **Self-contained.** One `.astro` file that works when copied into another project, with no hidden dependencies.
- **Typed.** Props are declared with `interface Props` and have sensible defaults.
- **Accessible.** Uses semantic HTML, works with the keyboard, and includes the right ARIA attributes when needed.
- **Lightweight.** No client-side JavaScript unless the component truly needs it.
- **Customizable.** Uses scoped styles and CSS custom properties so it's easy to adapt.
- **Responsive.** Looks good on mobile and desktop.

## Workflow

1. Fork the repository and create a branch from `main`:
   ```bash
   git checkout -b feat/component-name
   ```
2. Install dependencies and start the dev server:
   ```bash
   pnpm install
   pnpm dev
   ```
3. Make your changes and check that the project builds:
   ```bash
   pnpm build
   ```
4. Commit with a clear message (for example, `feat: add Accordion component`).
5. Open a pull request describing what you changed and why. Screenshots are very welcome for visual changes.

## Code of conduct

Be kind and respectful. We're all here to learn and build cool things together.
