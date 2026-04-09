# JSON:API Tree Browser

Interactive single-page app to paste a [JSON:API](https://jsonapi.org/) document and browse its entity tree.

**Live:** https://jsonapi-browser.pages.dev/

## Features

- Entity tree view starting from the root resource(s)
- Relationships are resolved recursively from `included` resources
- Circular references are detected and marked
- Stats bar showing primary, included, total resource counts and type breakdown
- Example payload included for quick testing

## Deployment

The app is hosted as a Cloudflare Page. Deployment is currently manual:

```sh
npx wrangler pages deploy . --project-name jsonapi-browser
```

Wrangler will prompt for the account interactively if multiple are available.
