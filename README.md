# Soenneker.Shadcn.UI.Components

Generated HTML captures of shadcn/ui component previews, organized by component implementation family.

## File names

Each file uses this convention:

```text
<family>-<component>.html
```

Families currently include:

- `radix-*` for Radix-backed previews
- `base-*` for Base UI-backed previews
- `aria-*` for React Aria-backed previews

For example, `radix-button.html`, `base-button.html`, and `aria-button.html` contain the captured button previews for those three implementations. Not every component exists in every family.

## Using the captures

The files contain the preview markup rendered by the upstream component pages at generation time. They are useful for inspecting structure, attributes, accessibility state, SVG content, and utility-class differences across implementations.

They are not self-contained styled demos. The markup references utility classes and design tokens from the source site, and interactive behavior from React component libraries is not reproduced by opening an HTML file directly.

Treat generated IDs and framework-specific attributes as capture output rather than stable selectors. Prefer semantic elements, `data-slot` values, ARIA attributes, and class patterns when comparing files.

These files are refreshed by `Soenneker.Shadcn.UI.Runner`. Changes made directly to generated HTML may be replaced by a later refresh.
