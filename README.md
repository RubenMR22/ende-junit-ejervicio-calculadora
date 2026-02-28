# Testing con Junit

Este es un ejemplo sencillo de pruebas unitarias usando Junit 5

Observa que este proyecto no tiene ninguna clase con el método `main`, no nos hace fatal. Además, tampoco tiene ningún `scanner` ni ningún `print`.

Haz un fork de este proyecto en tu repositorio de Github y contesta a las siguientes preguntas:

1. ¿Qué sentido puede tener este proyecto y para que lo podrías usar?

  Este proyecto representa un módulo de lógica de negocio que está validado mediante pruebas unitarias automáticas. Su finalidad es garantizar que el código funciona correctamente y mantener la calidad del producto dentro de la empresa.
  Garantiza robustez ya que controla correctamente las posibles entradas inválidas y valida mediantes sus pruebas automáticas cubriendo diferentes escenarios (valores positivos, negativos o inválidos).
   
2. Revisa las pruebas de la suma y comenta lo que te parezca de interés

  El proyecto sigue la estructura que se muestra a continuación:
  
    - Código productivo: src/main/java/es/etg/dax/testing/Calculadora.java

    - Caso de excepción: src/main/java/es/etg/dax/testing/exception/OperacionNoValidaException.java

    - Tests: src/test/java/es/etg/dax/testing/CalculadoraTest.java

  El método sumarPositivosMal da un error en las pruebas. El resultado esperado de la suma de los dos números es 4, mientras que el resultado real debe ser 5. Cuando el error de código quede corregido y el resultado esperado sea igual al resultado real, las pruebas mostrarán que todo funciona correctamente.
  Este fallo es interesante porque permite demostrar que las pruebas unitarias funcionan de manera correcta, cumpliendo su función de control de calidad al detectar que el comportamiento de uno de los métodos no coincide con el resultado que se espera.
   
3. Realiza un estudio de caja negra de la división e implementa las pruebas en junit: Se realizará en markdown.

   La función que se analizará en este estudio será la siguiente:
     - Método: dividir(int a, int b).
     - Salida: int.
     - Posible resultado que puede aparecer: OperacionNoValidaException si b == 0.

    Dominio de entrada:
      - a: cualquier número entero (positivo, negativo o cero)
      - b: cualquier número entero distinto de cero, ya que si es cero se debería lanzar una excepción.


   El proyecto debe cubrir las siguientes entradas posibles:
      - Caso 1: Positivo / positivo.
      - Caso 2: Negativo / positivo.
      - Caso 3: Positivo / negativo.
      - Caso 4: Negativo / negativo.
      - Caso 5: División por cero.
      - Caso 6: Dividendo cero.
      - Caso 7: División por uno.


   Tabla de casos de pruebas:
  - Caso de Prueba 1
      - valor1: 10
      - valor2: 2
      - esperado: 5
  - Caso de Prueba 2
      - valor1: -10
      - valor2: 2
      - esperado: -5
  - Caso de Prueba 3
      - valor1: 10
      - valor2: -2
      - esperado: -5
  - Caso de Prueba 4
      - valor1: -10
      - valor2: -2
      - esperado: 5
  - Caso de Prueba 5
      - valor1: 4
      - valor2: 0
      - esperado: Excepción
  - Caso de Prueba 6
      - valor1: 0
      - valor2: 2
      - esperado: 0
  - Caso de Prueba 7
      - valor1: 10
      - valor2: 1
      - esperado: 10



## Instrucciones

El alumno deberá hacer un fork de este proyecto e implementar la solución solicitada (preguntas y código).

>Se deberá utilizar este fichero, y los artefactos de código del proyecto, para resolver el ejercicio.


**Si no se puede acceder al repositorio la evaluación del ejercicio será de 0. No se evaluarán entregas modificadas/entregadas fuera del plazo establecido en la tarea**
