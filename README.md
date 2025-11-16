# Invoice Scanner

Aplicación web para la gestión y procesamiento de facturas con capacidades de reconocimiento óptico de caracteres (OCR) y análisis de datos.

## 📋 Descripción del Proyecto

Invoice Scanner es una aplicación web diseñada para facilitar la gestión de facturas para usuarios. El proyecto permite a los usuarios subir facturas y procesarlas mediante dos métodos principales:

- **Autollenado vía OCR**: Reconocimiento automático de texto y datos mediante tecnología OCR
- **Llenado manual**: Opción para ingresar datos manualmente cuando sea necesario

Los datos de las facturas se almacenan en la nube, permitiendo:
- Análisis de datos sobre gastos
- Generación de reportes y estadísticas
- Otras funcionalidades que se implementarán según la demanda de los usuarios

Adicionalmente, la aplicación incluye funcionalidades de respaldo, permitiendo exportar los datos a hojas de cálculo como Excel.

## ⚠️ Estado del Proyecto

**Este proyecto se encuentra actualmente en desarrollo.**

## 📄 Licencia

El prototipo está idealmente pensado para ser de código abierto, conservando la autoría del código.

## 🛠️ Tecnologías

Este proyecto utiliza [Nuxt 3](https://nuxt.com/). Para más información sobre Nuxt, consulta la [documentación oficial](https://nuxt.com/docs/getting-started/introduction).

## 🚀 Configuración

Instala las dependencias del proyecto:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## 💻 Servidor de Desarrollo

Inicia el servidor de desarrollo en `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## 🏗️ Producción

Compila la aplicación para producción:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Previsualiza localmente la build de producción:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Consulta la [documentación de deployment](https://nuxt.com/docs/getting-started/deployment) para más información.
