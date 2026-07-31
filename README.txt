MASTER FANTASY PRO V4.5 — CORRECCIÓN SOBRE EL PROYECTO REAL

FALLO ENCONTRADO:
El OCR sí leía el texto, pero el parser esperaba frases del tipo “Has comprado a...”.
Las capturas reales usan: “MANAGER ha comprado/vendido al jugador NOMBRE de/a LALIGA por IMPORTE”.
Por eso la tabla de revisión quedaba sin operaciones válidas y Actividad no se actualizaba.

CORREGIDO:
- Parser adaptado al formato real de las capturas de LALIGA Fantasy.
- Reconoce manager, compra/venta, jugador e importe.
- Soporta saltos de línea, puntos en importes, iniciales y acentos.
- Mantiene revisión manual antes de guardar.
- Mantiene la misma clave de almacenamiento para conservar los datos existentes.
- Caché del service worker actualizada para forzar la nueva versión.

INSTALACIÓN:
1. Sustituye todos los archivos del repositorio por estos.
2. Espera a que GitHub Pages termine de publicar.
3. En PC pulsa Ctrl+F5.
4. En iPhone cierra la app por completo y vuelve a abrirla. Si aún carga la anterior, elimina el acceso de la pantalla de inicio y vuelve a añadirlo.
