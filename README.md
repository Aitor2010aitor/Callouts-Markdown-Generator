# Callouts Markdown Generator

Un editor visual e interactivo para aprender, escribir y exportar **Markdown de GitHub**, con soporte completo para **Callouts** (`> [!NOTE]`, `> [!TIP]`…), vista previa en tiempo real y exportación a PDF.

Perfecto para documentación, `README.md`, wikis, blogs técnicos y cualquier proyecto que utilice Markdown.

---

## ✨ Características

* 📖 Guía completa sobre los Callouts de GitHub, con explicación de cuándo usar cada tipo.
* ⚡ **Editor Markdown** con vista previa en tiempo real al estilo GitHub.
* 🧰 **Barra de herramientas** para insertar callouts y dar formato con un clic.
* 🖼️ Soporte de **imágenes, badges, tablas, bloques de código, checklists** y más.
* ↶ **Deshacer / Rehacer** con `Ctrl+Z` y `Ctrl+Y`.
* 📂 Abrir archivos `.md` desde tu equipo.
* 📋 Copiar el Markdown limpio con un solo clic.
* 🖨️ **Exportar a PDF** con estilo de página impresa.
* 🔄 Scroll sincronizado entre editor y vista previa.
* 🎨 Interfaz moderna, oscura y responsive.
* 🇪🇸 Totalmente en español.

---

## 🚀 Uso

### Online

Accede a la herramienta desde tu navegador:

```text
https://aitor2010aitor.github.io/Callouts-Markdown-Generator/
```

### Localmente

1. Descarga o clona el repositorio.
2. Abre el archivo:

```text
index.html
```

3. Ve a la pestaña **Generador** y empieza a escribir.

### No requiere

* ❌ Instalación
* ❌ Configuración
* ❌ Dependencias
* ❌ Servidor

Todo funciona directamente en el navegador. Las fuentes se cargan desde Google Fonts y, si no hay conexión, se usan las del sistema.

---

## 📚 Tipos de Callouts Soportados

> [!NOTE]
> Información adicional o contexto útil para el lector.

```md
> [!NOTE]
> Información importante para el lector.
```

> [!TIP]
> Consejos, recomendaciones o atajos opcionales.

```md
> [!TIP]
> Usa atajos para trabajar más rápido.
```

> [!IMPORTANT]
> Información crítica para completar correctamente una tarea.

```md
> [!IMPORTANT]
> Configura las variables de entorno antes de iniciar.
```

> [!WARNING]
> Advertencias sobre riesgos o posibles problemas.

```md
> [!WARNING]
> Esta acción eliminará datos permanentemente.
```

> [!CAUTION]
> Consecuencias negativas derivadas de una acción incorrecta.

```md
> [!CAUTION]
> Modificar este archivo puede corromper la base de datos.
```

Dentro de un callout puedes usar listas, tablas, código, imágenes y formato en línea.

---

## 🧰 Generador

El **Generador** es un editor de dos paneles: escribes a la izquierda y ves el resultado a la derecha.

### Barra de herramientas

| Grupo | Botones |
| --- | --- |
| **Callouts** | Nota, Consejo, Importante, Advertencia, Precaución |
| **Texto** | Negrita, Cursiva, Tachado, MAYÚS, minús, Código |
| **Bloques** | Título, Línea, Lista, Checklist, Cita, Imagen, Bloque código, Tabla |

Los botones funcionan **con o sin texto seleccionado**:

* Con selección, el formato se aplica al texto elegido (línea a línea, respetando el prefijo `>` de los callouts).
* Sin selección, los de texto envuelven la palabra bajo el cursor o insertan una plantilla (`**texto**`), y los de bloque se aplican a la línea actual o insertan un ejemplo.

### Acciones del editor

| Acción | Descripción |
| --- | --- |
| ↶ **Deshacer** / ↷ **Rehacer** | Historial propio de hasta 300 pasos, incluidos los cambios hechos por los botones |
| 📂 **Abrir .md** | Carga un archivo `.md`, `.markdown` o `.txt` en el editor |
| ↺ **Reiniciar** | Vacía el editor (se puede recuperar con `Ctrl+Z`) |
| **Sincronizar scroll** | Mueve la vista previa al mismo ritmo que el editor |
| **Copiar código** | Copia el Markdown limpio al portapapeles |
| **Exportar PDF** | Abre el diálogo de impresión con el documento listo para guardar como PDF |

