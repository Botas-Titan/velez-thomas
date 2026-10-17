# Manual para publicar la landing "Velez Thomas" en Carrd (Cowork)

> **Cómo usar este manual:** copia y pega TODO el contenido de este archivo como primer mensaje en una nueva sesión de Cowork. Le da al asistente el contexto y los pasos. Luego tú harás el login en Carrd (eso no lo puede hacer el asistente).

---

## 1. Contexto para el asistente (léelo, no me lo repitas)

- Tengo una landing page de un producto llamado **tenis Velez Thomas** (colores negro y miel).
- El archivo listo para publicar es: **`carrd-embed.html`** (carpeta del proyecto: `C:\Users\gabri\Downloads\claude\velez-thomas\`).
- Ese archivo es **autocontenido**: las fotos van incrustadas en base64 y la "página de gracias" (con políticas de garantía) está integrada: aparece como una pantalla encima cuando se envía el formulario.
- Lo voy a publicar en **Carrd** (tengo plan **Pro**, así que tengo el elemento **Embed / Code**).
- Carrd es de **una sola página**; por eso la gracias va integrada, no como página aparte.

## 2. Qué quiero que hagas, asistente

1. Antes que nada, **ábreme `carrd-embed.html`** y ayúdame a editar 2 valores al inicio del `<script>`:
   - `var WA_NUMERO = '573224146909';` → reemplázalo por mi número real de WhatsApp (formato: 57 + número, sin `+` ni espacios). **Pregúntame el número si no te lo he dado.**
   - `var VIDEO_URL = '';` → si ya tengo el enlace directo del video `.mp4`, ponlo ahí; si no, déjalo vacío.
2. Verifica que el archivo abra bien en el navegador (fotos visibles, contador corriendo, y que al enviar el formulario aparezca la pantalla de gracias con las políticas). Si algo falla, corrígelo.
3. Abre **Carrd** en el navegador de Cowork (`https://carrd.co`) y **guíame paso a paso** mientras yo hago el login y pego el código. Ve indicándome cada clic y revisando conmigo que quede bien.
4. **Importante (lo que NO debes hacer):** no inicies sesión por mí, no crees cuentas, no aceptes términos ni publiques por mí. Esas acciones las hago yo; tú me guías y revisas.

## 3. Pasos exactos en Carrd (guíame con estos)

1. Entro a `https://carrd.co` e inicio sesión (lo hago yo).
2. **+ Add site** → plantilla **Blank** (en blanco).
3. Botón **+ (Add element)** → elijo **Embed**.
4. En el panel derecho, **Type → Code**.
5. En el campo **Code**, pego **TODO** el contenido de `carrd-embed.html`.
6. En **Style**, dejo **Inline** (para que se vea, no oculto).
7. Selecciono la **sección/contenedor** del embed → **Width: Full** y **Padding: None** (la landing ya viene centrada a 520px sola).
8. **Preview** para revisar en móvil (icono de teléfono). Reviso: fotos, colores, contador, testimonios, marcas (que abran WhatsApp), formulario → pantalla de gracias → botón "Volver".
9. **Publish** → le pongo mi subdominio o mi dominio propio.

## 4. Recomendado hacerlo en Carrd (no en el código)

- **Píxel de Meta / TikTok:** ponerlo en **Settings** de Carrd (campo de analítica/embed en head) es más limpio. En el código también quedó el bloque comentado por si lo prefiero ahí.
- **Video:** cuando lo tenga comprimido (HandBrake), lo **subo** (como asset de Carrd o a un hosting) y pego su URL directa en `VIDEO_URL` dentro del código. Mientras tanto se ve un recuadro guía.

## 5. Datos útiles

- Precio actual en la landing: **$150.000** (antes $329.900, -55%). Si quiero cambiarlo, dímelo y lo ajustas en el código (aparece en varias partes).
- El formulario hoy **no envía los datos a ningún lado todavía**: solo muestra la pantalla de gracias. Si quiero recibir los pedidos, ayúdame a conectarlo a **WhatsApp, Google Sheets o n8n** (pregúntame cuál prefiero).
- Nº de WhatsApp: pendiente por darte. Píxel: pendiente por darte el ID.

---

### Checklist final antes de publicar
- [ ] `WA_NUMERO` con mi número real.
- [ ] Botones de marcas abren WhatsApp con el mensaje correcto.
- [ ] Formulario muestra la pantalla de gracias + políticas.
- [ ] Se ve bien en móvil (vista previa de Carrd).
- [ ] (Opcional) Video y píxel configurados.
