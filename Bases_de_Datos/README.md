# 📊 Bases de Datos - Proyecto PlayToPlay

Bienvenido al apartado de **Bases de Datos** de nuestro proyecto. Aquí es donde hemos diseñado toda la "memoria" de la tienda. Sin una estructura de datos bien pensada, sería imposible saber qué hemos vendido, quién se ha apuntado a un torneo o qué nos queda en el almacén.

## 📋 Sobre este módulo
En esta parte del proyecto me he centrado en crear la arquitectura lógica que permite a **PlayToPlay** funcionar como un negocio organizado. No se trata solo de guardar nombres en una lista, sino de que toda la información esté conectada: que sepamos qué empleado ha realizado una venta, qué productos se han llevado los clientes o quiénes son los participantes de nuestros eventos.

## 🛠️ Diseño Lógico (Modelo Entidad-Relación)

### La Estructura
He diseñado un diagrama **Entidad-Relación** que sirve como el mapa de toda nuestra información. En él hemos definido cinco pilares fundamentales para el negocio:
* **Clientes:** El registro de nuestra comunidad y jugadores.
* **Productos:** Todo el inventario, desde el hardware que monta Eme hasta los periféricos gaming.
* **Empleados:** El equipo técnico y de ventas (Ro, Juan y Eme).
* **Ventas:** El historial detallado de cada transacción en mostrador.
* **Torneos:** La gestión de los eventos competitivos que dan vida a la zona polivalente.

### Relaciones Clave
Para que la base de datos sea realmente útil, hemos creado conexiones que reflejan el día a día de la tienda:
* **Control de Ventas:** Cada ticket está vinculado a un empleado y a un cliente, asegurando que el proceso comercial sea transparente.
* **Gestión de Torneos:** Conectamos a los clientes con los eventos para controlar inscripciones, dorsales y fechas.
* **Ciclo de Premios:** Los productos del stock se vinculan directamente como premios de los torneos, cerrando el círculo entre la competición y la venta.

## 🚀 Conclusión Técnica
Este diseño garantiza que la información sea fiable y que no haya datos repetidos o errores (redundancia). Al usar claves únicas para cada producto o cliente, nos aseguramos de que el sistema sea escalable; es decir, que la tienda pueda crecer y gestionar miles de datos sin que el sistema se vuelva caótico. Es, básicamente, el cerebro que pone orden a todo lo que pasa en PlayToPlay.

## 📁 Contenido del Repositorio
En esta carpeta encontrarás:
* 📄 **Memoria del módulo (Word/PDF):** Explicación detallada de la lógica, las entidades y las reglas de negocio.
* 🖼️ **Diagrama E/R:** El esquema gráfico que muestra cómo se conectan todos los datos.

---
*Este proyecto forma parte del grado de Sistemas Microinformáticos y Redes (SMR).*
