# eje2

---

![image.png](image.png)

![image.png](image%201.png)

![image.png](image%202.png)

Actores:

Empleado administrativo

Alumno

Servicio del banco

Casos De Uso:

CargarCarreras

Registrarse

Iniciar Sesion

Cerrar Sesion

Incribirse

Pagar con Tarjeta

Diagrama

![image.png](image%203.png)

Nombre Del Caso de uso:

Cargar Carreras

Descripcion:

En este caso de uso se describe el evento en el que un empleado Administrativo carga las carreras al sistema

Actores:

Cargar Carreras

PreconDiciones:

Null Pointer

| Curso Normal | Acciones del Actor | Acciones del sistema |
| --- | --- | --- |
|  | 1: el empleado administrativo selecciona “cargar carrera” | 2: el sistema le muestra un formulario con los campos: nombre, duracion en anhos, costo, cantidad maxima de cuotas para el pago |
|  | 3: el el empleado administrativo, carga los datos y le da al boton de “cargar” | 4: el sistema valida los datos |
|  |  | 5: el sistema valida que el nombre sea un nombre repetido |
|  |  | 6: el sistema valida que la duracion no sea mas de 5 anhos |
|  |  | 7: el sistema, carga en el sistema la carrera |

Curso Alterno:

paso 5 alterno: el sistema valida que se ingreso un nombre de carrera repetido, lo redirige al paso2

paso 6: el sistema valida que la duracion de la carrera es mas de 5 anhos, 

PostCondiciones:

dado un empleado que tiene informacion de una nueva carrera, cargarla en el sistema

---

Nombre de cu: Registrarse

Descripcion: En este caso de uso se describe como un Alumno se registra en el sistema

Actores:

Alumno (No registrado)

PreCondiciones:

Null

| Curso Normal | Acciones del actor | Acciones del sistema |
| --- | --- | --- |
|  | 1: el Alumno no registrado, selecciona “registrado” | 2: el sistema le muestra un formulario con los datos: nombre, apellido, nombreDeUsuario y contrasenha |
|  | 3: el Alumno registrado, llena los datos | 4: el sistema valida que no haya otro usuario con el mismo nombre de usuario |
|  |  | 5: el sistema valida que haya ingresado una contrasenha de mas de 6 digitos |
|  |  | 6: el sistema registra en el sistema al Alumno |

Curso Alterno: 

paso alterno 4: ya existe un Alumno con el nombre de usuario ingresado, se informa y se lo redirige al paso 2

Paso alterno 5: el Alumno ingreso una contrasenha de menos de 6 digitos, se informa y se lo redigie al paso 2

PostCondicion:

Que un alumno no registrado, quede registrado en el sistema

---

Nombre de caso de uso: Iniciar Sesion

Descripcion: En este caso de uso se describe como un Alumno inicia sesion

Actores:

Alumno (Registrado)

PreCondicion:

nULL

| Curso normal | Acciones del actor | Acciones del sistema |
| --- | --- | --- |
|  | 1: el alumno (Registrado) selecciona “Iniciar Session” | 2: el sistema le muestra un formulario que tiene los campos: usuario, contrasenha |
|  | 3: alumno (Registrado) ingresa los datos y le da al boton de “Iniciar” | 4: el sistema valida los datos  |
|  |  | 5: el sistema le inicia una sesion al Alumno y le habilita las funciones de un Alumno en el sistema |

Curso Alterno: 

4: el sistema valida que la contrasenha o el usuario no son validos, se informa y retorna desde el paso 2

PostCondicion: 

que un alumno registrado quede con una sesion activa

---

Nombre del caso de uso: Cerrar Sesion

Descripcion: En este caso de uso se describe como un alumno cierra sesion

Actores:

Alumno

PreCondiciones:

el alumno debe tener una sesion iniciada

| Curso Normal | Acciones del Actor | Acciones del sistem |
| --- | --- | --- |
|  | 1: el alumno slecciona “Cerrar Sesion” | 2: el sistema solicita una confirmacion del cierre de sesion |
|  | 3: el alumno confirma el cierre de sesion | 4: el sistema registra el cierre de sesion y le quita las funciones de un alumno logueado |

Curso Alterno:

3: el alumno no confirma el cierre de sesion. FIN de la CU

Post Condicion: 

La sesion ha sido cerrada, las opciones son deshabilitadas y se eliminan los datos de sesion.

---

Nombre de la cu: Incribirse

Descripcion: en esta cu, se describe como un alumno se inscribe a una carrera

Actores:

Alumno

PreCondiciones:

Alumno logueado

| Curso Normal | Acciones del Actor | Acciones del sistema |
| --- | --- | --- |
|  | 1: el alumno selecciona “incribirse” | 2: el sistema le muestra una lista de carreras |
|  | 3: el alumno selecciona una carrera | 4: el sistema ejecuta la cu de “pagar con tarjeta” |
|  |  | 5: el sistema imprime un comprobante de inscripcion y otro de pago |
|  |  | 6: el sistema regstra la inscripcion del alumno |

Curso Alterno:

4: falla la CU de “pagar con tarjeta”, se cancela la inscripcion, FIN DE LA CU

PostCondiciones:

Que un alumno quede inscripto en la carrera seleccionada

---

nombre de la cu: Pagar con Tarjeta

Descripcion: en esta Cu se describe como un Alumno realiza el pago

Actores:

Alumno, Servicio de Banco

PreCondiciones:

Que se haya ejecutado anteriormente la CU de “Inscribirse”

| Curso Normal | Acciones del Actor | Acciones del sistema |
| --- | --- | --- |
|  | 2: el Alumno, ingresa la cantidad de cuotas a pagar, el nro de tarjeta y le da al boton de “confirmar” | 1: el sistema le solicita la cantidad de cuotas a pagar y el nro de tarjeta |
|  | 4: el servicio del banco acepta la conexion con el sistema y le pide el nro de tarjeta  | 3: el sistema solicita conexion con el servicio del banco |
|  | 6: el sistema valida que la tarjeta sea valida y tenga fondos | 5: el sistema, le envia el nro de tarjeta |
|  | 7: el servicio del banco le retorna el resultado | 8: el sistema recibe que la tarjeta es valida |
|  |  | 9: el sistema recibe que la tarjeta cuenta con fondos |
|  |  | 10: el sistema registra el pago y cierra conexion con el sistema del banco |
|  |  | 11: el sistema imprime 1 comprobante de inscripcion y otro de pago |

Curso Alterno: 

paso 3: fallo en la conexion con el sistema del servicio del banco

paso8 alterno: el sistema recibe la que tarjeta es invalda. Termina la CU

Paso 9 alterno: el sistema recibe que la tarjeta no tiene fondos suficientes. Termina la CU

PostCondiciones:

Se efectuo y realizo el pago a travez de la tarjeta