---
title: How to use create your page layouts in Statinamic
---

Statinamic uses React components as layouts.

By default, Statinamic might need 2 layouts:

- `Page`
- `PageError`

If you use the `statinamic/lib/PageContainer`, you will need those components in
your `pageComponents` definition
(by default, declared in `app/pageComponents.js`).

## Default page layouts that Statinamic can use

### `Page`

`Page` will be used as the default layout.
**It is required for Statinamic to work.**

[Check out the default Page and the props it got.](https://github.com/MoOx/statinamic/blob/master/src/boilerplate/web_modules/Page/index.js)

### `PageError`

`PageError` will be used as the default layout when a page has an error
(**eg: http 404 not found**).

_This layout is optional_ and a `PageContainer` contains a minimal fallback if
it is not available.

[Check out the default PageError and the props it got.](https://github.com/MoOx/statinamic/blob/master/src/boilerplate/web_modules/PageError/index.js)

### `PageLoading`

_This layout is optional_ and not in the default boilerplate. You might want to
use it to add a loader while a page is loading.
