# Static hosting

Preserve the existing public HTML, images and audio and the gh-pages recovery
source. Native Cloudflare Git builds publish gh-pages with credentials held in
Cloudflare and previews off. Run npm ci, npm run check:deploy and npm run
test:hosting before publishing. orcas.gif is streamed from generated16MiBchunks;
its original URL, digest, MIME and Range behavior must remain. Generated manifests,
chunks and types stay ignored. Never add Cloudflare secrets to GitHub.
