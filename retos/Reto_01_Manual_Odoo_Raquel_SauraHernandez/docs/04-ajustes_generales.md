# 04 — Ajustes generales


En este archivo se detallan los ajustes generales de Odoo, incluyendo la gestión de usuarios, notificaciones y diseño.

## Pasos

#### 1. **Activar notificaciones.**
 
 **Notificaciones.**

 - Es una buena práctica activar las notificaciones al principio, ya que no configurarlas puede llevar a recibir notificaciones irrelevantes y a ignorar a posteriori las importantes.

 - Se recomienda activar las notificaciones a través del bot de Odoo y permitir que los avisos se realicen mediante el chat interno.

 - Si se habilita esta opción, los avisos aparecerán en la pestaña de la aplicación, de forma similar a una red social.


![[parte04_NotificacionesBotOdoo.png]]



#### 2. **Perfil.**

**Modo oscuro.**

- Puede activarse desde el perfil. 

- Esta opción se considera "obligatoria" para trabajar durante mucho tiempo mirando la pantalla, ya que es más "amable con la vista", pero la decisión queda completamente a gusto personal.


![[parte04_OpcionPreferencias.png]]



![[parte04_Preferencias.png]]



**Datos.**

- Es una buena práctica actualizar el perfil. 

- Los datos introducidos son visibles para todos los empleados de la base de datos de Odoo. Se deben cumplimentar datos como el nombre, el puesto de trabajo, el móvil, el teléfono de trabajo y el rol (ej. gerente o si tiene un mentor). 

- En algunas empresas, cumplimentar todos los campos es obligatorio.

![[parte04_OpcionPreferencias.png]]



![[parte04_AjustesPreferencias.png]]



**2FA (Autenticación en dos pasos).**

- La activación de 2FA es recomendada al 100%. 


![[parte04_2FA.png]]


- Se activa confirmando la contraseña y escaneando un código QR para vincularlo con una aplicación de autenticación (como Google Authenticator). 


![[parte04_2FAContraseña.png]]



![[parte04_2FAQR.png]]


- Desde esta sección, también es posible cerrar la sesión en todos los dispositivos si se detecta actividad extraña, o deshabilitar el 2FA, esto último no es nada recomendado.


![[parte04_CerrarSesion_Dsp.png]]



**Firma email.**

- Es posible editar directamente el pie de firma del correo electrónico desde el perfil.


![[parte04_FirmaEmail.png]]



**Notificaciones en Odoo.**

- El usuario puede elegir cómo ser notificado

- La opción por defecto es a través de correo electrónico, pero puede ser un poco molesta y saturar la bandeja, llevando al usuario a ignorar los avisos.

- Se recomienda cliquear la opción de gestionar en Odoo para recibir las notificaciones a través de su panel, lo cual se considera más práctico.


![[parte04_Notificaciones.png]]



#### 3. **Usuarios y compañías.**

En Enterprise se paga por usuario.

La gestión de usuarios y compañías se realiza desde el panel de ajustes.


![[parte04_Ajustes.png]]



**Compañías.**

- Es posible crear diferentes compañías y bases de datos, esta es una característica principal del plan de Enterprise. 

- Los módulos o aplicaciones (ej. CRM, Contabilidad) pueden asociarse a cada compañía. 


![[parte04_Compañias.png]]



![[parte04_NuevaEmpresa.png]]



![[parte04_DatosNuevaEmpresa.png]]


- Es importante actualizar los datos de la empresa (logo, dirección, CIF/NIF) porque son cruciales para el módulo de facturación.


![[parte04_EmpresasActuales.png]]



![[parte04_DatosEmpresa.png]]



**Usuarios y Roles por Módulo.** 

- Se pueden añadir nuevos usuarios y configurar los permisos o roles que tendrán.

- Los permisos se gestionan en función de los módulos instalados (Ventas, Servicios, Productividad, etc.). Por ejemplo, en el módulo de Ventas, un usuario puede configurarse para ver solo sus documentos, todos los documentos de la empresa, o tener un rol de administrador. Los permisos pueden darse, modificarse o quitarse.

- Al crear un usuario, este recibe un correo electrónico para establecer su contraseña.


![[parte04_Usuarios.png]]



![[parte04_NuevoUsuario.png]]



![[parte04_DatosNuevoUsuario.png]]



**Costes de Usuarios.** 

- Los planes de pago (Enterprise) se tarifan por usuario. En contraste, la versión Community permite tener usuarios ilimitados.



#### 4. **Idiomas y diseño de documentos.**

**Idiomas.** 

- Desde la sección de ajustes generales, se pueden añadir diferentes idiomas.
 
 ![[parte04_Idiomas.png]]



![[parte04_BuscarIdiomas.png]]



![[parte04_InstalarIdioma.png]]


- Una vez agregado, el usuario puede cambiar el idioma en la configuración de su perfil.


![[parte04_IdiomaPerfil.png]]



**Diseño de Documentos (Facturación).** 

- En la sección "Diseño del documento" (dentro de ajustes generales) se puede modificar cómo lucen las facturas.


![[parte04_ConfiguracionDocumento.png]]


- Se puede cambiar la plantilla de la factura.

- Odoo puede cambiar los colores de la factura automáticamente, reconociendo los colores del logo de la empresa. También se puede modificar el lema y el pie de firma del documento.



![[parte04_DiseñoDocumento.png]]



#### 5. **Emails de resumen: periodicidad y destinatarios.**

Esta configuración se refiere a los informes que resumen la actividad dentro de la aplicación.

**Contenido y Periodicidad.** 

- Por defecto, la periodicidad es diaria e incluye información como leads entrantes, correos generados, tareas abiertas y facturación.


![[parte04_ConfiguracionResumenes.png]]



![[parte04_ResumenesActuales.png]]



**Personalización.** 

- El usuario puede seleccionar específicamente qué información desea recibir (ej. solo oportunidades ganadas). 

- La periodicidad también es modificable, pudiendo seleccionar un resumen mensual.


![[parte04_DetallesResumen.png]]



**Destinatarios.** 

- Se puede configurar para que el correo de resumen sea enviado a otras personas o departamentos además del propio usuario. 

- Es posible crear múltiples informes personalizados para diferentes destinatarios.


![[parte04_DestinatariosResumen.png]]






