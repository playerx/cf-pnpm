# Cloudflare Pages with PNPM

1. Set environment variable to skip the npm install phase:
   `NPM_FLAGS = --version`

2. Set environment variable to use node.js v16 (CF Pages pipeline use v12 by default)
   `NODE_VERSION = 16`

3. Set build command to (so pnpm’s store is cached too):
   `npx pnpm i --store=node_modules/.pnpm-store && npm run build`

[Reference](https://community.cloudflare.com/t/add-pnpm-to-pre-installed-cloudflare-pages-tools/288514/5)
