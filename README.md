# Sistema de Facturación – Restaurante

Aplicación web de una sola página (HTML + CSS + JavaScript) para facturación de restaurante.

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La aplicación completa (debe llamarse exactamente así) |
| `404.html` | Página de error; redirige al inicio |
| `.nojekyll` | Evita que GitHub procese el sitio con Jekyll |
| `CNAME` | Solo si usas dominio propio (ver abajo) |
| `README.md` | Este documento |

## Publicar en GitHub Pages

1. Crear repositorio en GitHub y subir estos archivos a la raíz.
2. **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, carpeta `/ (root)` → Save.
3. En 1–2 minutos queda en `https://TU-USUARIO.github.io/NOMBRE-REPO/`.

## Dominio propio

1. Crear un archivo `CNAME` en la raíz con una sola línea: tu dominio (ej. `facturacion.midominio.com`).
2. En tu proveedor de DNS:
   - Subdominio (`facturacion.midominio.com`): registro **CNAME** → `TU-USUARIO.github.io`
   - Dominio raíz (`midominio.com`): registros **A** → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
3. En **Settings → Pages → Custom domain** escribir el dominio, guardar y marcar **Enforce HTTPS** cuando esté disponible.

## Importante

- Los datos se guardan en el `localStorage` del navegador: **cada dispositivo tiene sus propios datos** (no se sincronizan).
- Haz respaldos periódicos si la app tiene opción de exportar.
