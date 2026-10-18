# 🧩 Palabraria

> *"Donde las palabras se cruzan y las ideas cobran forma"*

**Palabraria** es un generador de crucigramas interactivo que transforma archivos de Excel (`.xlsx`, `.xls`) o de texto (`.csv`, `.tsv`) con pistas y respuestas en crucigramas listos para imprimir. Cuenta con un diseño elegante inspirado en mapas topográficos y juegos de mesa clásicos, además de exportación profesional a PDF.

🌐 **[🚀 Ver Demo en Vivo](https://antonsimal.github.io/Palabraria/)**

![Versión](https://img.shields.io/badge/Versión-1.1.0-1f1b17?style=flat-square)
![Licencia](https://img.shields.io/badge/Licencia-MIT-5a8f5a?style=flat-square)
![Estado](https://img.shields.io/badge/Estado-Activo-5a8f5a?style=flat-square)

---

## ✨ Características

- 📊 **Soporte nativo para Excel**: Lee automáticamente la **Columna A** (pistas) y la **Columna B** (respuestas).
- 🧠 **Limpieza inteligente**: Acepta respuestas con espacios, números o mayúsculas/minúsculas (ej. `Ctrl Z`, `Sistema Operativo`). El sistema las adapta automáticamente a la cuadrícula eliminando espacios y acentos (ej. `CTRLZ`, `SISTEMAOPERATIVO`).
- 🎲 **Múltiples alternativas**: Genera diferentes disposiciones del crucigrama con un solo clic.
- 👁️ **Vista dual**: Alterna instantáneamente entre ver el crucigrama con o sin respuestas.
- 📄 **Exportación a PDF profesional**: Descarga el crucigrama con celdas negras reales y pistas organizadas en dos columnas lado a lado.
- 🗺️ **Diseño Topo**: Estética cuidada inspirada en mapas topográficos con tonos tierra y crema.
- 📱 **100% Responsive**: Se adapta perfectamente a móviles, tablets y escritorio.

---

## 🚀 Inicio Rápido

No necesitas instalar nada. La aplicación funciona completamente en el navegador:

1. Visita la **[Demo en Vivo](https://antonsimal.github.io/Palabraria/)**
2. Haz clic en **"Seleccionar archivo"** y carga tu archivo de Excel o texto.
3. Revisa la vista previa y haz clic en **"🧩 Generar Palabraria"**.
4. Descarga tu PDF listo para imprimir.

*(Opcional) Si deseas ejecutarlo localmente, descarga el archivo `index.html` y ábrelo en tu navegador, o usa un servidor local:*
```bash
python -m http.server 8000
```

---

## 📋 Formato de los archivos

### 📊 Archivo de Excel (.xlsx, .xls) *(Recomendado)*
El sistema está diseñado para leer tu hoja de cálculo de la siguiente manera:
- **Columna A**: Contiene la pista o pregunta.
- **Columna B**: Contiene la respuesta.

**Ejemplo práctico en Excel:**

| Columna A (Pista) | Columna B (Respuesta) |
| :--- | :--- |
| Software principal que administra los recursos de la computadora. | Sistema Operativo |
| Atajo de teclado que se usa para deshacer un error cometido recientemente. | Ctrl Z |
| Extensión de archivo típica para un documento de texto profesional. | DOCX |
| Memoria temporal y volátil que se borra al apagar la PC. | RAM |

> 💡 **Nota sobre las respuestas:** No necesitas ajustar el formato manualmente. Si escribes `Sistema Operativo` o `Ctrl Z` en la Columna B, Palabraria lo procesará inteligentemente y lo colocará en la cuadrícula como `SISTEMAOPERATIVO` o `CTRLZ` (mayúsculas, sin espacios ni acentos), mientras que en el PDF se mostrará la pista original completa y legible.

### 📝 Archivo de Texto (.csv, .tsv, .txt)
Si prefieres usar texto, el sistema detecta automáticamente el separador (tabulación, coma o punto y coma).
```csv
Pista,Respuesta
"Capital de Francia",PARIS
"Color del cielo",AZUL
```

---

## 🎯 Cómo usar la herramienta

1. **Cargar archivo**: Haz clic en el botón de carga y selecciona tu archivo de Excel o texto.
2. **Vista previa**: Revisa la lista para confirmar que las preguntas y respuestas se leyeron y adaptaron correctamente.
3. **Generar**: Haz clic en "🧩 Generar Palabraria".
4. **Alternativas**: Si la distribución no te convence, usa "🎲 Nueva Alternativa" para reorganizar las palabras y buscar más intersecciones.
5. **Verificar**: Usa los botones "Ocultar/Mostrar Respuestas" para revisar el resultado.
6. **Descargar**: Exporta el PDF "Sin Respuestas" (para los jugadores) o "Con Respuestas" (hoja de respuestas para el facilitador).

---

## 🛠️ Tecnologías Utilizadas

- **HTML5 / CSS3** - Estructura semántica y estilos modernos con variables CSS.
- **JavaScript (ES6+)** - Lógica del generador y algoritmo de colocación de palabras.
- **SheetJS (xlsx)** - Lectura y procesamiento de archivos Excel directamente en el navegador.
- **jsPDF** - Generación de documentos PDF profesionales sin necesidad de backend.

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Si quieres mejorar Palabraria:

1. Haz un fork del repositorio.
2. Crea una rama para tu funcionalidad (`git checkout -b feature/nueva-funcionalidad`).
3. Haz commit de tus cambios (`git commit -m 'Añadir nueva funcionalidad'`).
4. Haz push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Abre un Pull Request.

### 💡 Ideas para futuras mejoras:
- [ ] Modo de juego interactivo en la web (escribir directamente en las celdas).
- [ ] Exportar el crucigrama a formato de imagen (PNG/SVG).
- [ ] Biblioteca de plantillas de crucigramas predefinidos.

---

## 🐛 Reportar Problemas

Si encuentras un bug o tienes una sugerencia, por favor abre un [Issue](https://github.com/antonsimal/Palabraria/issues) en el repositorio incluyendo:
- Descripción clara del problema.
- Pasos para reproducirlo.
- El archivo (Excel o CSV) que causó el error (si aplica).

---

## 📄 Licencia

Este proyecto está bajo la **Licencia MIT**. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

## 👨‍💻 Autor

Desarrollado con ❤️ por **[Anton Simal](https://github.com/antonsimal)**

---

<div align="center">

**Palabraria** · Generador de crucigramas con estilo topográfico

⭐ ¡Si te gusta este proyecto, no olvides darle una estrella en GitHub! ⭐

</div>
