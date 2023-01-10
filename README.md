# Cloudflare Pages with PNPM

1. Set environment variable to skip the npm install phase:
   `NPM_FLAGS = --version`

2. Set build command to (so pnpm’s store is cached too):
   `npx pnpm i --store=node_modules/.pnpm-store && npm run build`
