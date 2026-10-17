# Mariscos Luse

Tienda y centro de control en https://mariscos-luse.pages.dev/ . Publicación automática desde la rama main con Cloudflare Pages Free.

## Gestión del negocio

Acceso Tech con Supabase Auth y permisos en base de datos. Incluye catálogo compartido, precios con historial, entradas por lote y proveedor, compra bruta y cantidad aprovechable, costos adicionales por producto, mermas, ajustes, ventas realizadas, gastos y dashboard de rentabilidad.

Los pedidos del carrito siguen siendo demostraciones locales y no se convierten automáticamente en ventas ni reservas. El inventario comienza en cero hasta registrar existencias reales. Las proyecciones requieren costos y precios reales; el resultado no incluye impuestos ni gastos omitidos.

## Fuente y publicación

El ZIP mariscos-luse-fuente.zip contiene fuente React, migraciones, pruebas y guía. Extraer en otra carpeta, ejecutar npm ci y configurar las variables públicas de Supabase a partir de .env.example. Nunca poner claves secretas en VITE_*.

npm test ejecuta pruebas; npm run build compila; node scripts/prepare-static.mjs genera un HTML estático con el código y estilos integrados en publish/. Subir index.html y mantener los archivos públicos. El ZIP no incluye contraseñas, sesiones ni claves privadas.

Cloudflare: framework None; comando de compilación vacío; salida /.

La copia del código no constituye un respaldo de los datos de Supabase. El respaldo automático de base de datos sigue pendiente.
