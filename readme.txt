Bienvenido a la Aplicacion de Preguntas y Respuestas, esta aplicacion corre con el framwork de Flask y se desarrollo en VScode, 
para poder iniciarla es requerido que la version de python sea Python 3.9.10 o superior, 
verificar que todas las librerias se encuentren instalas (pip, pipenv, flask, flask-SQLAlchemy, flask-login).

1. Primero necesitamos intalar pipenv, nos vamos  terminal y corremos el siguiente codigo:

pip install pipenv

2. Ahora necesitamos instalar las librerias de flask, en la terminal corremos:

pipenv install flask

3. Una vez instalado el ambiente, lo inciamos:

pipenv shell

4. Ahora necesitamos instalar las librerias pra utilizar los servicios de la aplicacion:

pipenv install flask-sqlalchemy

luego:

pip install flask-login

y luego:

pipenv install python-dotenv

5. Y por ultimo, ejecutamos el siguiente comando:

flask run

Aqui podremos utilizar la direccion Running on http://127.0.0.1:5000/ en un navegador para utilizar la aplicacion.
___________________________________________________________________________________________________________________________

* Para utilizar la app, se diseñaron 3 tipos de usuarios: Adminstrador, Experto, y Regular.
* Al inicio de la aplicacon se ven las preguntas contestadas sin nececidad de loguiarse.
* para utlizar la aplicacion se pueden crear nuevos usuarios, los cuales se almacenan en la base de datos

* Para usar la aplicacion todos los usuarios tienen que registrarse, siempre que un usuario se registra, se asigna automaticamente como usuario: Regular;
y puede hacer preguntas y asignarselas a los expertos para que sean contestadas.
- Los usuarios Regulares pueden volverse usuarios Expertos, solamente con la autorizacion del usuarion Administrador.
- Credenciales de usuario Regular: usuario > nuevousuario1 , contraseña > nuevousuario1

* Solamente los usuarios Expertos pueden ver las preguntas sin contestar y responder preguntas asignadas a estos.
- cuando los usuarios Expertos contestan una pregunta, esta sale en la pagina pricipal como preguntas contestadas, las cuales siempre se muestran sin necesidad de registrarse o loguiarse.
- los usuarios expertos tambien pueden hacer preguntas y asignarla a otros expertos 
- Creenciales de usuario Experto: usuario >  andresT , contraseña > andres1    -    usuario >  camiloandres , contraseña > camiloandres1

* Unicamente el usuarion Administrador, puede convertir a un usuario regular en uno experto; loguiandose y luego en la ventana de Ajustes de usuario, seleccionar el usuario regular que quiera convertir en experto.
- el usuario Administrador tambien puede hacer preguntas y asignarsela a cualquier experto.
- Creenciales de usuario Administrador: usuario >  camiloT , contraseña > camilo1

