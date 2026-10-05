# Tienda en React: hooks, formularios y navegación

Proyecto de referencia para la asignatura **DSY1104 · Desarrollo Full Stack II** (Duoc UC).

Una tienda pequeña de tecnología, construida con React, Vite y React Bootstrap. Es un **material de estudio**, no una aplicación de producción: está recortada a propósito para mostrar solo lo que las guías del curso enseñan (catálogo con filtro por categoría y búsqueda, carrito, inicio de sesión con validación, y un panel simple de administración de productos), sin pantallas extra que no se explican en ninguna guía.

**Todos los componentes reciben sus datos por `props` y los leen con `props.algo`** (por ejemplo `props.onClick`, `props.children`), tal como se enseña en el curso — sin destructuring en los parámetros de función.

Este repositorio muestra la tienda **funcionando**, sin pruebas unitarias. Si buscas el mismo proyecto pero con las pruebas con Vitest ya agregadas, está en `dsy1104-pruebas-unitarias-vitest`.

## Estructura

```
src/
├── components/
│   ├── atoms/        Button, Badge, Precio
│   ├── molecules/     CampoFormulario, ProductCard, CartItem
│   ├── organisms/     Navbar, Footer, ProductCatalog, FormularioLogin, ShoppingCart
│   └── templates/     PlantillaPublica
├── pages/             Catalogo, Carrito, Login, AdminProductos, NoEncontrada
├── context/           CartContext, ProductosContext
├── services/          productoService (el CRUD)
├── hooks/             useTituloPagina
├── data/              productos.json
├── utils/             formatoPrecio, validaciones, filtrarProductos, categorias
└── App.jsx            las rutas
```

## Cómo instalar y ejecutar

```bash
npm install
npm run dev
```
