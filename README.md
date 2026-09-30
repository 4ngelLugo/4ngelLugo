<h1 align="center">Miguel Ángel Lugo Ceballos</h1>
<h3 align="center">Desarrollador Full Stack · React + PHP + MySQL/SQLServer</h3>

<p align="center">
  Construyo aplicaciones web completas: desde la interfaz en React hasta la API en PHP y la base de datos en MySQL,
  pensadas para resolver procesos reales de empresas.
</p> 

<p align="left">
  <a href="mailto:lugomiguel372@gmail.com">
    <img src="https://img.shields.io/badge/lugomiguel372%40gmail.com-1a1b27?style=for-the-badge&logo=gmail&logoColor=EA4335&labelColor=1a1b27" alt="Correo" />
  </a>
</p>

---

### Sobre mí

- Trabajo en **Carnes Brangus**, donde desarrollo **Utilidades Brangus**, la plataforma interna que maneja el inventario completo de la planta de procesamiento, desde el ingreso de los lotes hasta el despacho, con trazabilidad en cada paso.
- Integro hardware con la web: lectura de **básculas**, impresión silenciosa de **rótulos Zebra** con código de barras, impresión con QZ Tray y lectores de código de barras.
- Desarrollé la aplicación de **pedidos del casino** (restaurante de la empresa) y un sistema de **gestión de personal** con registro de asistencia, cálculo de horas y notificaciones push.
- Sigo aprendiendo sobre arquitectura backend, bases de datos y buenas prácticas de seguridad.

---

### Formación

- **Tecnólogo en Análisis y Desarrollo de Software**
- **Técnico en Desarrollo de Software**

---

### Tecnologías

<p align="left">
  <img src="https://skillicons.dev/icons?i=react,vite,js,html,css,tailwind,materialui,php,mysql,npm,git,github,vscode&perline=13" alt="Tecnologías" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/microsoftsqlserver/microsoftsqlserver-plain.svg" height="48" alt="SQL Server" title="SQL Server" />
</p>

---

## Proyectos profesionales

> Estos repositorios son privados por pertenecer a empresas. Con gusto muestro el trabajo en una entrevista.

### Utilidades Brangus
*React 18 · Vite · Tailwind CSS · MUI · React Router · PHP · MySQL · SQL Server*

Plataforma web interna y modular de Carnes Brangus, usada a diario en la planta de procesamiento, los distintos puntos de venta y las oficinas. Su núcleo es el **inventario completo de la planta**: cada kilo que entra se sigue a lo largo de todo el proceso, hasta que sale despachado.

**Inventario y producción de planta**
- **Ingreso de lotes y mercancía:** recepción de lotes y de mercancía, con registro de pesos, evidencias y liquidación de lotes.
- **Trazabilidad de lotes:** seguimiento de cada lote a través de todas sus etapas, del ingreso al despacho.
- **Desposte:** manejo de los distintos tipos de desposte, con registro de productos y pesos leídos directamente desde básculas conectadas e impresión de rótulos térmicos Zebra con código de barras para canastillas, sin diálogos de impresión.
- **Transformaciones:** conversión de productos en otros productos, con su efecto en el inventario.
- **Traslados:** movimientos de producto entre áreas y bodegas.
- **Órdenes y pedidos:** órdenes de pedido de clientes de la planta, pedidos de las sedes y devoluciones.
- **Despacho:** programación de despachos, conductores y ayudantes, y certificados de calidad.
- **Inventario de planta:** existencias actualizadas con cada movimiento, más control e impresión de rótulos.

**Otros módulos**
- **Sedes:** inventario de las sedes, entradas y salidas, descuentos y reportes.
- **Mantenimiento:** activos y hojas de vida de equipos, planes preventivos, cronograma, solicitudes y órdenes de trabajo, técnicos, repuestos e indicadores.
- **Administración:** usuarios con roles y permisos por sede y área, inventario de insumos con auditoría, gestión humana, anuncios, chat y notificaciones en tiempo real con Pusher.
- **Integraciones:** consumo de SQL Server y del ERP de la empresa, replicadores de productos, precios y terceros, y reportes y documentos generados en PDF y Excel (pdfmake, jsPDF, ExcelJS, Recharts).

Backend en servicios PHP independientes por acción, con respuestas JSON uniformes, validación de datos y reglas de negocio en el servidor, y migraciones SQL versionadas.


### Chat corporativo
*React · PHP orientado a objetos · Pusher*

Chat interno de la empresa, integrado en Utilidades Brangus, con mensajería en tiempo real entre trabajadores.

- Conversaciones individuales y **grupos** con administradores, contador de mensajes no leídos y marcas de lectura.
- Envío, edición y eliminación de mensajes, validando que cada usuario solo pueda modificar los suyos.
- Envío y descarga de **archivos** mediante URL firmadas con HMAC-SHA256.
- Tiempo real con **Pusher**, encapsulado detrás de una interfaz para poder cambiarlo por WebSockets propios en el futuro.
- Backend con una arquitectura **orientada a objetos** con servicios separados, autenticación por token Bearer, secretos en `.env` y respuestas JSON estandarizadas.


### Casino Brangus: pedidos del restaurante
*React 19 · Vite 7 · Tailwind CSS 4 · pdfmake · PHP · MySQL*

Aplicación tipo kiosco para que los trabajadores pidan en el restaurante de la empresa, pensada para pantallas táctiles.

- El trabajador elige el menú (**desayuno** o **almuerzo**) y se identifica con su documento.
- Arma su pedido desde el menú del día, eligiendo cantidades, y ve el total en tiempo real.
- Al confirmar, el pedido se guarda en la base de datos y se genera un **ticket en PDF** con consecutivo, fecha, detalle y documento enmascarado.
- La sesión se cierra automáticamente al terminar, lista para el siguiente trabajador.


### Gestión de Personal
*React · PHP · MySQL*

Plataforma de gestión de trabajadores en varias sedes con arquitectura por roles (administrador, gestión humana, supervisor de campo):

- Registro de asistencia por jornada y **cálculo automático de horas** trabajadas, con consolidación por periodos.
- Gestión de personal y documentos, horarios por sede y asignación de supervisores.
- Flujo de **novedades** con aprobación y rechazo.
- **Notificaciones** en la app y push en el navegador (Web Push API).
- Carga masiva de planillas desde Excel.

---

## Proyectos públicos

| Proyecto | Descripción | Stack |
|---|---|---|
| [SGI-ProyectoFormativo](https://github.com/4ngelLugo/SGI-ProyectoFormativo) | Sistema de gestión desarrollado como proyecto formativo | JavaScript |
| [historias_clinicas-optica](https://github.com/4ngelLugo/historias_clinicas-optica) | Gestión de historias clínicas para una óptica | PHP |
| [documentos-php-react](https://github.com/4ngelLugo/documentos-php-react) | Gestión de documentos con frontend en React y backend en PHP | React · PHP |
| [fetchCatAPI](https://github.com/4ngelLugo/fetchCatAPI) | Prueba técnica de React: imagen y dato curioso de gatos desde dos APIs | React |
| [Tic-tac-toe-ReactJs](https://github.com/4ngelLugo/Tic-tac-toe-ReactJs) | Juego de tres en raya | React |
| [animatedForm](https://github.com/4ngelLugo/animatedForm) | Formulario animado de inicio de sesión y registro en una misma página | HTML · CSS · JS |

---

### Estadísticas

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=4ngelLugo&layout=compact&theme=tokyonight&hide_border=true&locale=es" alt="Lenguajes más usados" />
</p>
