# Practica 3 solucion


## Caso de estudio (reglas de negocio):

<p>El hospital está formado por un conjunto de consultorios. Cada consultorio cuenta con una clave formada
por 1 carácter y 2 dígitos. A cada consultorio se le asocia una especialidad, por ejemplo, en el consultorio
A22 se atiende la especialidad de cardiología. Algunos consultorios son únicamente para consultas
generales por lo que no cuentan con especialidad asignada. Para cada especialidad se guarda su nombre
y el número mínimo de años de experiencia que debe tener un médico para poder ejercerla dentro del
hospital.</p>

* Médicos del hospital.
<p>El hospital cuenta con una plantilla de médicos. Se registran los siguientes datos: nombre, apellidos,
número de cédula profesional, email (opcional) y su(s) especialidad(es) si es que cuenta con alguna.
Algunos médicos son supervisores de área que tienen a su cargo de 3 hasta 10 médicos. Se requiere saber
qué médicos están asignados a cada supervisor. Se registra también el tiempo en años de experiencia
que tiene el médico en cada una de sus especialidades.</p>

* Registro de citas.
<p>Para atender a los pacientes, se requiere registrar una cita la cual puede realizarse por teléfono. El
empleado encargado de atender las llamadas telefónicas debe registrar los siguientes datos: fecha y hora
de la cita, nombre y apellidos del paciente, fecha de nacimiento, número de seguro social (SSN), edad, y el
consultorio al que tendrá que acudir para su cita. En caso de que el paciente ya este registrado con
anterioridad, solo se registran los datos de su nueva cita. Para cada cita que solicite un paciente se genera
un número de cita que inicia en 1. Es decir, todos los pacientes inician con la cita 1, después la cita 2, y así
sucesivamente.</p>

* Registro de consultas
<p>Cada Cita genera una consulta. Si el paciente no acude a su cita, no se genera. Cuando el paciente entra a
consulta, se realiza un conteo del tiempo que dura su consulta, se almacena este valor en minutos, el
médico que lo atendió y la cita asociada. Cada paciente cuenta con un expediente (archivo .doc) el cual
se actualiza en cada consulta. Se requiere que este documento se almacene en la base de datos. Como
parte de los datos de la consulta, se registra el peso y la presión arterial del paciente.</p>


# * Propuesta de entidades
* Registro de recetas médicas

<p> Cada consulta genera una receta médica. Se requiere llevar un control detallado de los medicamentos que
se le recetan al paciente. Para cada consulta del paciente se requiere registrar los datos de su receta
médica: Fecha de elaboración, folio de 8 caracteres.
Se cuenta con un catálogo de medicamentos que un médico puede emplear para incluir en la receta de
un paciente. Para cada medicamento se registra una clave de 8 caracteres, descripción y sustancia activa.
Cabe mencionar que cada medicamento puede tener varios nombres que dependen de la marca que los
fabrican. Se requiere almacenar la lista de los nombres conocidos de cada medicamento.
Se requiere registrar la lista de medicamentos asignada a cada receta. Una receta puede incluir uno o y
hasta 5 medicamentos. Para cada medicamento que se incluye en una receta, se registra la dosis en
miligramos, la frecuencia en horas y el número de días de tratamiento. Debido a que cada medicamento
tiene varios nombres, el médico asigna uno de estos nombres en la receta para facilitar su compra.
Vacunas.
El hospital ofrece la aplicación de vacunas gratuitas a sus pacientes (máximo 10 vacunas por paciente). Se
requiere llevar el control de las vacunas que han recibido. Se cuenta con un catálogo de tipos de vacunas
en donde se almacena su clave de 3 caracteres, su nombre y un texto con recomendaciones de su forma
de aplicación y empleo. Al momento de aplicar la vacuna se registra la fecha y hora en la que le fue aplicada
al paciente y al médico que la autorizó.</p>
