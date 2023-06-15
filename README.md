# TailWind CSS Instalación
En este proyecto instalé TailWind CSS como Using PostCSS, puedes ver más instalaciones en la documentación de TailWind CSS.

# Descargar módulos
Para descargar los módulos que necesita este proyecto, ejecuta el siguiente comando en la terminal de tu editor de código:
  - npm install -D tailwindcss postcss autoprefixer

(Recomiendo que si la instalación noi)

# Archivo de configuración
  -npx tailwindcss init
                    Se ejecuta el siguiente comando npx tailwindcss init para crear el archivo de configuracion o de plantillas tailwind.config.js colocando la siguiente configuración:
                                module.exports = {
                                content: ["./public/index.html", "./src/**/*.{html,js}"],
                                theme: {
                                    extend: {},
                                },
                                plugins: [],
                                };


# Desde 0
    Vamos a importar TailWind a nuestra hoja de estilos .css (de src)
        Incluir Tailwind en el CSS agregando las directivas a src/css/tailwind.css

        Nos vamos a copiar estas lineas para importar src/css/tailwind.css
            @tailwind base;
            @tailwind components;
            @tailwind utilities;

------------------------------------------------------------------------------------------------
    Ejecutamos este comando 

        npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch

        Las rutas en este caso serian
            npx tailwindcss -i ./src/css/tailwind.css -o ./public/css/tailwind.css --watch

        ¿Que hace esto?
            genera un build o un contructor desde  src/css/tailwind.css a nuestra carpeta public/css/tailwind.css
            
       
        Ya se podría usar clases de tailwind en el index
