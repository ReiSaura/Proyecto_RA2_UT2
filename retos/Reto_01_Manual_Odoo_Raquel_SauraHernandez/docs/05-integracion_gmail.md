![Banner](../assets/img/portada/Banner.png)


# 05 — Integración con Gmail (OAuth GCP + Add-on)


## Requisitos

- Cuenta Google Cloud (GCP).

## Pasos resumidos

1. **Activar plugin de correo en Odoo e instalar *Odoo Inbox Add-on* en Gmail.**

	-  Para activar el plugin de correo se debe ir a "Opciones generales" dentro de ajustes y, en la sección de integraciones, activar la opción Plugin de correo. 
	
	- Es fundamental guardar la configuración tras activarla.
	
	- Para instalar Odoo Inbox Add-on en la bandeja de entrada de Gmail, se debe hacer clic en el botón de más (+) para buscar la aplicación.
	
	
	![Plugin de Correo](../assets/img/05-integracion_gmail/parte05_PluginCorreo.png)
	



	- Tras instalar y conceder los permisos que necesita para acceder, hay que loguearse en el _add-on_ de Gmail introduciendo la URL de su base de datos de Odoo. 
	
	- Una conexión exitosa mostrará un mensaje de "success".
	
	![Búsqueda de Plugin](../assets/img/05-integracion_gmail/parte05_BusquedaPlugin.png)



2. **Google Cloud Console.** 

	**Acceso a OAuth en Odoo.** 
	
	- Para activar el acceso a OAuth se debe ir a "Opciones generales" dentro de ajustes y, en la sección de integraciones, se debe acceder a Autenticación OAuth y luego a proveedores OAuth.
	
	
	![Autenticación OAuth](../assets/img/05-integracion_gmail/parte05_AutenticacionOAuth.png)


	
	![Ajustes de Proveedores](../assets/img/05-integracion_gmail/parte05_AjustesProveedores.png)


	
	![Datos](../assets/img/05-integracion_gmail/parte05_DatosProveedor.png)



	**Creación del Proyecto en GCP.** 
	
	- En la Consola de Google Cloud, el usuario debe crear un nuevo proyecto (por ejemplo, "ODU test").
	
	
	![Nuevo ProyectoGCC](../assets/img/05-integracion_gmail/parte05_NuevoProyectoGCC.png)



	**Habilitación de API.** 
	
	- Dentro del proyecto, se busca y se habilita la Gmail API.
	
	
	![GMAIL API](../assets/img/05-integracion_gmail/parte05_GmailAPI.png)


	
	![Instalar API](../assets/img/05-integracion_gmail/parte05_InstalarAPI.png)



	**Creación de Credenciales.** 
	
	- Se debe seleccionar Crear credenciales y después datos del usuario.
	
	
	![Crear Credenciales](../assets/img/05-integracion_gmail/parte05_CrearCredenciales.png)



	- Se deben establecer los permisos que Odoo necesitará, como leer, redactar y enviar correos.
	
	
	![Permisos](../assets/img/05-integracion_gmail/parte05_Permisos.png)
	
	
	- El tipo de aplicación debe seleccionarse como **Aplicación web**.
	
	- Se debe agregar la URL de redireccionamiento autorizada (**Redirect URI**). Esta URL debe tener el formato `https://[vuestro nombre].com/google-gmail/confirm`.
	
	 - Al finalizar, se hace clic en "crear" para obtener las credenciales.
	
	
	
	![Tipo de App](../assets/img/05-integracion_gmail/parte05_TipoApp.png)


	
	![URL](../assets/img/05-integracion_gmail/parte05_URL.png)



3. **Copiar Client ID/Secret y Guardar**.

	**Obtención de Credenciales.** 
	
	- En la Consola de Google Cloud (Credenciales), se debe copiar el ID del cliente y el Secreto del cliente.
	
	
	**Configuración del Servidor en Odoo.** 
	 
	- De vuelta en Odoo, el usuario debe habilitar la opción utilizar servicios de correo electrónico personalizados.
	
	- Se activará una nueva opción: usar un servidor de GM, donde se pegarán el ID del cliente y el Secreto del cliente.
	
	
	![Credenciales Odoo](../assets/img/05-integracion_gmail/parte05_CredencialesOdoo.png)
	
	
	- **No** se debe olvidar guardar los cambios después de pegar las credenciales.



4. **Probar desde Gmail.** 

	 **Identificación Automática.**
	
	- Una vez vinculado, el complemento de Odoo en Gmail identifica la empresa y el remitente del correo.
	
	
	![Contactos](../assets/img/05-integracion_gmail/parte05_Contactos.png)
	
	
	![Lista de Contactos](../assets/img/05-integracion_gmail/parte05_ListaContactos.png)
	
	
	![Información de la Empresa](../assets/img/05-integracion_gmail/parte05_InformacionEmpresa.png)
	




![Banner](../assets/img/portada/Banner.png)
