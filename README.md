# Julkee x Lempee hakemus

Astro sivut ja tehty Codexilla.
Aikaa meni noin 1h 20min plus deploy noin 15min.

## Missä nään sivut?

Live versio: https://julkeexlempee.rantarepo.workers.dev/

### Omalla koneella

- Kloonaa repo
- Terminaalissa `bun install` ja `bun run dev`
- Selaimella -> `http://localhost:4321/`

## Cloudflare Workers

- Build command: `bun run build`
- Deploy command: `npx wrangler deploy`
- Root directory: `/`
- Staattisen sivuston tiedostot tulevat `dist/`-hakemistosta (`wrangler.jsonc`).
- `packageManager` pinnnaa Bunin versioon 1.4.4, joka osaa lukea nykyisen `bun.lock`-lockfilen.

Staattinen Astro-sivu ei tarvitse `@astrojs/cloudflare`-adapteria.
