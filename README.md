# Administrador de Convenios - Maquetación estática

Este proyecto contiene las vistas estáticas del administrador de convenios solicitadas: una página principal con la lista de convenios aliados y una pantalla para la creación de nuevos convenios. No hay integración con APIs ni lógica dinámica; todo el contenido es puramente HTML y CSS.

## Requisitos previos

No es necesario instalar dependencias ni contar con un entorno de compilación. Solo necesitas un navegador web moderno (Chrome, Firefox, Edge, Safari, etc.).

## Clonar o descargar el proyecto

```bash
# Clonar el repositorio
git clone <URL_DEL_REPOSITORIO>
cd Xpert-Convenio-Maq
```

Si recibiste los archivos comprimidos, simplemente descomprímelos y ubícate en la carpeta `Xpert-Convenio-Maq`.

## Ejecutar en local

Existen dos formas sencillas de visualizar la maqueta:

### 1. Abrir directamente los archivos HTML

1. Navega hasta la carpeta del proyecto.
2. Abre `index.html` haciendo doble clic o arrastrándolo a la ventana del navegador.
3. Desde la página principal podrás navegar a `create-convenio.html` mediante el botón **"+ Nuevo convenio"**.

> Nota: Al abrir los archivos directamente, algunos navegadores podrían bloquear fuentes externas por políticas de seguridad. Si notas diferencias en la tipografía, utiliza la opción 2.

### 2. Servir el proyecto con un servidor estático

Puedes levantar un servidor HTTP simple para que los recursos se carguen exactamente igual que en producción. A continuación algunas opciones:

#### Con Python (viene instalado en la mayoría de sistemas)

```bash
# Dentro de la carpeta del proyecto
python3 -m http.server 5173
```

Luego abre en el navegador: [http://localhost:5173/index.html](http://localhost:5173/index.html)

#### Con Node.js (`npx serve`)

```bash
# Dentro de la carpeta del proyecto
npx serve .
```

El comando mostrará la URL local (usualmente `http://localhost:3000`). Ingresa en el navegador y navega a `index.html`.

#### Extensiones como Live Server (VS Code)

1. Abre la carpeta del proyecto en VS Code.
2. Instala y activa la extensión **Live Server**.
3. Haz clic derecho sobre `index.html` y elige **Open with Live Server**.

## Estructura del proyecto

```
Xpert-Convenio-Maq/
├── index.html              # Landing de administrador de convenios
├── create-convenio.html    # Formulario para crear un convenio
├── styles/
│   ├── main.css            # Estilos de la página principal
│   └── create.css          # Estilos del formulario de convenios
└── README.md               # Este archivo con las instrucciones
```

## Personalización

Puedes editar los archivos HTML y CSS según las necesidades del proyecto. No hay herramientas de build, por lo que los cambios se reflejarán inmediatamente al recargar la página.

## Próximos pasos sugeridos

- Integrar la maqueta con datos reales consumiendo APIs.
- Añadir validaciones y lógica de formularios.
- Configurar un bundler o framework si se requiere escalar la solución.

¡Disfruta explorando el prototipo! Si tienes preguntas o necesitas ajustes adicionales, no dudes en indicarlo.
