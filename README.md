# Aplicación de Gestión de Inventarios y Ventas para BookWorld

## Descripción

Este proyecto consiste en una aplicación de consola en Java para gestionar las operaciones principales de BookWorld, una librería. La aplicación permite realizar las siguientes funciones esenciales:

- **Gestión de Inventario:** Agregar, actualizar, eliminar y listar productos disponibles en el inventario.
- **Gestión de Clientes:** Agregar, actualizar, eliminar y listar clientes.
- **Ventas y Facturación:** Registrar ventas, calcular ventas totales y generar reportes.
- **Consultas y Reportes:** Consultar ventas totales, ventas de los últimos tres meses, y los cinco clientes que más gastan.

La aplicación se conecta a una base de datos MySQL a través de JDBC para manejar las operaciones CRUD y generar reportes.

## Tecnologías Usadas

- **Lenguaje de Programación:** Java
- **Base de Datos:** MySQL
- **Conexión a la Base de Datos:** JDBC (Java Database Connectivity)
- **Entorno de Desarrollo:** Eclipse / IntelliJ IDEA

## Requisitos

Para ejecutar este proyecto, necesitarás tener los siguientes programas y librerías instalados:

- **Java 8 o superior**
- **MySQL Server**: Para crear y gestionar la base de datos.
- **JDBC Driver para MySQL**: Para la conexión de la aplicación con MySQL.

### Instalación

1. **Clonar el Repositorio:**

   Si aún no tienes el repositorio en tu máquina local, clónalo usando el siguiente comando:

   ```bash
   git clone https://github.com/tu-usuario/libros-gestión.git
Configurar la Base de Datos:

Crea una base de datos en MySQL llamada bookworld_db.
Importa el archivo script.sql para crear las tablas necesarias (Producto, Cliente, Venta).
Configurar la Conexión a la Base de Datos:

Abre el archivo ConexiónBaseDatos.java y modifica los parámetros de la conexión según tu configuración de MySQL.
Ejecutar el Proyecto:

Una vez que la base de datos esté configurada, ejecuta la clase MenuPrincipal.java para iniciar la aplicación.

bash
Copiar código
java MenuPrincipal
Estructura del Proyecto
El proyecto está organizado de la siguiente manera:

graphql
Copiar código
/BookWorldGestión
│
├── src/
│   ├── ConexiónBaseDatos.java       # Clase para gestionar la conexión a la base de datos
│   ├── ProductoDAO.java             # Clase para las operaciones CRUD de productos
│   ├── ClienteDAO.java             # Clase para las operaciones CRUD de clientes
│   ├── VentaDAO.java               # Clase para las operaciones CRUD de ventas
│   ├── MenuPrincipal.java          # Menú interactivo de la aplicación
│   └── script.sql                  # Script SQL para crear la base de datos y tablas
└── README.md                       # Este archivo
Funcionalidades
Gestión de Inventario
Agregar Producto: Permite agregar nuevos productos al inventario con su nombre, precio y cantidad.
Actualizar Producto: Permite modificar las propiedades de un producto existente.
Eliminar Producto: Elimina un producto del inventario.
Listar Productos: Muestra todos los productos registrados en el inventario.
Gestión de Clientes
Agregar Cliente: Registra un nuevo cliente con su información personal y de contacto.
Actualizar Cliente: Permite modificar la información de un cliente.
Eliminar Cliente: Elimina un cliente de la base de datos.
Listar Clientes: Muestra todos los clientes registrados.
Ventas y Facturación
Registrar Venta: Permite registrar una nueva venta, asociando un cliente y producto con una cantidad vendida.
Ventas Totales: Consulta el total de ingresos generados por todas las ventas.
Ventas Últimos 3 Meses: Consulta las ventas realizadas en los últimos tres meses.
Top 5 Clientes: Consulta los cinco clientes que más han gastado en la tienda.
Consultas y Reportes
Ventas Totales: Muestra un reporte de las ventas totales realizadas.
Ventas Últimos 3 Meses: Genera un reporte de las ventas realizadas en los últimos tres meses.
Top 5 Clientes: Genera un reporte de los cinco clientes que más han gastado en la librería.
Ejemplo de Ejecución
Menu Principal: Al ejecutar la aplicación, verás un menú con las siguientes opciones:

markdown
Copiar código
1. Gestión de Inventario
2. Gestión de Clientes
3. Ventas y Facturación
4. Consultas y Reportes
5. Salir
Operaciones CRUD: Cada módulo tiene submenús para gestionar los productos, clientes y ventas.

Ejemplo de Gestión de Inventario:

markdown
Copiar código
1. Agregar Producto
2. Actualizar Producto
3. Eliminar Producto
4. Listar Productos
Después de realizar una operación, la aplicación actualizará la base de datos y mostrará un mensaje de confirmación.

Pruebas
Para garantizar el correcto funcionamiento de la aplicación, se han realizado pruebas exhaustivas de las operaciones CRUD y generación de reportes. Cada una de las funciones ha sido probada con datos de ejemplo, y se han corregido errores de manejo de excepciones y rendimiento.

Resultados de las Pruebas:
Prueba de Agregar Producto: El producto se agrega correctamente en la base de datos.
Prueba de Actualizar Producto: El producto se actualiza correctamente y se refleja en la base de datos.
Prueba de Registrar Venta: La venta se registra correctamente y se genera un reporte de ventas.
Bibliografía
DuBois, S. (2016). Java for Absolute Beginners: Learn to Program the Fundamentals the Java 9+ Way. Apress.
MySQL. (n.d.). MySQL 8.0 Reference Manual. Recuperado de https://dev.mysql.com/doc/
Oracle. (n.d.). Java Database Connectivity (JDBC) Overview. Recuperado de https://docs.oracle.com/javase/
Farquhar, M., & Cotten, T. (2020). Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems. O'Reilly Media.
Techopedia. (n.d.). CRUD Operations. Recuperado de https://www.techopedia.com/
Contribuciones
Si deseas contribuir a este proyecto, por favor sigue estos pasos:

Haz un fork de este repositorio.
Crea una nueva rama (git checkout -b feature/nueva-funcionalidad).
Realiza tus cambios y haz commit (git commit -am 'Agregué nueva funcionalidad').
Haz push a tu rama (git push origin feature/nueva-funcionalidad).
Abre un Pull Request.
