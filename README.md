# Nela · Tu vida también es un proyecto

Sitio web estático (HTML + CSS + JS, sin framework). Se publica con **GitHub Pages**.

## Cómo está organizado
- `index.html` — página principal (home emocional).
- `professional.html` — perfil profesional / CV.
- `guia-*.pdf` — las 4 guías en español. `guia-*-en.pdf` — las mismas en inglés.
- `favicon.*`, `apple-touch-icon.png`, `og-image.png` — íconos e imagen para compartir.
- `nela-historia.jpg`, `nela-professional.jpg` — fotos.

## Activar el captador de correos (Formspree) — 1 sola línea
1. Crea una cuenta gratis en https://formspree.io
2. Crea un formulario y copia su ID (se ve así: `xmyzabcd`).
3. Abre `index.html`, busca `TU_ID` y reemplázalo por tu ID.
   - Está en la línea: `var FORMSPREE = "https://formspree.io/f/TU_ID";`
4. Guarda. Listo: ahora los correos del quiz, newsletter y contacto te llegan a Formspree.

> Mientras diga `TU_ID`, el sitio funciona y la guía se descarga igual;
> solo los correos no se guardan hasta que pongas tu ID real.

## Cómo actualizar una guía
Sube el PDF nuevo con el **mismo nombre** (ej. `guia-empezando.pdf`) y reemplaza el anterior.
No hay que tocar nada más: el sitio ya apunta a esos nombres.

## Cómo cambiar textos
Edita `index.html`. Los textos en español e inglés están en el diccionario `I18N`
dentro de la etiqueta `<script>` al final del archivo.

## Dominio propio (cuando quieras)
GitHub → Settings → Pages → Custom domain. Se añade un archivo `CNAME` automáticamente.
