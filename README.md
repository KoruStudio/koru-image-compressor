[README.md](https://github.com/user-attachments/files/31810190/README.md)
# KSVT — Compresor de Imágenes

Herramienta del sistema [Koru Studio Visual Tools](https://github.com/KoruStudio). Comprime y convierte imágenes en lote directamente en el navegador. Sin servidor, sin cuenta, sin conexión.

## Qué hace

- Comprime JPEG, PNG, WebP y GIF a JPEG, WebP o PNG indexado
- PNG indexado propio: cuantización por corte mediano, 24–76 % del peso original
- Descarga individual por imagen o lote completo en ZIP
- Procesa archivos de más de 20 MB sin congelar la interfaz
- Motor automático: Web Worker si el navegador lo soporta, hilo principal como reserva

## Cómo usarlo

Descarga `index.html` y ábrelo con doble clic. No necesita instalación ni conexión.

También disponible en GitHub Pages: `https://korostudio.github.io/koru-image-compressor`

## Formatos

| Entrada | Salida |
|---|---|
| JPEG, PNG, WebP, GIF | JPEG · WebP · PNG indexado |

## Pesos esperados

| Caso | Resultado típico |
|---|---|
| Foto JPEG → JPEG 80% | −40 % a −85 % |
| Captura PNG → PNG 80% | −24 % a −78 % |
| Foto JPEG → WebP 80% | −50 % a −90 % |
| PNG ya optimizado → PNG | 0 % (se conserva el original) |

## Dependencias

Ninguna en red. El ZIP se genera con un escritor propio incluido en el archivo.

## Licencia

MIT — Donald © 2024 Koru Studio
