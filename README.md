# Sitio Web Utilizando Tailwind CSS

Este sitio web está desarrollado utilizando Tailwind CSS, un marco de trabajo de utilidad de CSS de bajo nivel.

## Instalación de Tailwind CSS

Para utilizar Tailwind CSS en tu proyecto, primero debes instalarlo a través de npm:

```bash
npm install -D tailwindcss
```

Crea un archivo tailwind.css, asegúrate de que Tailwind CSS esté incluido en tu archivo de CSS:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

Generar archivo de configurarcion de Tailwind CSS

```bash
npx tailwindcss init
```

Tailwind CSS es altamente personalizable. Puedes modificar el archivo tailwind.config.js para ajustar los colores, márgenes, rellenos y más según las necesidades de tu proyecto.

## Implementación de Vite en un Proyecto Existente

Vite es una herramienta de desarrollo rápida para proyectos web modernos que puede integrarse fácilmente en proyectos existentes. A continuación, se detallan los pasos para agregar Vite a tu proyecto:

### Paso 1: Instalar las siguientes dependencias de desarrollo

```bash
npm install -D vite postcss autoprefixer
```

### Paso 2: Generar archivo de configuración PostCSS

```bash
npx tailwindcss init -p
```

### Paso 3: Modificar los scripts en el archivo package.json para integrar Vite

```json
"scripts": {
    "dev": "vite", // Ejecutar Vite en modo de desarrollo
    "build": "vite build", // Construir la aplicación para producción
    "serve": "vite preview" // Servir la aplicación construida localmente
  }
```

### Paso 4: Asegurate de enlazar tailwind.css a tu archivo HTML

```html
<link rel="stylesheet" href="./tailwind.css" />
```

## Formateo y orden de clases Automático

Instalar Prettier y el plugin prettier-plugin-tailwindcss como dependencias de desarrollo en tu proyecto, puedes ejecutar los siguientes comandos:

```bash
npm install -D prettier prettier-plugin-tailwindcss
```

1. instalar la extensión de ["Prettier - Code formatter"](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) en Visual Studio Code

2. En Visual Studio Code haz clic en Archivo (File) en la barra de menú.
   Selecciona Preferencias (Preferences) y luego Configuración (Settings) o simplemente presiona Ctrl+, (Control más coma).

En la barra de busqueda escribe "format". Asegurate de tener los siguientes item.
![Ejemplo de configuracion.](https://raw.githubusercontent.com/johinnerMC/cloud-images/master/guia/format.jpg)

3. Crea un archivo de configuración ".prettierrc" que se utiliza para especificar las reglas de formato que Prettier debe seguir al formatear tu código.

4. A continuación, añade el plugin a tu archivo de configuración de Prettier:

```json
{
  "plugins": ["prettier-plugin-tailwindcss"]
}
```

El plugin prettier-plugin-tailwindcss te permitirá formatear de manera adecuada las clases de Tailwind CSS en tu código cuando utilices Prettier.

## Recursos Adicionales

- Documentación de Tailwind CSS: https://tailwindcss.com/docs
- Repositorio de Tailwind CSS en GitHub: https://github.com/tailwindlabs/tailwindcss
- Documentación de Vite: https://vitejs.dev/guide/
