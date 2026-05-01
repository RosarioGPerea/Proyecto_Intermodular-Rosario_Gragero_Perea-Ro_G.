# 🌐 Redes Locales - Proyecto PlayToPlay

Bienvenido al apartado de **Redes Locales** de nuestro proyecto intermodular. Aquí se encuentra toda la arquitectura técnica que permite que **PlayToPlay** funcione de manera fluida, segura y, sobre todo, sin los temidos problemas de "lag" en nuestra zona de competición.

## 📋 Sobre este módulo
En esta sección me he encargado de diseñar, configurar y testear la infraestructura de red que da soporte a la tienda. El objetivo principal era conseguir que convivan tres áreas muy distintas:
1.  **Zona de Gestión:** Donde Ro y Juan manejan facturas y datos de clientes.
2.  **Zona Técnica:** El taller de Eme para montajes y reparaciones.
3.  **Zona Premium:** El corazón del negocio, con 6 puestos de alto rendimiento para torneos de eSports.

## 🛠️ Detalles Técnicos de la Red

### Topología y Hardware
Para garantizar la máxima fiabilidad, he optado por una **topología en estrella**. Todo el tráfico se centraliza en un **Switch Cisco 2960 de 24 puertos**, conectado a un **Router Cisco 2911**. Esta combinación nos permite gestionar velocidades Gigabit, algo fundamental para que los torneos de *Rocket League* o *LoL* se jueguen con un ping bajísimo.

### Direccionamiento IP
Hemos organizado la red bajo el rango **192.168.1.0/24**. Cada equipo tiene una identidad fija para evitar conflictos y facilitar el mantenimiento:
* **Gestión y Técnico:** IPs del rango `.10` al `.12`.
* **Puestos de Torneo:** Reservados del `.20` al `.25`.
* **Impresora y WiFi:** Direcciones específicas para que siempre sean localizables por el resto de equipos.

### Servicios Destacados
* **WiFi de Cortesía:** Configurado con seguridad WPA2-PSK para que los clientes naveguen seguros mientras esperan.
* **Impresión en Red:** Servicio inalámbrico para que Ro y Juan puedan imprimir tickets desde cualquier rincón.
* **DNS Optimizado:** Uso de los servidores de Google (8.8.8.8) para una navegación rápida.

## 🚀 Simulación y Pruebas
Todo el diseño se ha puesto a prueba en **Cisco Packet Tracer**. En la documentación adjunta puedes ver las capturas de los **tests de PING**, donde hemos conseguido un **0% de pérdida de paquetes** entre los dispositivos y el router, confirmando que la red es 100% operativa.

## 📁 Contenido del Repositorio
En esta carpeta encontrarás:
* 📄 **Memoria del proyecto (Word/PDF):** Explicación detallada de cada paso y justificación técnica con esquemas de red que incluyen imágenes de la topología y el direccionamiento y capturas de pruebas del funcionamiento.
* 💻 **Archivo .pkt:** El archivo de simulación original de Cisco Packet Tracer.

---
*Este proyecto forma parte del grado de Sistemas Microinformáticos y Redes (SMR).*
