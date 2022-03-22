# Postgresql-playbooks
Playbooks de ansible para instalar un servidor de base de datos en máquinas Centos7.

El playbook "1" realiza las tareas iniciales necesarias para poder crear el servidor de base de datos.

El playbook "2" chequea que se haya instalado postgresql y lo inicia.

El playbook "3" crea la base de datos y el usuario.

El playbook "4" sirve para insertar valores en la base de datos.

Deberás crear los archivos ".sql" en el directorio "/tmp". Para insertar los datos de dichos archivos a la base de datos, tendrás que modificar el playbook "4" poniendo el nombre que le hayas asignado al archivo ".sql" donde pone "nombrearchivo.sql".

En el archivo "prueba.sql" hay datos de prueba para insertar en la base de datos.

El usuario que se crea es "root" con contraseña "toor", para la base de datos con nombre "database1", si quieres cambiar estos valores deberás modificar el archivo "vars.yml" antes de ejecutar los playbooks.

El archivo "hosts" tendrás que modificarlo poniendo la ip de los hosts que quieres aprovisionar.
