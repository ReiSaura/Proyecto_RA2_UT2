# 07 — Calendario y Citas


## Pasos

- Calendario (día/semana/mes) + disponibilidad del equipo.
- **Integración con Google Calendar** (API OAuth GCP).
- **Odoo Meet** (videollamadas) o enlaces externos.
- **Módulo Citas** (Enterprise): enlaces públicos, buffers, preguntas previas.


1. **Calendario (día/semana/mes) + disponibilidad del equipo**

	El módulo de Calendario se utiliza para conectar y mantener toda la agenda y actividades dentro de Odoo.
	
	
	![[parte07_Calendario.png]]
	
	
	**Vistas.**
	
	- El calendario se puede filtrar y ordenar por vista semanal, vista mensual o vista anual.
	
	
	**Disponibilidad del equipo.** 
	
	- Si hay varios usuarios en la cuenta de Odoo, el calendario permite ver las agendas de los compañeros. 
	
	- Esto es útil para agendar una reunión en grupo y verificar la disponibilidad de las personas antes de convocarlas.
	
	
	![[parte07_Vistas.png]]
	
	
	**Creación de eventos.** 
	
	- Los eventos se crean al clicar en el calendario y se pueden definir la fecha y hora de inicio y fin, además de adjuntar recordatorios, notas y archivos.
	
	
	![[parte07_CreacionEvento.png]]



2. **Integración con Google Calendar (API OAuth GCP)**

	Es posible vincular el calendario de Odoo con el calendario de Google. Este proceso requiere una configuración mediante la API de Google Cloud Platform (GCP), similar a la vinculación de Gmail.
	
	**Habilitación de API en GCP.** 
	
	- Se debe crear un nuevo proyecto en la Consola de Google Cloud (ej. "ODU Calendar") y habilitar la Google Calendar API.
	
	
	![[parte07_CreacionProyectoGCC.png]]


	
	![[Parte07_CalendarAPI.png]]


	
	
	![[parte07_HabilitarAPI.png]]



	**Credenciales.** 
	
	- Se deben crear credenciales como aplicación web. Al crear los permisos, se recomienda marcar todas las opciones de calendario para estar cubierto.
	
	
	![[parte07_Credenciales.png]]


	
	![[parte07_API_DatosUsuario.png]]
	
	
	**URL de Redireccionamiento.** 
	
	- Es fundamental establecer una URL de redireccionamiento autorizada con el siguiente formato: `https://[vuestro nombre].com/google-account/authentication`.
	
	
	
	![[parte07_Informacion.png]]


	
	![[parte07_Permisos.png]]


	
	![[parte07_TodosPermisos.png]]



	**Vinculación en Odoo.** 
	
	- Una vez obtenido el *ID del cliente y el Secreto del cliente de GCP, estos se copian y se pegan en Odoo en Ajustes > Ajustes de calendario > Google Calendar.
	
	
	![[parte07_Vinculacion.png]]



3. **Odoo Meet (videollamadas) o enlaces externos**

	Al crear un evento en el calendario, Odoo facilita la integración de videollamadas:
	
	**Enlaces externos.** 
	
	- En la sección "URL de llamada", se puede pegar la URL de cualquier plataforma externa, como Zoom o Google Meet.
	
	**Odoo Meet.** 
	
	- Odoo ofrece su propia opción de reunión llamada "Reunión de ODU", lo que permite integrar la videollamada directamente dentro de la aplicación sin usar otra plataforma.
	
	
	![[parte07_NuevaLlamada.png]]


	
	![[retos/Reto_01_Manual_Odoo_Raquel_SauraHernandez/assets/img/07-calendario_y_citas/parte07_Enlace.png]]


	
	![[parte07_InicioLLamada.png]]
	
	
	**Funcionalidad.** 
	
	- Odoo Meet es funcional, similar a plataformas como Discord, y permite funciones como unirse a la llamada, añadir participantes, establecer el fondo o añadir mensajes. También se pueden adjuntar recordatorios, notas y aspectos previos/posteriores a la llamada.



4. **Módulo Citas (Enterprise):** enlaces públicos, buffers, preguntas previas

	El módulo de Citas debe instalarse por separado y es una opción exclusiva para los planes de pago (Enterprise). Es ideal para servicios de consultoría o servicios médicos.
	
	
	![[parte07_Citas.png]]


	**Tipos de Citas.**
	
	- Permite configurar diferentes tipos de citas (personales, videollamadas, consultas pagadas, reservas de recursos o mesas de restaurantes).
	
	
	![[parte07_TiposDeCitas.png]]


	**Duración y Planificación.** 
	
	- Se define la duración de las citas, la ventana de planificación (intervalo de fechas) y el horario específico (ej. lunes de 9 a 12).
	
	
	![[parte07_CitaCreada.png]]
	
	
	**Buffers (Tiempo Mínimo).** 
	
	- Se puede configurar el tiempo mínimo que debe transcurrir antes de que alguien pueda reservar una cita, siendo el valor por defecto de una hora de antelación.
	
	
	 **Preguntas Previas.**
	
	- Permite personalizar el proceso añadiendo preguntas para conocer el motivo de la consulta antes de que la cita se agende.
	
	 
	 **Enlaces Públicos.** 
	 
	 - Odoo genera un enlace que se puede copiar y compartir públicamente. Los clientes acceden, eligen un hueco, introducen sus datos y confirman la cita.
	
	
	![[parte07_CompartirCita.png]]


	
	![[parte07_Enlace.png]]


	
	![[parte07_EstablecerCita.png]]
	
	
	**Integración.** 
	
	- Una vez agendada por el cliente, la cita aparece automáticamente en el Calendario de Odoo del usuario correspondiente

	
	![[parte07_CitaEnCalendario.png]]