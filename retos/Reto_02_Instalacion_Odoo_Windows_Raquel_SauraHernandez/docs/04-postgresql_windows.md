# 04 — PostgreSQL en Windows

> Odoo requiere **PostgreSQL**. Según instalador y versión, se incluye o puede requerir instalación separada.

1. Verifica si el instalador de Odoo **instala PostgreSQL** automáticamente.

	
	![OdooServer y PostgreSQL](../assets/img/04-postgresql_windows/parte04_OdooServer+PostgreSQL.png)
	


2. Si no, descarga **PostgreSQL para Windows** e instálalo:
   - Selecciona versión soportada por tu Odoo.
   - Define usuario `postgres` y contraseña **segura** (anótala).


	![Página de PostgreSQL](../assets/img/04-postgresql_windows/parte04_Pagina_PostgresSQL.png)


	
	![Instalador PostgreSQL en Windows](../assets/img/04-postgresql_windows/parte04_WindowsPostgreSQL.png)


	
	![Versión de PostgresSQL](../assets/img/04-postgresql_windows/parte04_InstalarPostgreSQL.png)


2. Comprueba que el **servicio de PostgreSQL** está en ejecución.

	![Servicio de PostgreSQL](../assets/img/04-postgresql_windows/parte04_PostgreSQL-Servicio.png)


> Resultado esperado: PostgreSQL instalado y funcionando (usuario/puerto guardados).
