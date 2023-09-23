# Taller 1 Evaluación Curso de Introducción al Procesamiento en Paralelo 

Maximiliano Correa Pico - 2161594

# Introducción 

La sucesión de Fibonacci es un concepto fundamental en matemáticas que ha inspirado una variedad de aplicaciones y representaciones visuales en el mundo de la geometría y la programación. Esta sucesión, que comienza con los números 0 y 1, se caracteriza por su propiedad única en la que cada término es la suma de los dos anteriores. Esta relación de recurrencia da lugar a una secuencia infinita de números naturales: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34 y así sucesivamente.

En este taller, nos enfocaremos en un aspecto práctico de la sucesión de Fibonacci. Proponemos la creación de un programa en lenguaje C que calcule la suma de los números de Fibonacci en índices pares de hasta N términos de la sucesión. Para abordar este desafío, proporcionaremos dos soluciones: una solución secuencial y otra solución paralela utilizando OpenMP (Open Multi-Processing). Esta última permitirá aprovechar al máximo los recursos de procesamiento disponibles y acelerar el cálculo de la suma de manera eficiente.

# Implementación

1) Solución Secuencial.

![image](https://github.com/Maxito06/IntroPP2161594/assets/117324114/51d4f020-3102-413a-a535-45b4ed874482)

2) Solución Paralela con OMP.

![image](https://github.com/Maxito06/IntroPP2161594/assets/117324114/0ddec32a-3898-47c9-8c9a-ae96bf283d7b)

# Tiempo de ejecución 

1) Solución Secuencial
   
![image](https://github.com/Maxito06/IntroPP2161594/assets/117324114/394f8a6d-580c-45aa-b0fe-d0912cad3e66)

2) Solución Paralela


# Conclusiones

* Rendimiento: De acuerdo a la teoría y las pruebas se puede concluir que la solución paralela toma la delantera, especialmente cuando se cuenta con un valor N grande. Esto se debe al aprovechamiento eficaz de los recusrsos de procesamiento disponibles para el aceleramiento de la ejcución de tareas.

* Escalabilidad: Se puede observar una clara diferencia en el tiempo de ejución, en especial una vez más en el momento en el que N se hace más grande, ya que en situaciones así la respuesta paralela y su alta escalabilidad se convierten en una clara opción para la reducción de tiempo de procesamiento.

* Consistencia de resultados: Es importante verificar que ambas soluciones (secuencial y paralela) produzcan resultados consistentes. En este caso y por fortuna para el desarrollo del taller hubo cosistencia de resultados.

* Uso de recursos: Claramente y como se mencionó anteriormente el plus de la solución paralela se debe al mayor utilizamiento de recursos del sistemas como lo son: CPU y memoria, esto puede afectar cuando se cuenta con herramientas de recursos limitados, por eso lo ideal es lograr un equilibrio entre rendimiento y uso de recursos adicionales.

* Optimización y paralelización: Es importante destacar que esta práctica nos permite notar y entender que no todos los problemas serán adecuados para implementar una solución paralela y será prudente elegir cuando verdaderamente se necesite.


