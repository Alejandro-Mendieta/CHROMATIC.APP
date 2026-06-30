```markdown
# 🎨 CHROMATIC · ESTUDIO PROFESIONAL DE COLOR

> Una herramienta profesional para diseñadores, artistas y creadores. Selecciona, explora y exporta colores con una ruleta cromática de 5 niveles y una base de datos de más de 1000 colores.

## ✨ Características Principales

### 🎡 Selector Cromático Avanzado
- **Ruleta de 5 niveles** con diferentes saturaciones (100% → 20%)
- **360 segmentos por nivel** para máxima precisión
- **Controles HSV** (Matiz, Saturación, Brillo) con sliders interactivos
- **Visualización en tiempo real** del color seleccionado

### 🎨 Base de Datos de Colores
- **Más de 1000 colores** con nombres profesionales
- Categorías: Rojos, Naranjas, Amarillos, Verdes, Azules, Púrpuras, Marrones, Grises, Blancos, Negros, Rosas, Cian, Lavandas, Metálicos
- **Colores de marcas famosas** (Spotify, Twitter, Instagram, etc.)
- **Detección inteligente** del nombre más cercano

### 📚 Gestión de Paletas
- **Guardar colores favoritos** en paleta personal
- **Almacenamiento local** (persistente entre sesiones)
- **Eliminar colores** con un clic
- **Límite de 20 colores** por paleta

### 🌈 Paletas Armónicas
- **4 tipos de armonías**: Complementario, Análogo, Triádico, Tetrádico
- **Generación automática** de paletas basadas en el color actual
- **Sugerencias inteligentes** de colores relacionados

### 📤 Exportación Profesional
| Formato | Descripción | Uso |
|---------|-------------|-----|
| **PNG Color** | Imagen 600x600 con info del color | Redes sociales, presentaciones |
| **PNG Gradiente** | Gradiente puro sin texto | Fondos, wallpapers |
| **JSON** | Datos completos de la paleta | Backup, compartir |
| **CSS Variables** | Código CSS listo para copiar | Desarrollo web |

### 🔍 Herramientas de Análisis
- **Contraste WCAG** (Ratios AA/AAA con blanco y negro)
- **Generador de gradientes CSS** (color + complementario)
- **Estadísticas en tiempo real** (colores guardados, armonías, contraste)
- **Información completa**: RGB, HEX, HSV, luminosidad

### 🎯 Interfaz Profesional
- **Modo oscuro/claro** con persistencia
- **Diseño responsive** (funciona en móvil y escritorio)
- **Atajos de teclado** para acciones rápidas
- **Toast notifications** para feedback visual

## ⌨️ Atajos de Teclado

| Tecla | Acción |
|-------|--------|
| `Ctrl + S` | Guardar color actual |
| `Ctrl + G` | Copiar gradiente CSS |
| `Ctrl + D` | Cambiar modo oscuro/claro |
| `Ctrl + E` | Exportar color como PNG |

## 🚀 Instalación y Uso

### Opción 1: Uso directo (recomendado)
1. Descarga el archivo `index.html`
2. Ábrelo en tu navegador favorito
3. ¡Comienza a explorar colores!

### Opción 2: Servidor local
```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx serve .

