# Gestor de gastos 💸

![HTML](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white) ![CSS](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) ![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?logo=github&logoColor=white)

Aplicación web para organizar las finanzas personales, registrar movimientos y planificar objetivos económicos. Permite visualizar la distribución del dinero y llevar un seguimiento de los compromisos de pago desde una interfaz adaptada a dispositivos móviles.

**[Acceder al Gestor de gastos](https://laragotthelf.github.io/Gestor-de-gastos/)**

## Funcionalidades

| Herramienta | Descripción |
| --- | --- |
| Movimientos | Alta, edición y eliminación de ingresos, gastos y ahorros, con fecha, descripción y clasificación. |
| Organización | Espacios personalizables, como Trabajo y Personal, que pueden consultarse juntos o por separado. |
| Períodos | Consultas semanales, mensuales, anuales o entre fechas elegidas. |
| Monedas | Registro en ARS y USD, con conversión a pesos según el tipo de cambio ingresado manualmente. |
| Cuotas | Proyección mensual de compras, importe pendiente y seguimiento de pagos. |
| Presupuesto | Límites mensuales por pestaña e indicadores de consumo del presupuesto. |
| Ahorro | Objetivos mensuales, progreso y estimaciones de recortes por categoría. |
| Visualización | Resumen financiero, gráfico interactivo de anillo y desglose por categoría y subcategoría. |
| Apariencia | Tema claro u oscuro y secciones plegables. |

## Cómo utilizar la aplicación

1. Abrir el enlace de la aplicación desde un navegador.
2. Seleccionar una pestaña o crear una nueva desde Ajustes.
3. En **Nuevo movimiento**, elegir el tipo de operación, completar los datos y guardar.
4. Seleccionar el período y las pestañas que se desean consultar.
5. Configurar el presupuesto y la meta de ahorro según las necesidades personales.

El saldo del período se obtiene mediante la siguiente relación:

**Saldo disponible = Ingresos − Gastos − Ahorro**

Las cuotas programadas se incluyen como gastos del mes correspondiente, aunque todavía no estén marcadas como pagadas.

## Acceso desde el celular

No es necesario descargar un APK ni instalar la aplicación desde una tienda.

- **Android:** abrir el enlace en Chrome, ingresar al menú de tres puntos y seleccionar Añadir a pantalla de inicio o Instalar, según la opción disponible.
- **iOS:** abrir el enlace en Safari, acceder a Compartir y seleccionar Añadir a pantalla de inicio.

El acceso permanece vinculado a la misma dirección web. Las nuevas versiones se distribuyen mediante GitHub Pages y pueden requerir recargar la página con conexión a Internet.

## Almacenamiento y privacidad

En la versión independiente alojada en GitHub Pages, los registros y ajustes se conservan en el almacenamiento local del navegador (`localStorage`). No se requiere una cuenta para utilizarla en este modo.

Los datos no se sincronizan automáticamente entre dispositivos o navegadores. Borrar los datos del sitio puede ocasionar la pérdida de los registros. Actualmente no existe una función de exportación o recuperación de copias de seguridad.

El proyecto incluye un service worker para almacenar recursos de la aplicación y permitir su uso sin conexión después de una carga inicial satisfactoria, sujeto a la disponibilidad de la caché del navegador.

## Estructura del repositorio

```text
Gestor-de-gastos/
├── index.html      # Interfaz, estilos y lógica de la aplicación
├── manifest.json   # Configuración de la aplicación web instalable
├── sw.js           # Gestión de caché y acceso sin conexión
├── icon-192.png    # Icono de 192 × 192
├── icon-512.png    # Icono de 512 × 512
└── README.md      # Documentación del proyecto
```

## Tecnologías

HTML5, CSS3, JavaScript, SVG, Web Storage API, Service Worker API y Web App Manifest. Publicación mediante GitHub Pages, sin necesidad de un proceso de compilación para la versión independiente.

## Consideraciones

La cotización del dólar debe ingresarse manualmente. Las sugerencias de ahorro son estimaciones basadas en los movimientos y en la prioridad de cada categoría; no constituyen asesoramiento financiero.
