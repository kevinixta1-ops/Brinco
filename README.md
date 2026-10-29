# Brinco · Ropa y accesorios para familias primerizas

Tienda web de ropa y accesorios de crianza para bebés, con un asistente (chatbot) que ayuda a las familias primerizas.

- Un solo archivo, `index.html` (HTML, CSS y JavaScript), sin dependencias ni instalación.
- Lista de compra por etapa (0–3, 3–6, 6–12 y 12–24 meses) que filtra el catálogo.
- Catálogo de ropa y de crianza: paseo, alimentación, cuidado e higiene, descanso, juego y seguridad.
- **Jueves de Brinco:** 15 % de descuento automático cada jueves, con aviso en la parte superior y precios tachados. Para probarlo otro día, abre la página con `?jueves` al final de la dirección.
- Bolsa de compras de demostración.
- Chatbot "Brinqui" sobre hospital, tallas, cantidades, lavado, abrigo, sueño, paseo, alimentación, pañales, seguridad, descuentos, envíos y cambios.

## Publicarlo en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `brinco`).
2. Sube `index.html` y `README.md` a la rama `main`.
3. Ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. En uno o dos minutos estará en `https://TU-USUARIO.github.io/brinco/`.

## Personalizar

Todo lo editable está al inicio del script de `index.html`:

- `CONFIG`: textos de envíos y cambios, y el descuento (`pct` = porcentaje, `dia` = día de la semana, 4 = jueves).
- `STAGES` y `EXTRAS`: etapas y cantidades sugeridas.
- `PRODUCTS`: catálogo (nombre, categoría, etapas, precio y emoji).

Los productos, precios y políticas son de ejemplo.

## Sobre el chatbot

GitHub Pages solo sirve archivos estáticos, así que el chatbot funciona con reglas de palabras clave y no necesita servidor ni claves. Para conectar un modelo de IA real (por ejemplo, la API de Claude) hay que añadir un backend o función serverless que guarde la clave de API en secreto; nunca pongas la clave directamente en `index.html`.
