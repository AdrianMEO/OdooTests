# OdooTests
<p>1. **Creación del repositorio en GitHub**</p>
  <p>En GitHub (https://github.com) , creo un repositorio llamado OdooTests.</p>
  <p>Dentro del repositorio, creo la siguiente estructura de carpetas:</p>
  <p>extra-addons/
    dummy_module/
      __init__.py
      __manifest__.py</p>
  <p>Estos archivos (__init__.py y __manifest__.py) son necesarios para que Odoo reconozca el módulo como parte de sus addons.</p>

<p>2. **Conexión con Render**</p>
  <p>Inicio sesión en Render (https://render.com) utilizando mi cuenta de GitHub.</p>
  <p>Autorizo el acceso a mis repositorios.</p>
  <p>Selecciono New > Web Service y elijo el repositorio OdooTests.</p>
  <p>Render clona automáticamente el código del repositorio para desplegar la aplicación.</p>

<p>3. **Configuración de la base de datos PostgreSQL**</p>
  <p>En Render creo un PostgreSQL gratuito en Add New > Postgres.</p>
  <p>Una vez creado, Render me proporciona las variables de conexión:</p>
  <p>HOST</p>
  <p>USER</p>
  <p>PASSWORD</p>
  <p>DB_NAME</p>
  <p>Copio estas variables y las añado en el apartado de Environment Variables del servicio principal de Odoo en Render, para que la aplicación pueda conectarse correctamente a la base de datos.</p>
<p>4. **Despliegue y comprobación**</p>
  <p>Render instala automáticamente las dependencias y ejecuta el despliegue del servicio.</p>
  <p>Una vez finalizado el proceso, se genera una URL donde puedo acceder a la instancia de Odoo.</p>
  <p>Accedo desde el navegador, inicio sesión como administrador y compruebo que la base de datos y el módulo dummy_module aparecen correctamente.</p>
