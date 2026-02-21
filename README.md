# Testing con Junit

Este es un ejemplo sencillo de pruebas unitarias usando Junit 5

Observa que este proyecto no tiene ninguna clase con el método `main`, no nos hace fatal. Además, tampoco tiene ningún `scanner` ni ningún `print`.

Haz un fork de este proyecto en tu repositorio de Github y contesta a las siguientes preguntas:

1. ¿Qué sentido puede tener este proyecto y para que lo podrías usar?

  Este proyecto puede servir de utilidad para observar el funcionamiento de las pruebas, requeriendo sus entradas y salidas respectivas.
   
2. Revisa las pruebas de la suma y comenta lo que te parezca de interés

  El método sumarPositivosMal da un error en las pruebas. El resulto esperado de la suma de los dos números es 4, mientras que el resultado real debe ser 5. Cuando el error de código quede corregido y el resultado esperado sea igual al resultado real, las pruebas mostrarán que todo funciona correctamnete.
   
3. Realiza un estudio de caja negra de la división e implementa las pruebas en junit: Se realizará en markdown.
   
  - Caso de Prueba 1
      valor1: 10
      valor2: 2
    esperado: 5
  - Caso de Prueba 2
      valor1: -10
      valor2: 2
      esperado: -5
  - Caso de Prueba 3
      valor1: 10
      valor2: -2
    esperado: -5
  - Caso de Prueba 4
      valor1: -10
      valor2: -2
      esperado: 5
  - Caso de Prueba 5
      valor1: 4
      valor2: 0
      esperado: Excepción
  - Caso de Prueba 6
      valor1: 0
      valor2: 2
      esperado: 0
  - Caso de Prueba 7
      valor1: 10
      valor2: 1
      esperado: 10



## Instrucciones

El alumno deberá hacer un fork de este proyecto e implementar la solución solicitada (preguntas y código).

>Se deberá utilizar este fichero, y los artefactos de código del proyecto, para resolver el ejercicio.


**Si no se puede acceder al repositorio la evaluación del ejercicio será de 0. No se evaluarán entregas modificadas/entregadas fuera del plazo establecido en la tarea**