### Pestañas de la vista previa

* **Previsualización**: cómo se verá en GitHub.
* **Código limpio**: el Markdown final, listo para copiar.

### Atajos de teclado

| Atajo | Acción |
| --- | --- |
| `Ctrl` + `Z` | Deshacer |
| `Ctrl` + `Y` o `Ctrl` + `Shift` + `Z` | Rehacer |
| `Enter` dentro de un callout | Continúa el callout con `>` automáticamente |
| `Enter` dentro de una tabla | Pregunta si quieres añadir otra fila |

En Mac se usa `Cmd` en lugar de `Ctrl`.

---

## 📝 Markdown soportado

| Elemento | Sintaxis |
| --- | --- |
| Títulos | `#` a `######` |
| Negrita / cursiva | `**negrita**`, `*cursiva*`, `***ambas***` |
| Tachado | `~~texto~~` |
| Código en línea | `` `código` `` |
| Bloques de código | ` ```lenguaje ` … ` ``` ` |
| Listas | `- elemento`, `1. elemento` |
| Checklists | `- [ ] pendiente`, `- [x] hecho` |
| Citas | `> texto` |
| Separador | `---` |
| Enlaces | `[texto](https://url)` |
| Imágenes | `![alt](https://url-imagen.png)` |
| Imágenes HTML | `<img src="..." width="400" />` |
| Badges clicables | `[![alt](https://img.shields.io/...)](https://enlace)` |
| Tablas | `\| Col A \| Col B \|` con fila `\| --- \| --- \|` |

### Imágenes y badges

* Las líneas seguidas que contienen solo imágenes o badges se muestran **en una misma fila**, como en GitHub.
* Si una imagen no carga, se reintenta una vez. Los badges de `img.shields.io/badge/...` que fallen se **dibujan en local** a partir de su URL (sin el logo), y el resto de imágenes se sustituyen por su texto alternativo.
* Solo se aceptan imágenes `http(s)://` y `data:image/`. Los enlaces con esquemas peligrosos (como `javascript:`) se bloquean.

### Limitaciones

* No hay listas anidadas.
* No hay resaltado de sintaxis en los bloques de código.
* De las etiquetas HTML solo se interpreta `<img>`; el resto se muestra como texto.

---

## 🖨️ Exportar a PDF

El botón **Exportar PDF** genera una versión de impresión en tema claro:

* Formato A4 con márgenes y numeración de página.
* Callouts con su color e icono.
* Tablas, bloques de código y callouts que no se parten entre páginas.
* Títulos que no quedan solos al final de una página.
* Espera a que carguen las imágenes antes de abrir el diálogo.
* El primer título del documento se propone como nombre del archivo.

En el diálogo de impresión elige **Guardar como PDF** como destino.

---

## 🛠️ Tecnologías

* HTML5
* CSS3
* JavaScript (vanilla)

No utiliza frameworks ni librerías externas.

---

## 🎯 Objetivo

Este proyecto fue creado para ayudar a desarrolladores, escritores técnicos y usuarios de GitHub a comprender fácilmente cómo funcionan los Callouts de Markdown y generar el código correcto sin necesidad de memorizar la sintaxis.

La herramienta combina aprendizaje, ejemplos prácticos y un editor completo con vista previa en una única interfaz simple y accesible.

---

## 🤝 Contribuir

Las contribuciones son bienvenidas.

1. Haz un Fork del proyecto.
2. Crea una nueva rama.

```bash
git checkout -b mi-mejora
```

3. Realiza tus cambios.
4. Haz commit de los cambios.

```bash
git commit -m "Añadir nueva funcionalidad"
```

5. Envía un Pull Request.

---

## ⭐ Apoya el proyecto

Si esta herramienta te ha resultado útil:

* Dale una estrella al repositorio.
* Compártela con otros desarrolladores.
* Propón mejoras o nuevas funcionalidades.

Tu apoyo ayuda a que el proyecto siga creciendo.

---

## 📄 Licencia

Este proyecto está distribuido bajo la licencia MIT.

Puedes usarlo, modificarlo y distribuirlo libremente respetando los términos de la licencia.

---

## 👨‍💻 Autor

Creado para facilitar la creación de documentación más clara, visual y profesional mediante GitHub Markdown Callouts.
