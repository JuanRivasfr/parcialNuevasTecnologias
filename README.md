# 🛒 Sistema de Ventas y Administración

Aplicación para gestionar ventas en mostrador y administración de clientes/productos.

---

## ✨ Funcionalidades principales

- 📦 **Pedidos múltiples**: Se pueden realizar pedidos con varios productos al mismo tiempo.  
- 🏷️ **Venta por defecto**: Todas las ventas se registran inicialmente como **mostrador**.  
- 🧾 **Facturación a clientes**:  
  - Para facturar una venta, el cliente debe estar registrado previamente.  
  - Si el cliente no existe, debe crearse antes de la venta.  

---

## 🚏 Rutas principales

| Ruta    | Descripción                        |
|---------|------------------------------------|
| `/pos`  | Punto de venta (vitrina)           |
| `/admin`| Panel de administración (CRUD)     |

---

## 🖥️ Detalles de cada vista

### 🔹 POS (`/pos`)
- Permite la **venta de productos en vitrina**.  
- Si la venta requiere factura:  
  - Se solicita la **identificación del cliente**.  
  - Si no existe, se debe **crear primero el cliente**.  

### 🔹 Admin (`/admin`)
- Vista **CRUD** para gestión de:  
  - 🛍️ Productos  
  - 👥 Clientes  
- Incluye **informe de ventas**.  
- ⚠️ **Restricción**:  
  - No se puede eliminar ningún **producto** ni **cliente** que esté registrado en alguna venta.  

---

## 📂 Estructura básica

```bash
├── /pos        # Punto de venta
├── /admin      # Administración
└── README.md   # Documentación del proyecto
