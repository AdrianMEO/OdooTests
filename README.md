# OdooTests
1. **Creación del repositorio en GitHub**
  En GitHub (https://github.com) , creo un repositorio llamado OdooTests.
  Dentro del repositorio, creo la siguiente estructura de carpetas:
  extra-addons/
    dummy_module/
      __init__.py
      __manifest__.py
  Estos archivos (__init__.py y __manifest__.py) son necesarios para que Odoo reconozca el módulo como parte de sus addons.

2. **Conexión con Render**
  Inicio sesión en Render (https://render.com) utilizando mi cuenta de GitHub.
  Autorizo el acceso a mis repositorios.
  Selecciono New > Web Service y elijo el repositorio OdooTests.
  Render clona automáticamente el código del repositorio para desplegar la aplicación.

3. **Configuración de la base de datos PostgreSQL**
  En Render creo un PostgreSQL gratuito en Add New > Postgres.
  Una vez creado, Render me proporciona las variables de conexión:
  HOST
  USER
  PASSWORD
  DB_NAME
  Copio estas variables y las añado en el apartado de Environment Variables del servicio principal de Odoo en Render, para que la aplicación pueda conectarse correctamente a la base de datos.
4. **Despliegue y comprobación**
  Render instala automáticamente las dependencias y ejecuta el despliegue del servicio.
  Una vez finalizado el proceso, se genera una URL donde puedo acceder a la instancia de Odoo.
  Accedo desde el navegador, inicio sesión como administrador y compruebo que la base de datos y el módulo dummy_module aparecen correctamente.
