<div align="center">
   <img width="125" src="logo.png" alt="Logo">
</div>

<div align="center">
  <h1><b>Gelato</b></h1>
  <p><i>Jellyfin Stremio Integration Plugin</i></p>
</div>

Bring the power of Stremio addons directly into Jellyfin. This plugin replaces Jellyfin’s default search with Stremio-powered results and can automatically import entire catalogs into your library through scheduled tasks, seamlessly injecting them into Jellyfin’s database so they behave like native items.

 <a href="https://discord.gg/rEbhk4RBhs">
    <img src="https://img.shields.io/badge/Talk%20on-Discord-brightgreen">
</a>

### Features
- **Unified Search** – Jellyfin search now pulls results from Stremio addons
- **Catalogs** – Import items from stremio catalogs into your library with scheduled tasks
- **Realtime Streaming** – Streams are resolved on demand and play instantly
- **Database Integration** – Stremio items appear like native Jellyfin items
- **Act as an proxy** - Streams are proxied through Jellyfin, so debrid sees everything as a single IP.
- **Per user settings** - Users can have their own manifest, perfect for age restricted accounts.
- **More Content, Less Hassle** – Expand Jellyfin with community-driven Stremio catalogs

## Usage

### Uso con plugins de la comunidad

1. Configura tu addon de Stremio favorito:
   - **Torrentio**: `https://torrentio.strem.fun/{tu-config}/manifest.json`
   - **Comet**: `https://comet.elfhosted.com/manifest.json` (o tu instancia self-hosted)
   - **MediaFusion**: `https://mediafusion.elfhosted.com/manifest.json`
   - **Orion**: `https://orion.elfhosted.com/manifest.json`
   - Cualquier otro: usa su URL de manifest (normalmente termina en `/manifest.json`)

2. En Jellyfin → Plugins → Gelato → Settings:
   - Pega la URL del manifest del addon que quieras.
   - Puedes tener un manifest diferente por usuario (ideal para cuentas con restricciones de edad).

3. Añade las rutas configuradas a tu librería de Jellyfin y haz scan.
   
## Notes

- Ahora soporta **cualquier addon de Stremio** (Torrentio, Comet, MediaFusion, Orion, etc.)
- **P2P currently in beta**

### FAQ

- You need to restart the server after editing the manifest/config in aiostreams.
- You should have at least one search enabled catalog. I suggest the tmdb addon.
- if something borked or you want to start over, you can use the purge task under scheduled tasks.
- I suggest lowering the default timeout on your stremio addons in aiostreams (5 seconds for example)
- debridio tmdb and debridio tvdb are pronlematic. I suggest using the regular tmdb addon.
- Stream cache can be cleared by restarting the server
