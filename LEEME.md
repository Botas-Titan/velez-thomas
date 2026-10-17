# LÉEME — Landing Velez Thomas

Archivos de este proyecto:
- `index.html` → la landing page.
- `gracias.html` → página de gracias + políticas de garantía (a donde llega el cliente tras enviar el formulario).
- `img/` → carpeta donde van tus fotos y logos.
- `GUIA-FOTOS.md` → cómo tomar las fotos.

---

## 1) Poner tus fotos
Guarda las imágenes dentro de la carpeta `img/` con estos nombres (o cambia el nombre en el HTML):
- `thomas-negro.jpg` y `thomas-miel.jpg` (foto principal por color)
- `uso-1.jpg` … `uso-4.jpg` (uso diario)
- `cliente-1.jpg` … `cliente-3.jpg` (testimonios)
- `logo-velez.png` (logo, fondo transparente)

En el HTML, cada espacio está marcado con un recuadro `📸` y un comentario que dice qué archivo va ahí. Reemplaza el `<div class="ph">…</div>` por una etiqueta imagen, por ejemplo:
```html
<img src="img/thomas-negro.jpg" alt="Zapato Velez Thomas negro" style="border-radius:16px">
```
(Si me pasas las fotos, yo hago estos reemplazos por ti.)

---

## 2) Comprimir las FOTOS (TinyPNG)
1. Entra a **https://tinypng.com**
2. Arrastra tus `.jpg` / `.png` (hasta 20 a la vez).
3. Descarga las versiones comprimidas y ponlas en `img/`.
> Objetivo: cada foto por debajo de ~200 KB. Así carga rápido en móvil (donde llega tu tráfico).

## 3) Comprimir el VIDEO (HandBrake)
1. Descarga HandBrake gratis: **https://handbrake.fr**
2. Abre tu video → en **Preset** elige `Web > Vimeo/YouTube 720p60` (o 1080p si es para anuncios).
3. Pestaña **Video**: Quality RF ~ **23–26** (más alto = más liviano).
4. **Start Encode**. El archivo final debe pesar bastante menos.

---

## 4) Instalar el PÍXEL (Meta o TikTok)
En `index.html`, arriba del todo (dentro de `<head>`), hay un bloque comentado para **Meta** y otro para **TikTok**.
1. Descomenta el que vayas a usar (quita `<!--` y `-->`).
2. Reemplaza `TU_PIXEL_ID_AQUI` (Meta) o `TU_TIKTOK_PIXEL_ID` (TikTok) por tu ID real.
3. En `gracias.html` ya está preparado el evento de **conversión** (Purchase / CompletePayment): descoméntalo también.

Así mides visitas en la landing y compras en la página de gracias.

---

## 5) Conectar el FORMULARIO
Por defecto, al enviar el formulario redirige a `gracias.html`. Para que además te lleguen los datos, elige UNA opción y me dices cuál:
- **WhatsApp** (lo más simple): el botón arma un mensaje con los datos y abre tu chat.
- **Google Sheets** (gratis, guarda todo en una hoja).
- **n8n** (ya lo usas): mando los datos a un webhook y automatizas.

También cambia el número de WhatsApp: busca `573224146909` en `index.html` y `gracias.html` y pon tu número real (con 57 y sin espacios).

---

## 6) Precios y textos
Están todos en `index.html`. Busca y cambia:
- `$329.900` (precio tachado) y `$150.000` (precio promo). Están en varias partes.
- `-55%` (el % de descuento).
- Nombres/ciudades de los testimonios.

---

## 7) Móvil
La landing ya está hecha **mobile-first** (ancho máx. 520 px centrado, barra de compra fija abajo al hacer scroll, botones grandes). Se ve bien en celular, que es donde llega tu tráfico.

---

## 8) Publicar
Cuando esté lista, se puede subir a **GitHub Pages**, Netlify o tu hosting. Avísame y te guío en el que prefieras.
