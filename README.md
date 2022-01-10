# Nuxt 3 Teleport issue

This is a repository to demonstrate a rendering issue in Nuxt 3 when using `<teleport>`.

## Setup

Make sure to install the dependencies

```bash
yarn
```

Start the development server on http://localhost:3000

```bash
yarn dev
```

## Reproduction

1. Open localhost:3000
2. Observe that the page renders with a navigation, a header ("Page 1") and some content which resides in a `<teleport>`.
3. Click on "Page 2" in the navigation

### Expected outcome

"Page 2" is now rendered.

### Actual outcome

The route changes, but "Page 2" is not rendered. Instead, the DOM includes an empty body.

### Additional observations

1. If you remove the `<teleport>` inside `TeleportedContent.vue`, the application works as expected.
2. If you start the experiment from [/Page2](http://localhost:3000/Page2), the application works as expected (even with the `<teleport>` in place).
3. I have tried to create an app with just Vue3 and Vue Router 4. It works as expected.
