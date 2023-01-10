# Cloudflare Pages with PNPM

1. Set environment variable to skip the npm install phase:
   `NPM_FLAGS = --version`

2. Set environment variable to use node.js v16, by default it CF pipeline uses v12
   `NODE_VERSION = 14`

3. Set build command to (so pnpm’s store is cached too):
   `npx pnpm i --store=node_modules/.pnpm-store && npm run build`
