# Sitio Web Utilizando Tailwind CSS

Este sitio web está desarrollado utilizando Tailwind CSS, un marco de trabajo de utilidad de CSS de bajo nivel.

## Instalación de Tailwind CSS

Para utilizar Tailwind CSS en tu proyecto, primero debes instalarlo a través de npm:
```bash
npm install -D tailwindcss
```
Crea un archivo tailwind.css, asegúrate de que Tailwind CSS esté incluido en tu archivo de CSS:

*<span style="color:blue;">@tailwind</span> base;*   
*<span style="color:blue;">@tailwind</span> components;*   
*<span style="color:blue;">@tailwind</span> utilities;*

Generar archivo de configurarcion de Tailwind CSS
```bash
npx tailwindcss init
```
Tailwind CSS es altamente personalizable. Puedes modificar el archivo tailwind.config.js para ajustar los colores, márgenes, rellenos y más según las necesidades de tu proyecto.


## Implementación de Vite en un Proyecto Existente
Vite es una herramienta de desarrollo rápida para proyectos web modernos que puede integrarse fácilmente en proyectos existentes. A continuación, se detallan los pasos para agregar Vite a tu proyecto:


### Paso 1: Instalar las siguientes dependencias
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
```json
<link rel="stylesheet" href="./tailwind.css">
```


## Recursos Adicionales
* Documentación de Tailwind CSS: https://tailwindcss.com/docs  
* Repositorio de Tailwind CSS en GitHub: https://github.com/tailwindlabs/tailwindcss
* Documentación de Vite: https://vitejs.dev/guide/