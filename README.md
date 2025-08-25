🏨 Sistema de Reservas Hostal HDQ
Este proyecto es un sistema de reservas completo para un hotel o hostal, desarrollado con HTML, CSS y JavaScript. La aplicación permite a los usuarios realizar reservas, ver la disponibilidad de habitaciones y consultar estadísticas, mientras que los datos se almacenan de forma remota y segura en una Hoja de Cálculo de Google.

🚀 Funcionalidades Principales
Pestaña "Nueva Reserva": Un formulario interactivo para que los clientes ingresen sus datos, seleccionen fechas y el número de huéspedes. El sistema calcula automáticamente las habitaciones disponibles y el costo total.

Pestaña "Habitaciones": Muestra una lista detallada de todas las habitaciones del hostal con información como el número, tipo, capacidad y precio por noche.

Pestaña "Estadísticas": Proporciona un panel de control con métricas clave como el total de reservas, habitaciones disponibles y la ocupación promedio, lo que facilita la gestión del negocio.

🛠️ Tecnología Utilizada
Front-end:

HTML5: Para la estructura y el contenido de la página.

CSS3: Para el diseño, la presentación visual y la responsividad.

JavaScript: Para la lógica de la aplicación, la interacción del usuario, las validaciones y el cálculo de precios.

Back-end:

Google Apps Script: Actúa como un intermediario o API. Recibe los datos enviados desde el formulario y los inserta como una nueva fila en una Hoja de Cálculo de Google.

Google Sheets: La base de datos donde se almacenan todas las reservas de manera organizada.

📝 Configuración y Uso
Para poner en funcionamiento este sistema, sigue estos sencillos pasos:

Configurar Google Sheets:

Crea una nueva hoja de cálculo en Google.

Nombra la hoja de trabajo principal como "Reservas".

Asegúrate de que la primera fila (encabezado) contenga las siguientes columnas en el orden exacto: Fecha de Reserva, ID Reserva, Nombre, Email, Teléfono, Huéspedes, Check-in, Check-out, ID Habitación, Tipo Habitación, Precio por Noche, Noches, Total, Comentarios.

Crear el Google Apps Script:

En tu Hoja de Cálculo, ve a Extensiones > Apps Script.

Copia y pega el código proporcionado en la respuesta anterior en el editor de Apps Script.

Reemplaza 'Your_Spreadsheet_ID_Here' en el código con el ID de tu Hoja de Cálculo (la cadena de caracteres que se encuentra en la URL).

Guarda el script.

Implementar la Aplicación Web:

En el editor de Apps Script, haz clic en Implementar > Nueva implementación.

Selecciona Aplicación web y configura el acceso a "Cualquier persona".

Haz clic en Implementar y luego Autorizar acceso.

Copia la URL de la aplicación web que se genera.

Conectar el Front-end:

Abre el archivo HTML y busca la variable GOOGLE_SCRIPT_URL.

Reemplaza la URL actual con la URL de la aplicación web que acabas de copiar.

Guarda el archivo HTML.

¡Listo! Abre el archivo HTML en tu navegador y el sistema estará operativo. Cada reserva que confirmes se registrará automáticamente en tu Hoja de Cálculo de Google.
