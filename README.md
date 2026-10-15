# 503.party
## Cloudflare hosting

Native Git publishes gh-pages with npm ci, npm run build, npm run test:hosting,
and npm run deploy. Credentials stay in Cloudflare; previews are disabled. The
existing public files and Pages recovery remain. orcas.gif exceeds the25MiB
static-file limit, so native builds split it into content-addressed16MiBassets.
A typed Worker streams its unchanged URL/bytes, with full/Range/HEAD/ETag/CORS
behavior checked in the real local Worker runtime. No R2 credential is required.
