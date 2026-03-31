<div align="center">
   <img width="125" src="logo.png" alt="Logo">
</div>

<div align="center">
  <h1><b>RodriGelato Community</b></h1>
  <p><i>Jellyfin Stremio Integration Plugin - Versión Comunidad</i></p>
</div>

**Trae el poder de CUALQUIER addon de Stremio directamente a Jellyfin.**  
Este plugin reemplaza la búsqueda de Jellyfin con resultados de Stremio y permite importar catálogos completos a tu librería.

### ✅ Ahora soporta:
- Torrentio
- Comet
- MediaFusion
- Orion
- StremThru
- CUALQUIER addon que tenga `/manifest.json`
- **AIOStreams** (sigue funcionando si lo prefieres)

### Uso (muy simple)

1. Elige tu addon favorito y copia su **URL del manifest**:
   - Torrentio → `https://torrentio.strem.fun/manifest.json`
   - Comet → `https://comet.elfhosted.com/manifest.json` (o tu instancia)
   - MediaFusion → `https://mediafusion.elfhosted.com/manifest.json`
   - Orion → `https://orion.elfhosted.com/manifest.json`
   - Cualquier otro: la URL que termine en `/manifest.json`

2. En Jellyfin → Plugins → Gelato Community → Settings:
   - Pega la URL del manifest.
   - (Opcional) Puedes poner un manifest diferente por usuario.

3. Añade las rutas configuradas a tu librería y haz scan.

4. ¡Listo! Busca y reproduce al instante.

**AIOStreams sigue 100% compatible** si quieres usarlo como agregador.

---

### Instalación del plugin

Añade este repositorio en Jellyfin:

https://raw.githubusercontent.com/sdd212013-rgb/RodriGelato/gh-pages/repository.json
