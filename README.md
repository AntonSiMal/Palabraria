# 🧩 Palabraria

> *"Donde las palabras se cruzan y las ideas cobran forma"*

**Palabraria** es un generador de crucigramas interactivo que transforma archivos de Excel (`.xlsx`, `.xls`) o de texto (`.csv`, `.tsv`) con pistas y respuestas en crucigramas listos para imprimir. Cuenta con un diseño elegante inspirado en mapas topográficos y juegos de mesa clásicos, además de exportación profesional a PDF.

🌐 **[🚀 Ver Demo en Vivo](https://antonsimal.github.io/Palabraria/)**

![Versión](https://img.shields.io/badge/Versión-1.1.0-1f1b17?style=flat-square)
![Licencia](https://img.shields.io/badge/Licencia-MIT-5a8f5a?style=flat-square)
![Estado](https://img.shields.io/badge/Estado-Activo-5a8f5a?style=flat-square)

---

## ✨ Características

- 📁 **Carga flexible de archivos**: Soporta Excel (`.xlsx`, `.xls`), CSV, TSV y TXT. En Excel, lee automáticamente la Columna A (pistas) y Columna B (respuestas).
- 🧠 **Limpieza inteligente de respuestas**: Acepta respuestas con espacios, números y cualquier combinación de mayúsculas/minúsculas. El sistema las adapta automáticamente a la cuadrícula (eliminando espacios y acentos).
- 🎲 **Múltiples alternativas**: Genera diferentes disposiciones del crucigrama con un solo clic.
- 👁️ **Vista dual**: Alterna instantáneamente entre ver el crucigrama con o sin respuestas.
- 📄 **Exportación a PDF**: Descarga el crucigrama en PDF con diseño profesional, celdas negras reales y pistas organizadas en dos columnas.
- 🗺️ **Diseño Topo**: Estética cuidada inspirada en mapas topográficos con tonos tierra, crema y acentos dorados.
- 📱 **100% Responsive**: Se adapta perfectamente a dispositivos móviles, tablets y escritorio.
- 🔍 **Vista previa en tiempo real**: Visualiza las pistas cargadas y cómo se adaptarán antes de generar el crucigrama.

---

## 🚀 Inicio Rápido

No necesitas instalar nada. La aplicación funciona completamente en el navegador:

1. Visita la **[Demo en Vivo](https://antonsimal.github.io/Palabraria/)**
2. Haz clic en **"Seleccionar archivo"** y carga tu archivo de Excel o texto.
3. Revisa la vista previa y haz clic en **"🧩 Generar Palabraria"**.
4. Descarga tu PDF listo para imprimir.

*(Opcional) Si deseas ejecutarlo localmente, solo descarga el archivo `index.html` y ábrelo en cualquier navegador moderno, o usa un servidor local:*
```bash
# Con Python
python -m http.server 8000

# Con Node.js
npx http-server
```

---

## 📋 Formato de los archivos

Palabraria es inteligente y se adapta a tu flujo de trabajo. Puedes usar cualquiera de estos formatos:

### 📊 Archivo de Excel (.xlsx, .xls) *(Recomendado)*
Simplemente organiza tu hoja de cálculo con dos columnas:
- **Columna A**: La pista o pregunta.
- **Columna B**: La respuesta.

*Ejemplo en Excel:*
| A (Pista) | B (Respuesta) |
| :--- | :--- |
| Memoria temporal y volátil que actúa como "tabla de trabajo". | RAM |
| Atajo de teclado para deshacer un error. | Ctrl Z |
| Software principal que administra los recursos. | Sistema Operativo |

### 📝 Archivo de Texto (.csv, .tsv, .txt)
Detecta automáticamente el separador (tabulación, coma o punto y coma).
```csv
pregunta,respuesta
"Capital de Francia",PARIS
"Color del cielo",AZUL
```

### 📌 Reglas importantes:
- ✅ **Las respuestas son flexibles**: Pueden contener **espacios, números y cualquier combinación de mayúsculas/minúsculas** (ej. `Ctrl Z`, `Sistema Operativo`, `DOCX`). El sistema las convertirá automáticamente a mayúsculas sin espacios ni acentos para encajar perfectamente en la cuadrícula (ej. `CTRLZ`, `SISTEMAOPERATIVO`).
- ✅ **Las preguntas** se mantienen exactamente como las escribiste para una lectura clara en el PDF.
- ✅ Se puede incluir o omitir la fila de encabezado en archivos de texto.

---

## 🎯 Cómo usar la herramienta

1. **Cargar archivo**: Haz clic en el botón de carga y selecciona tu archivo de Excel o texto.
2. **Vista previa**: Revisa la lista desplegable para confirmar que las preguntas y respuestas se leyeron y adaptaron correctamente.
3. **Generar**: Haz clic en "🧩 Generar Palabraria".
4. **Alternativas**: Si la distribución no te convence, usa "🎲 Nueva Alternativa" para reorganizar las palabras y buscar más intersecciones.
5. **Vista previa**: Usa los botones "Ocultar/Mostrar Respuestas" para verificar el resultado final.
6. **Descargar**: Exporta el PDF "Sin Respuestas" (para los jugadores) o "Con Respuestas" (para el facilitador).

---

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica y accesible.
- **CSS3** - Estilos modernos con variables CSS (`:root`) y `color-mix()` para la paleta topográfica.
- **JavaScript (ES6+)** - Lógica del generador, algoritmo de colocación de palabras y parsers robustos.
- **SheetJS (xlsx)** - Lectura y procesamiento de archivos Excel directamente en el navegador.
- **jsPDF** - Generación de documentos PDF profesionales sin necesidad de backend.

---

## 🎨 Paleta de Colores (Estilo Topo)

| Color | Hex | Uso |
|-------|-----|-----|
| 🟫 Tierra | `#ece6da` | Fondo general de la página |
| 📜 Crema | `#fffdf8` | Fondo de celdas y contenedores |
| ⬛ Tinta | `#1f1b17` | Texto principal y celdas negras |
| 🟫 Línea | `#b9ad9b` | Bordes, separadores y grid |
| 🟡 Acento | `#d4a04a` | Números de celda, badges y destacados |
| 🟢 Correcto | `#5a8f5a` | Mensajes de éxito |
| 🔴 Error | `#8b4545` | Mensajes de error |
| 🔵 Mar | `#daeffc` | Fondos de información y ayuda |

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Si quieres mejorar Palabraria:

1. Haz un fork del repositorio.
2. Crea una rama para tu funcionalidad (`git checkout -b feature/nueva-funcionalidad`).
3. Haz commit de tus cambios (`git commit -m 'Añadir nueva funcionalidad'`).
4. Haz push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Abre un Pull Request.

### 💡 Ideas para futuras mejoras:
- [ ] Soporte para crucigramas temáticos con imágenes o iconos.
- [ ] Exportar el crucigrama a formato de imagen (PNG/SVG).
- [ ] Modo de juego interactivo en la web (escribir directamente en las celdas).
- [ ] Biblioteca de plantillas de crucigramas predefinidos.
- [ ] Soporte para múltiples idiomas y diccionarios automáticos.

---

## 🐛 Reportar Problemas

Si encuentras un bug o tienes una sugerencia, por favor abre un [Issue](https://github.com/antonsimal/Palabraria/issues) en el repositorio incluyendo:
- Descripción clara del problema.
- Pasos para reproducirlo.
- El archivo (Excel o CSV) que causó el error (si aplica).
- Capturas de pantalla si es posible.

---

## 📄 Licencia

Este proyecto está bajo la **Licencia MIT**. Consulta el archivo [LICENSE](LICENSE) para más detalles. Esto significa que puedes usar, modificar y distribuir este código libremente, siempre que mantengas el aviso de copyright original.

---

## 👨‍💻 Autor

Desarrollado con ❤️ por **[Anton Simal](https://github.com/antonsimal)**

---

<div align="center">

**Palabraria** · Generador de crucigramas con estilo topográfico

⭐ ¡Si te gusta este proyecto, no olvides darle una estrella en GitHub! ⭐

</div>
