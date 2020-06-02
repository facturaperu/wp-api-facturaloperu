# FacturaloPeru | Wordpress | Woocommerce | Plugin Facturación

_Plugin que conecta realiza envios desde los pedidos de woocomerce hacia la API del Facturador PRO de FacturaloPeru_

## Comenzando 🚀

_Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._


### Pre-requisitos 📋

_Tener una instalación limpia de Wordpress superior a la version 5.0.1 con Woocommerce instalado_


### Instalación 🔧

_Desde el panel de administración de Wordpress, ir a Plugins > Añadir nuevo_

_Pulsar sobre el boton superior "Subir plugin"_

_En la siguiente pantalla aparecerá un boton para seleccionar archivo, cargar el plugin, se le solicitará el usuario y clave de Wordpress, una vez ingresado y el proceso exitoso dirigirse al listado de plugins para activarlo_


>Si se le ha enviado una actualización deberá reemplazar el plugin existente


## Funcionalidad ⚙️

* En el panel de administración de Wordpress dentro del menú de Woocommerce se habilita un submenu "FacturaloPeru API", al entrar se muestran dos campos para el API Token y la URL que se asignan en su Facturador PRO, para información de como obtener los datos, lea el [manual del Facturador](https://docs.google.com/document/d/1su5bLA1IpM0aOjzO6L3XWV96ac2eo1zJAI7zBMpVIyc/edit?usp=sharing).
* En la tienda online cuando realizé un pedido, al confirmarlo podrá ingresar el RUC o DNI, si lo hace de primero el resto de los campos se autocompletará con información de la Sunat.
* En el formulario de confirmación se mostrará la opción de tipo de comprobante (FACTURA o BOLETA), esto define el tipo de documento que será generado por la API.
* En el panel de Woocommerce, entrando a cada detalle de pedido observará dos nuevas cajas que tienen por titulo "Factura Enviada" y "Json Generado"
    * Dentro de la caja de Factura Enviada se mostrará un boton una vez el pedido se encuentre en completado, al pulsar sobre el botón se enviará un documento a la API para generar el comprobante seleccionado en la Sunat, obtendra de vuelta 3 enlaces y un boton "salvar respuesta" para almacenarlos, de manera que pueda tener a la mano su contenido (PDF,XML,CDR)
    * Si ocurre un error o desea probar el documento que se genera para enviar a la API, puede dirigirse a la cada de Json Generado, que le muestra el contenido, puede hacer pruebas con herramientas como Postman.
* Puede complementar la funcionalidad de la tiendad virtual observando el siguiente [documento](https://docs.google.com/document/d/1JqHw1VQKMDwWZvVcvfPEnmL0sWw7DjHyny2PYaXUYdQ/edit?usp=sharing).

## Autor

**FacturaloPeru** [facturaloperu.com](http://facturaloperu.com)