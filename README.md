# 🌿 FloraScan - Identificador Inteligente de Plantas

Aplicación web progresiva (PWA), completamente responsiva (optimizada tanto para teléfonos móviles como para ordenadores de sobremesa), diseñada para identificar especies de plantas a través de fotografías tomadas al instante con la cámara o subidas desde el explorador de archivos.

---

## ✨ Características Principales

- 📱 **Diseño 100% Adaptable:** Interfaz moderna y táctil inspirada en aplicaciones móviles nativas y óptima para pantallas grandes.
- 📸 **Captura con Cámara:** En móviles abre la cámara trasera nativa mediante el atributo `capture="environment"`; en PC activa un visor web interactivo en tiempo real con guía de enfoque.
- 📁 **Subida Fácil:** Arrastra y suelta imágenes (*drag & drop*) o selecciona archivos desde tu dispositivo (JPG, PNG, WebP).
- 🔬 **Ficha Botánica Detallada:**
  - Nombre común y nombre científico binomial.
  - Familia taxonómica y hábitat.
  - Nivel de coincidencia / precisión estimada.
  - Requisitos de iluminación solar, pautas de riego y tolerancia térmica.
  - Nivel de toxicidad para animales domésticos y consejos prácticos de mantenimiento.
- 🕘 **Historial de Escaneos:** Guarda tus últimas identificaciones localmente (`localStorage`).
- 🌐 **Soporte PWA / Offline:** Incluye `manifest.json` y `Service Worker` para instalarse en el dispositivo como app.
- ⚙️ **Modos Flexibles:**
  - **Demo Local (Predeterminado):** Funciona al instante sin necesidad de claves de API ni coste alguno.
  - **Pl@ntNet API:** Conexión opcional con la base de datos botánica global de Pl@ntNet.
  - **Plant.id API (Kindwise):** Reconocimiento de alta precisión botánica por IA.

---

## 🚀 Cómo Subir este Proyecto a GitHub y Publicarlo Gratis

### Paso 1: Inicializar Git
Abre una terminal en la carpeta descomprimida del proyecto y ejecuta:

```bash
git init
git add .
git commit -m "Initial commit: FloraScan Web App"
```

### Paso 2: Crear el repositorio en GitHub
1. Entra en tu cuenta de [GitHub](https://github.com/) y haz clic en **New repository**.
2. Dale un nombre, por ejemplo: `florascan` o `identificador-plantas`.
3. Deja la opción pública y no marques la casilla de añadir README (ya lo tenemos). Haz clic en **Create repository**.

### Paso 3: Subir los archivos
Copia los comandos que te muestra GitHub o usa los siguientes (sustituyendo tu usuario y nombre del repo):

```bash
git branch -M main
git remote add origin https://github.com/TU-USUARIO/florascan.git
git push -u origin main
```

### Paso 4: Publicar gratis en GitHub Pages
1. En tu repositorio en GitHub, ve a la pestaña **Settings** (Ajustes).
2. En el menú lateral izquierdo, haz clic en **Pages**.
3. Bajo el apartado **Build and deployment > Branch**, selecciona `main` y en la carpeta elige `/(root)`.
4. Haz clic en **Save**.
5. Espera unos segundos y GitHub te mostrará tu URL pública:
   `https://TU-USUARIO.github.io/florascan/`

¡Ya tienes tu aplicación funcionando en vivo en Internet!

---

## 📂 Estructura del Repositorio

```
├── index.html            # Interfaz principal semántica
├── css/
│   └── styles.css        # Hoja de estilos moderna y adaptativa
├── js/
│   ├── app.js            # Interfaz de usuario, cámara y eventos
│   ├── api.js            # Integraciones de identificación (Demo, Pl@ntNet, Plant.id)
│   └── mock-db.js        # Base de datos botánica local
├── icons/
│   ├── icon-192.png      # Icono PWA (192x192)
│   └── icon-512.png      # Icono PWA de alta resolución (512x512)
├── manifest.json         # Configuración PWA
├── sw.js                 # Service worker
├── .gitignore            # Archivos ignorados por Git
├── LICENSE               # Licencia MIT
└── README.md             # Guía del proyecto
```
