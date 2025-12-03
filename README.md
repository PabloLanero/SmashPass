# SmashPass
Este proyecto es para la asignatura de desarrollo de interfaces

## Ver la versión Desktop y Mobile

- **Reglas principales:** los estilos son mobile-first. A partir de **425px** (min-width: 425px) se aplican las reglas para la versión desktop.
- Los archivos SCSS están en `styles/` y se compilan a CSS que debe enlazarse desde las páginas en `frontend/`.

## Cómo visualizarlo localmente

1. Opción rápida (sin compilar SCSS):
	- Abre la carpeta `frontend/` en tu editor y sirve la carpeta con Live Server o abre `frontend/index.html` en el navegador.
	- Las páginas usan `index.css` dentro de `frontend/`. Si quieres ver los cambios de SCSS, compila primero (ver opción 2).

2. Opción recomendada (compilar SCSS a CSS):
	- Instala Dart Sass si no lo tienes: `npm install -g sass` (PowerShell)
	- Compila SCSS a CSS (ejemplo, genera `frontend/index.css` a partir del entry `styles/main.scss`):

```powershell
npm install -g sass;
sass --no-source-map --style=expanded ./styles/main.scss:./frontend/index.css
```

3. Abrir en el navegador y probar breakpoints:
	- Abre `frontend/index.html` en el navegador o usa Live Server.
	- Abre las herramientas de desarrollador y cambia el ancho de la ventana; verifica que a partir de **425px** se aplique la disposición desktop (dos columnas en landing, inputs y tarjetas más anchos, etc.).

Si quieres, puedo ejecutar la compilación SCSS y generar `frontend/index.css` aquí mismo. ¿Quieres que la compile ahora? 
