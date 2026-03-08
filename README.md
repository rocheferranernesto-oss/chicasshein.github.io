# Chic@s SheinUNE - Tienda Online

![Chic@s SheinUNE](https://img.shields.io/badge/Chic%40s%20SheinUNE-Moda%20con%20Esencia-ff6b9d)
![Versión](https://img.shields.io/badge/Versi%C3%B3n-1.0.0-6c5ce7)
![Estático](https://img.shields.io/badge/100%25-Est%C3%A1tico-00cec9)

> **Tu estilo, tus reglas, tu momento. ✨**

---

## 📋 Descripción

**Chic@s SheinUNE** es una tienda online 100% estática diseñada específicamente para el mercado cubano. Combina un diseño visual premium con una gestión de catálogo simplificada al máximo, sin necesidad de servidores externos, bases de datos ni dependencias complejas.

### Características Principales

- ✅ **Catálogo 100% Estático** - Productos integrados directamente en el código
- ✅ **Diseño Premium** - Interfaz moderna, vibrante y responsive
- ✅ **WhatsApp Integrado** - Contacto directo con clientes
- ✅ **Precios en CUP** - Formato cubano correcto
- ✅ **Panel de Admin** - Dashboard visual con estadísticas
- ✅ **Sin Ubicación** - Sin mapas ni referencias geográficas
- ✅ **Optimizado para Cuba** - Conexiones lentas y móviles

---

## 🚀 Cómo Usar Localmente

### Opción 1: Doble Clic (Más Simple)

1. Descarga todos los archivos del proyecto
2. Haz doble clic en `index.html`
3. ¡Listo! La tienda se abrirá en tu navegador

### Opción 2: Servidor Local (Recomendado para pruebas)

```bash
# Usando Python 3
python -m http.server 8000

# Usando Node.js (necesitas instalar http-server)
npx http-server -p 8000

# Usando PHP
php -S localhost:8000
```

Luego abre tu navegador en `http://localhost:8000`

---

## 📦 Estructura de Archivos

```
chicassheinune/
├── index.html          # Página principal de la tienda
├── admin.html          # Panel de administración
├── README.md           # Este archivo
└── (imágenes de productos)
```

### Archivos Principales

| Archivo | Descripción |
|---------|-------------|
| `index.html` | Página principal con catálogo de productos, filtros y contacto |
| `admin.html` | Panel de administración con login, dashboard e inventario |

---

## 🌐 Despliegue en Hosting Gratuito

### Opción 1: GitHub Pages

1. Crea un repositorio en GitHub
2. Sube los archivos `index.html`, `admin.html` y las imágenes
3. Ve a **Settings** → **Pages**
4. Selecciona la rama `main` y carpeta `/ (root)`
5. Tu tienda estará en `https://tuusuario.github.io/chicassheinune/`

### Opción 2: Netlify

1. Ve a [netlify.com](https://netlify.com)
2. Arrastra la carpeta del proyecto al área indicada
3. ¡Listo! Netlify te dará una URL instantánea

### Opción 3: Vercel

1. Ve a [vercel.com](https://vercel.com)
2. Importa tu repositorio de GitHub
3. Selecciona el framework "Other"
4. ¡Desplegado automáticamente!

---

## 🔐 Acceso al Panel de Administración

### URL
```
https://tu-dominio.com/admin.html
```

### Credenciales

| Usuario | Contraseña |
|---------|------------|
| **Ernesto** | `ERF*010701` |
| **Gladys** | `GFS*010203` |

### Funcionalidades del Admin

- 📊 **Dashboard** - Estadísticas visuales de productos y categorías
- 📦 **Inventario** - Vista de todos los productos en modo solo lectura
- 🗂️ **Categorías** - Gestión visual informativa de categorías

> ⚠️ **IMPORTANTE**: El panel de administración NO permite añadir, editar ni eliminar productos. El catálogo es 100% estático.

---

## 🔄 Cómo Añadir Nuevos Productos

Como el catálogo es **100% estático**, para añadir nuevos productos debes:

### Paso 1: Preparar la Información

Reúne la siguiente información para cada producto:
- 📸 **Imagen** del producto (modelo con fondo blanco)
- 🏷️ **Nombre** del producto
- 💰 **Precio** en CUP (solo número, sin símbolos)
- 📂 **Categoría** (Vestidos, Blusas, Pantalones, Abrigos, Camisas, Faldas, Accesorios, Personalizadas)
- ✨ **¿Es nuevo?** (true/false)

### Paso 2: Contactar al Desarrollador

Envía la información de los nuevos productos a tu asistente IA con el siguiente mensaje:

```
Hola, necesito añadir nuevos productos a Chic@s SheinUNE:

Producto 1:
- Nombre: [nombre]
- Precio: [precio]
- Categoría: [categoría]
- Es nuevo: [sí/no]

Producto 2:
...

Por favor regenera el código con el catálogo actualizado incluyendo todos los productos anteriores más estos nuevos.
```

### Paso 3: Actualizar los Archivos

El desarrollador te proporcionará:
- Nuevo archivo `index.html`
- Nuevo archivo `admin.html`

Solo reemplaza estos archivos en tu hosting y ¡listo!

---

## 🖼️ Cómo Reemplazar las Imágenes

### Requisitos de las Imágenes

- **Formato**: JPG, PNG o WebP
- **Tamaño máximo**: 500 KB por imagen
- **Dimensiones recomendadas**: 800x1000px (ratio 4:5)
- **Estilo**: Modelo humano o maniquí invisible + Fondo blanco puro (#ffffff)

### Pasos para Reemplazar

1. **Prepara tus imágenes**:
   - Comprime las imágenes a formato WebP para mejor rendimiento
   - Usa herramientas como [TinyPNG](https://tinypng.com/) o [Squoosh](https://squoosh.app/)

2. **Sube las imágenes**:
   - Sube las imágenes a la misma carpeta donde están los archivos HTML
   - O usa un servicio de hosting de imágenes como Cloudinary, Imgur, etc.

3. **Actualiza las rutas** (si es necesario):
   - Si las imágenes están en la misma carpeta: `nombre-imagen.jpg`
   - Si están en una subcarpeta: `imagenes/nombre-imagen.jpg`
   - Si están en URL externa: `https://ejemplo.com/imagen.jpg`

---

## ⚙️ Personalización

### Cambiar Colores

Los colores principales están definidos en las variables CSS al inicio de cada archivo:

```css
:root {
    --accent-pink: #ff6b9d;      /* Rosa principal */
    --accent-violet: #6c5ce7;    /* Violeta */
    --accent-turquoise: #00cec9; /* Turquesa */
    --accent-gold: #fdcb6e;      /* Dorado */
}
```

### Cambiar Números de WhatsApp

Busca en el código:
```javascript
whatsappNumber: "5358472238"  // Ernesto
whatsappNumber: "5353848949"  // Gladys
```

### Cambiar Textos

Busca las cadenas de texto en el HTML y modifícalas directamente.

---

## 📱 Optimización para Cuba

### Conexiones Lentas

- ✅ Imágenes con carga diferida (lazy loading)
- ✅ CSS y JavaScript embebidos (sin peticiones externas)
- ✅ Sin librerías pesadas
- ✅ Solo iconos vía CDN (Phosphor Icons)

### Dispositivos Móviles

- ✅ Diseño mobile-first
- ✅ Botones de fácil toque (mínimo 44px)
- ✅ Textos legibles sin zoom
- ✅ Menú hamburguesa en móvil

---

## 🛡️ Seguridad

- ✅ Contraseñas ofuscadas en el código
- ✅ Sanitización de datos en inputs
- ✅ Sesión guardada en localStorage del navegador
- ✅ Recomendado: Usar hosting con SSL (HTTPS)

---

## ♿ Accesibilidad

- ✅ Contraste de texto cumple WCAG 4.5:1
- ✅ Estados de foco visibles
- ✅ Etiquetas ARIA en elementos interactivos
- ✅ Navegación por teclado completa
- ✅ Textos alternativos en imágenes

---

## 🐛 Solución de Problemas

### La página no carga
- Verifica que todos los archivos estén en la misma carpeta
- Comprueba que las imágenes existan en las rutas especificadas

### Los productos no aparecen
- Abre la consola del navegador (F12) y verifica errores
- Asegúrate de que el array `PRODUCTS` tenga datos válidos

### El login no funciona
- Verifica que las credenciales sean correctas
- Limpia el localStorage del navegador y recarga

### Las imágenes no se ven
- Verifica que las rutas de las imágenes sean correctas
- Comprueba que las imágenes existan en el servidor

---

## 📞 Soporte

Para cualquier consulta, modificación o actualización del catálogo:

- 📱 **Ernesto**: +53 58472238
- 📱 **Gladys**: +53 53848949
- 🕐 **Horario**: Lunes a Sábado, 9:00 AM - 6:00 PM

---

## 📝 Notas Importantes

> ⚠️ **CATÁLOGO ESTÁTICO**: Esta tienda no tiene base de datos. Los productos están integrados directamente en el código JavaScript. Para añadir o modificar productos, contacta al desarrollador.

> ⚠️ **SIN UBICACIÓN**: Esta tienda no incluye mapas, direcciones físicas ni referencias geográficas de ningún tipo.

> ⚠️ **CATEGORÍA "ABRIGOS"**: La categoría se llama "Abrigos", no "Sacos". Esta modificación está aplicada en toda la web.

---

## 📄 Licencia

© 2026 Chic@s SheinUNE. Todos los derechos reservados.

---

## 🙏 Agradecimientos

Diseñado y desarrollado con ❤️ para el negocio de Ernesto y Gladys en Cuba.

**¡Gracias por confiar en nosotros!**