# Usando VS Code Live Server
# Instala la extensión y haz clic en "Go Live"
```

### Opción 3: Despliegue web
Sube el archivo a cualquier servicio de hosting (GitHub Pages, Netlify, Vercel, etc.)

## 📖 Cómo Usar

### 1. Seleccionar un color
- **Ruleta**: Haz clic en cualquier zona (borde = vivos, centro = pastel)
- **Sliders**: Ajusta Matiz, Saturación y Brillo
- **Códigos**: Copia RGB, HEX o HSV con un clic

### 2. Guardar en paleta
- Haz clic en **"GUARDAR COLOR"**
- Los colores aparecerán en "MI PALETA"
- **Haz clic** en cualquier color guardado para usarlo
- **Hover** y clic en ✕ para eliminar

### 3. Explorar armonías
- Selecciona el tipo de armonía (Complementario, Análogo, etc.)
- Los colores sugeridos aparecen abajo
- **Haz clic** en cualquier sugerencia para usarla

### 4. Exportar
- **Exportar color**: Genera PNG con información del color
- **Exportar gradiente**: Genera PNG solo del gradiente
- **Exportar JSON**: Guarda toda tu paleta
- **Importar JSON**: Recupera paletas guardadas

### 5. Obtener código CSS
- **CSS Variables**: Genera variables CSS automáticamente
- **Gradiente CSS**: Código listo para copiar
- **Contraste WCAG**: Verifica accesibilidad

## 🎨 Categorías de Colores Incluidas

| Categoría | Cantidad |
|-----------|----------|
| 🔴 Rojos | 60 |
| 🟠 Naranjas | 60 |
| 🟡 Amarillos | 60 |
| 🟢 Verdes | 80 |
| 🔵 Azules | 80 |
| 🟣 Púrpuras/Violetas | 60 |
| 🟤 Marrones/Tierra | 70 |
| ⚪ Grises | 70 |
| 🤍 Blancos/Beiges | 70 |
| ⚫ Negros | 50 |
| 🩷 Rosas/Corales | 60 |
| 💙 Cian/Turquesas | 60 |
| 💜 Lavandas/Lilas | 60 |
| 💚 Verdes neón | 40 |
| 🥇 Metálicos | 50 |
| 🏷️ Marcas famosas | 50 |
| **TOTAL** | **≈ 1020 colores** |

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica
- **CSS3** - Estilos modernos con variables CSS
- **JavaScript (ES6+)** - Lógica interactiva
- **Canvas API** - Ruleta cromática y cuadrículas
- **LocalStorage** - Persistencia de datos
- **html2canvas** - Exportación de imágenes

## 📁 Estructura del Proyecto

```
chromatic/
├── index.html          # Aplicación completa (todo en uno)
├── README.md           # Documentación
```

## 🔧 Personalización

### Modificar colores de la base de datos
Edita el objeto `colorNames` en el script para añadir más colores:

```javascript
const colorNames = {
    '255,0,0': 'ROJO CADMIO',
    // Añade más colores aquí
};
```

### Ajustar tamaño de exportación
Modifica la constante `size` en las funciones `exportColorAsPNG` y `exportGradientAsPNG`:

```javascript
const size = 600; // Cambia a 800, 1024, etc.
```

### Cambiar límite de colores en paleta
Edita la línea en `saveCurrentColor()`:

```javascript
if(customColors.length > 20) customColors.pop(); // Cambia 20 por tu límite
```

## 🌐 Navegadores Soportados

| Navegador | Versión mínima |
|-----------|----------------|
| Chrome | 60+ |
| Firefox | 60+ |
| Safari | 12+ |
| Edge | 79+ |
| Opera | 50+ |
| iOS Safari | 12+ |
| Chrome Android | 60+ |

## 📊 Rendimiento

- **Tamaño del archivo**: ~150KB (minificado)
- **Tiempo de carga**: < 500ms
- **Memoria RAM**: ~30MB
- **Sin dependencias externas** (excepto html2canvas opcional)

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea tu rama (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Distribuido bajo la licencia MIT. Ver `LICENSE` para más información.

## 📧 Contacto

- **Autor**: ALEJANDRO MENDIETA
- **Web**: https://chromatic.app

## 🙏 Agradecimientos

- Inter font family by Google Fonts
- html2canvas library for PNG export
- WCAG contrast guidelines by W3C

## 📌 Notas de Versión

### v2.0 (2026)
- ✨ Añadidos más de 1000 colores a la base de datos
- ✨ Nuevo selector de 5 niveles en la ruleta
- ✨ Exportación de gradiente PNG
- ✨ Modo oscuro/claro con persistencia
- ✨ Paletas armónicas (4 tipos)
- ✨ Contraste WCAG con recomendaciones
- ✨ Atajos de teclado
- ✨ Diseño completamente responsive

### v1.0 (2025)
- 🎉 Lanzamiento inicial
- Selector de color básico
- Paleta personal
- Exportación a PNG y JSON

---

## 🎯 Ejemplos de Uso

### Diseñador Gráfico
1. Selecciona un color base
2. Genera paletas armónicas
3. Guarda los colores que más te gusten
4. Exporta como CSS variables para tu proyecto

### Desarrollador Web
1. Encuentra el color exacto que necesitas
2. Copia el código HEX o RGB
3. Genera el gradiente CSS automáticamente
4. Verifica el contraste WCAG

### Artista Digital
1. Explora la ruleta para encontrar inspiración
2. Guarda tus colores favoritos
3. Exporta como PNG para compartir
4. Importa paletas anteriores

### Social Media Manager
1. Captura colores de marca
2. Crea paletas coherentes
3. Exporta como imágenes para posts
4. Mantén consistencia visual

---

**Hecho con 🎨 para creadores de todo el mundo**
```ALEJANDRO MENDIETA
