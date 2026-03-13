# Cine Use Popcorn

Una aplicación web desarrollada en React para buscar películas y gestionar una lista de películas vistas. Utiliza la API de OMDB para obtener información sobre películas.

## Características

- **Búsqueda de películas**: Busca películas por título utilizando la API de OMDB
- **Detalles de película**: Ver información detallada de cada película (año, género, puntuación, sinopsis, etc.)
- **Lista de vistas**: Guarda las películas que has visto en localStorage
- **Puntuación personalizada**: Califica las películas vistas con estrellas
- **Persistencia de datos**: Los datos se almacenan en el navegador del usuario

## Estructura del Proyecto

```
cine-use-popcorn/
├── public/
│   ├── index.html
│   ├── manifest.json
│   ├── logo192.png
│   └── logo512.png
├── src/
│   ├── custom_hooks/
│   │   ├── useKey.js         # Hook personalizado para atajos de teclado
│   │   ├── useLocalStorageState.js  # Hook para gestionar estado en localStorage
│   │   └── useMovies.js     # Hook para fetching de películas
│   ├── App.css              # Estilos principales
│   ├── App.js               # Componente principal de la aplicación
│   ├── App-v1.js            # Versión inicial de la app
│   ├── App-v3.js            # Versión alternativa
│   ├── App-section12.js     # Versión de la sección 12
│   ├── StarRating.js        # Componente de calificación por estrellas
│   ├── index.css            # Estilos globales
│   └── index.js             # Punto de entrada de React
├── .gitignore
├── package.json
├── package-lock.json
└── README.md
```

## Requisitos Previos

- Node.js (versión 14 o superior)
- npm o yarn

## Instalación

1. **Clona el repositorio:**

   ```bash
   git clone <url-del-repositorio>
   cd cine-use-popcorn
   ```

2. **Instala las dependencias:**

   ```bash
   npm install
   ```

   o si prefieres usar yarn:

   ```bash
   yarn install
   ```

## Ejecución

### Modo desarrollo

Para iniciar la aplicación en modo desarrollo:

```bash
npm start
```

Esto abrirá la aplicación en [http://localhost:3000](http://localhost:3000).

### Producción

Para crear una versión de producción:

```bash
npm run build
```

Los archivos optimizados se generarán en la carpeta `build`.

## Scripts Disponibles

- `npm start`: Inicia el servidor de desarrollo
- `npm run build`: Crea la versión de producción
- `npm test`: Ejecuta las pruebas
- `npm run eject`: Expulsa la configuración de Create React App

## Dependencias

- **React**: ^19.2.0 - Biblioteca de JavaScript para construir interfaces de usuario
- **React DOM**: ^19.2.0 - Renderizado de React para el DOM
- **React Scripts**: 5.0.1 - Scripts y configuración para Create React App

## API Utilizada

Este proyecto utiliza la [API de OMDB](http://www.omdbapi.com/) para obtener información sobre películas. La API key configurada es `f315037`.

## Hooks Personalizados

La aplicación hace uso de varios hooks personalizados:

- **useMovies**: Maneja la búsqueda y obtención de películas desde la API
- **useLocalStorageState**: Gestiona el estado persistido en localStorage
- **useKey**: Permite usar atajos de teclado en la aplicación

## Contribución

Si deseas contribuir al proyecto, por favor abre un issue o crea un pull request.

## Licencia

MIT
