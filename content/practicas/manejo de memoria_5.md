---
title: "Manejo de memoria"
date: 2025-01-01
draft: false
---
Universidad Autónoma De Baja California ![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.001.png)![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.002.png)

Grupo-941 23/09/2025 

Alumno: 

Gastelum fierro Brian de Jesus 

Ejercicio 1 

Analiza el siguiente código en C y determina la salida del programa. Explica qué tipo de memoria (estática, dinámica o automática) se usa en cada caso. 

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.003.jpeg)

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.004.png)

Se utiliza  

En la variable global\_var y static\_var se usa memoria estatica En la variable local\_var se usa memoria automatica 

Ejercicio 3 

Analiza el siguiente código y encuentra el error relacionado con la memoria dinámica. 

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.005.jpeg)

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.006.png)

1. ¿Qué problema de manejo de memoria presenta este código? 

Se reserva memoria dinámica con malloc dentro de allocate\_memory(). Esa memoria nunca se libera con free. 

2. ¿Cómo podríamos solucionarlo? 

Liberando la memoria con free(arr) una vez que ya no la necesitamos 

El siguiente código usa pthread para crear un subproceso que modifica una variable global. Analiza la ejecución y predice la salida. 

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.007.jpeg)

![](Aspose.Words.dddbaa33-12d5-4d39-accf-9048ed1529ca.008.png)

¿Cual es la salida esperada del programa? 

Shared\_Var : 15 

¿Qué pasaría si removemos pthread\_join(thread,Null)? Me imprime 5  
