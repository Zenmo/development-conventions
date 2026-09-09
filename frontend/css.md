CSS code conventions
===

## General approach

- No preprocessor
- Prefer reusing styles through components rather than through CSS classes.

There are 2 options where to put the CSS:

### Scoped CSS

Use scoped CSS if that's native to the framework like Vue, Svelte and Astro. Use CSS variables for theming and consistency (colors, border style, fonts).

### CSS-in-JS

Use CSS-in-JS (or CSS-in-Kotlin) for React and Compose HTML. Use the host language for theming and consistency.

We currently use Emotion and Kobweb Silk.

## What to avoid

### Avoid Tailwind

Reasoning: Tailwind is a powerful tool that enables frontend experts to read and write styling faster. For programmers who occasionally do some frontend code and only know the basics it adds a layer of abstraction which they need to learn but doesn't eliminate the need to understand the underlying CSS.

This is not a blanket ban. Tailwind is well designed and it is the most popular CSS library. It is hard to avoid.

#### Guidelines if you do use Tailwind

- Be extra vigilant about keeping components small. The HTML is not semantic, so we can only go by the component name to gauge intent. Shadcn has good examples of this: [breadcrumb.tsx](https://github.com/shadcnspace/shadcnspace/blob/31dfdc30bae9db4c4da0b32d7c95ae47eaf916b4/src/components/ui/breadcrumb.tsx)
- Consider dropping down to plain CSS sometimes instead of composing ever more complex utility classes.

### Avoid CSS modules

It's simple but it places the CSS in a separate file which does not fit with a component-based approach.
