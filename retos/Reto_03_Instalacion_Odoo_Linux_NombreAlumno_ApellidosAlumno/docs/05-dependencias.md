# 05 — Dependencias (Python, wkhtmltopdf, librerías)

1. Instala Python y paquetes de compilación:
   ```bash
   sudo apt -y install python3 python3-pip python3-venv build-essential libxslt1-dev      libzip-dev libldap2-dev libsasl2-dev libjpeg-dev libpq-dev
   ```


	![Update/Upgrade](../assets/img/05-dependencias/paso01_Instalar_paquetes.png)



2. Instala **wkhtmltopdf** compatible (para reportes PDF).


	![Update/Upgrade](../assets/img/05-dependencias/paso02_Instalar_wkhtmltopdf.png)


3. Verifica versiones:
   ```bash
   python3 --version
   wkhtmltopdf --version
   ```


	![Update/Upgrade](../assets/img/05-dependencias/paso03_versiones.png)


> Resultado esperado: dependencias instaladas y comprobadas.
