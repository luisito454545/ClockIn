# ClockIn
Aplicación web y plataforma para el registro y control de horario laboral de empleados (fichaje)

# Índice

1. [Introducción - ¿qué estamos haciendo?](#2-introducción---qué-estamos-haciendo)
2. [Briefing de ideas](#3-briefing-de-ideas)
3. [Arquitectura del software](#4-arquitectura-del-software)
4. [Tecnologías a utilizar](#5-tecnologías-a-utilizar)
5. [Red](#6-red)
   1. [Diagrama de la red](#61-diagrama-de-la-red)
   2. [Mapa físico](#62-mapa-físico)
   3. [Mapa lógico](#63-mapa-lógico)
6. [Web](#7-web)
   1. [Diseño](#71-diseño)
   2. [Mockup](#72-mockup)
   3. [Mapa de navegabilidad](#73-mapa-de-navegabilidad)
   4. [Base de datos](#74-base-de-datos)
7. [Servicios explicados de un modo sencillo](#8-servicios-explicados-de-un-modo-sencillo-vinculado-al-diagrama-de-la-red)
   1. [DNS](#81-dns)
   2. [DHCP](#82-dhcp)
   3. [Apache](#83-apache)
   4. [Firewall](#84-firewall)
   5. [Copias de seguridad](#85-copias-de-seguridad)
8. [Conclusiones](#9-conclusiones)
9. [Bibliografía](#10-bibliografía)
10. [Guías de usuario](#11-guías-de-usuario)

---

<details>
<summary><h2>2. Introducción - ¿qué estamos haciendo?</h2></summary>

Aplicación web y plataforma para el registro y control de horario laboral de empleados (fichaje).
</details>

<details>
<summary><h2>3. Briefing de ideas</h2></summary>
# Proyecto ClockIn - Sistema de Fichaje y Control Horario

## Idea seleccionada
**ClockIn**: Una página web y una app móvil para que los empleados puedan fichar al entrar y salir a trabajar, controlar las horas y gestionar el teletrabajo.

---

## Justificación
Guillem y yo elegimos este proyecto porque la ley obliga a todas las empresas a llevar un registro de las horas de los trabajadores, pero muchas PYMEs siguen usando hojas de papel o archivos de Excel. 

Queremos hacer una solución fácil de usar y barata. La app permite fichar en la oficina comprobando la ubicación por el GPS del móvil (para no tener que comprar máquinas de huella ni tarjetas) y también deja fichar si trabajas desde casa. Además, le metemos una lógica al servidor para pillar fichajes raros o manipulados. Nos viene perfecto porque tocamos desarrollo web, apps, bases de datos, redes y seguridad.

---

## Objetivos (Hasta dónde queremos llegar)
Queremos dejar programado un Producto Mínimo Viable (MVP) que funcione bien y tenga:

* **Login con roles:** Entradas distintas para empleados y para los administradores de la empresa.
* **Fichaje presencial con GPS:** La app lee la ubicación del móvil y solo deja fichar si estás cerca de la oficina.
* **Modo teletrabajo:** Una opción para marcar que trabajas desde casa validando la red o la IP.
* **Detección de fichajes sospechosos:** Un filtro en el servidor que avise si hay cambios de ubicación imposibles o IPs raras.
* **Panel web de gestión:** Una web donde el jefe o RRHH pueda ver quién está trabajando y descargarse los informes del mes en PDF o Excel.

---

## Público objetivo
1. **PYMEs:** Empresas pequeñas que necesitan cumplir la ley sin gastar en aparatos de fichaje.
2. **Empresas con trabajo híbrido:** Negocios donde la gente alterna días de oficina y días en casa.
3. **Gestores de personal:** Para los que tienen que revisar los fichajes y sacar los informes a final de mes.

---

## Módulos del ciclo relacionados
* **Sistemas Operativos en Red (SOR):** Para montar el servidor, configurar la base de datos y gestionar los permisos.
* **Aplicaciones Web (AW):** Para programar el panel de control en la web y conectarlo con la base de datos.
* **Redes Locales (RL):** Para controlar las direcciones IP y saber si el usuario está conectado a la red de la oficina.
* **Seguridad Informática (SI):** Para cifrar las contraseñas, asegurar las conexiones y proteger los datos de ubicación de los usuarios.

---

## Materiales necesarios

### Hardware
* Nuestros ordenadores para programar y hacer las pruebas.
* Un teléfono móvil para probar la app y el GPS en la calle.
* Un router para hacer pruebas de red local.

### Software
* Visual Studio Code para escribir el código.
* PostgreSQL o MySQL para la base de datos.
* Node.js o Python para el servidor.
* Git y GitHub para trabajar juntos y subir el proyecto.
* Render o Supabase para subir la base de datos a internet.

---

## Recursos y fuentes
* Documentación oficial de los lenguajes y herramientas que usemos.
* El Real Decreto-ley 8/2019 sobre la ley del registro horario en España.
* Guías de la AEPD sobre el uso del GPS en el trabajo.
* Tutoriales de autenticación con tokens JWT y cálculo de distancias por GPS.

</details>

<details>
<summary><h2>4. Arquitectura del software</h2></summary>

Texto de la sección...
</details>

<details>
<summary><h2>5. Tecnologías a utilizar</h2></summary>

Texto de la sección...
</details>

<details>
<summary><h2>6. Red</h2></summary>

Texto de la sección...

<details>
<summary><h3>6.1 Diagrama de la red</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>6.2 Mapa físico</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>6.3 Mapa lógico</h3></summary>

Texto de la subsección...
</details>

</details>

<details>
<summary><h2>7. Web</h2></summary>

Texto de la sección...

<details>
<summary><h3>7.1 Diseño</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>7.2 Mockup</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>7.3 Mapa de navegabilidad</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>7.4 Base de datos</h3></summary>

Texto de la subsección...
</details>

</details>

<details>
<summary><h2>8. Servicios </h2></summary>

Texto de la sección...

<details>
<summary><h3>8.1 DNS</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>8.2 DHCP</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>8.3 Apache</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>8.4 Firewall</h3></summary>

Texto de la subsección...
</details>

<details>
<summary><h3>8.5 Copias de seguridad</h3></summary>

Texto de la subsección...
</details>

</details>

<details>
<summary><h2>9. Conclusiones</h2></summary>

Texto de la sección...
</details>

<details>
<summary><h2>10. Bibliografía</h2></summary>

Texto de la sección...
</details>

<details>
<summary><h2>11. Guías de usuario</h2></summary>

Texto de la sección...
</details>
