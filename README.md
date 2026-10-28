# Mi Recetario visual

## Publicación en Vercel
1. Descomprimí el ZIP y subí sus archivos a un repositorio nuevo de GitHub.
2. En Vercel elegí **Add New → Project** e importá ese repositorio.
3. En **Settings → Environment Variables** agregá `APP_PASSWORD` (una contraseña propia y larga) y `OPENAI_API_KEY` (tu clave de API de OpenAI).
4. Hacé **Redeploy** y abrí la URL que te entrega Vercel.

El análisis usa una API de IA y puede generar costos según el uso. No compartas tu clave API.

## Limitaciones importantes de esta primera versión
Esta versión es un prototipo funcional de interfaz y lectura: las recetas quedan en memoria mientras la página está abierta; al recargar/cerrar se pierden y no se sincronizan entre dispositivos. El login es una barrera simple, no autenticación robusta. Antes de guardar recetas de forma permanente o usarlo con datos privados, hay que agregar autenticación real y almacenamiento privado (por ejemplo Supabase Auth + Storage + base de datos con políticas de acceso).

Para ejecutar localmente se necesita Node.js 20+. Instalá dependencias con `npm install`. Las funciones API de Vercel requieren `vercel dev` para probarse localmente.
