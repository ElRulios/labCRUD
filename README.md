# CRUD de Productos - Laravel

Sistema básico para gestionar productos con Laravel.

## ¿Qué hace?

- Ver lista de productos
- Crear nuevos productos
- Editar productos
- Eliminar productos

## Requisitos

- PHP 8.2 o superior
- Composer
- MySQL
- Node.js y NPM

## Instalación

### 1. Descargar el proyecto

```bash
git clone <tu-repositorio>
cd crud
```

### 2. Instalar dependencias

```bash
composer install
npm install
```

### 3. Configurar

Copia el archivo de configuración:

```bash
cp .env.example .env
php artisan key:generate
```

### 4. Configurar base de datos

Edita el archivo `.env` con tus datos de MySQL:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=tu_base_datos
DB_USERNAME=tu_usuario
DB_PASSWORD=tu_contraseña
```

### 5. Crear tablas

```bash
php artisan migrate
```

### 6. Compilar recursos

```bash
npm run build
```

## Usar la aplicación

Inicia el servidor:

```bash
php artisan serve
```

Abre en tu navegador: **http://127.0.0.1:8000/products**

## Estructura de la Base de Datos

La tabla `products` tiene:
- **description**: Nombre del producto
- **price**: Precio
- **stock**: Cantidad disponible

## Tecnologías

- Laravel 11
- Bootstrap 5
- MySQL

## Comandos útiles

```bash
# Ver todas las rutas
php artisan route:list

# Limpiar caché
php artisan cache:clear

# Reiniciar base de datos
php artisan migrate:fresh
```

## Problemas comunes

**Error de base de datos**: Verifica que el nombre de la base de datos en `.env` sea correcto y que exista.

**Error de Vite**: Ejecuta `npm run build`.

---

Desarrollado con Laravel - Joaquin Lu Zheng
