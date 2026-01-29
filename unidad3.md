## 📘 Contenidos de la Unidad

### 🧩 Programación Modular

La **programación modular** es una técnica de desarrollo de software que consiste en dividir un programa en partes más pequeñas llamadas **módulos** o **funciones**, donde cada una realiza una tarea específica. Esto permite crear programas más organizados, legibles y fáciles de mantener.

### 🔹 Características:
- 📌 Divide el programa en módulos independientes  
- ⚙️ Cada módulo cumple una función específica  
- 🔁 Permite reutilizar código  
- 🛠️ Facilita el mantenimiento y la depuración  

### ✅ Ventajas:
- ✨ Código más ordenado y claro  
- ❌ Reducción de errores  
- 👥 Facilita el trabajo en equipo  
- 📈 Mejora la escalabilidad del programa

### 🔁 Funciones con envío de parámetros

Los parámetros pueden enviarse de 2 maneras:

🔹 **Envío por valor:** Se envía el contenido de la variable, ejemplo=5, se envía el 5 a la función que lo utilizara en sus instrucciones, pero la variable original no se altera.
Ejemplo: 

```c
#include <stdio.h>

void intercambiarValores();
int main() {
    int a = 3;
    int b= 5;

    intercambiarValores(a, b);
    printf("Valor de a es: %d\n", a);
    printf("Valor de b es: %d\n", b);

    return 0;
}

void intercambiarValores(int x, int y){
    int aux;
    aux = x;
    x = y;
    y = aux;
    
    printf("Valor de x es: %i\n", x);
    printf("Valor de y es: %i\n", y);
} 
```

🔹 **Envío por referencia:** Se envía la dirección de memoria de la variable es decir si dentro de la función se realiza algún cambio pues la variable fuera de la función sufrirá este cambio.
Ejemplo:

```c
#include <stdio.h>
void intercambiarValores(int *x, int *y);
int main() {
    int a = 3;
    int b= 5;

    intercambiarValores(&a, &b);

    printf("Valor de a es: %d\n", a);
    printf("Valor de b es: %d\n", b);

    return 0;
}

void intercambiarValores(int *x, int *y){
    int aux;
    aux = *x;
    *x = *y;
    *y = aux;
    
    printf("Valor de x es: %i\n", *x);
    printf("Valor de y es: %i\n", *y);
}
```

<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/24dac1eb-06c5-49fb-8c26-6e1aaee52d59"
       width="480"
       alt="Figura 1: Diagrama de flujo del algoritmo de suma">
</p>

<p align="center">
  <em> Imagen 2: Salida de la terminal Pase por referencia. <code>if</code>.</em>
</p>



### 📦Estructuras de Datos Estáticas

Las estructuras de datos estáticas son aquellas cuyo tamaño se define antes de la ejecución del programa y no puede cambiar durante su funcionamiento. Se almacenan en posiciones de memoria fijas, lo que las hace rápidas y eficientes.

### 🔹 Características

- 📏 Tamaño fijo
- ⚡ Uso eficiente de la memoria
- 🚀 Acceso rápido a los datos
- 🔒 No permiten crecimiento dinámico

### 📚 Tipos comunes

  **🧮 Arreglos**
  
Los arreglos (también llamados vectores o arrays) son estructuras de datos que permiten almacenar varios valores del mismo tipo dentro de una sola variable, usando un índice para acceder a cada elemento.
📦 En lugar de crear muchas variables, el arreglo las agrupa en una sola.

- **📏Unidimensionales:** Solo tiene una fila y columnas, llamados vector o lista.
Las posiciones del arreglo son llamadas índices y siempre empiezan en cero.

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

int main() {
    int lista[5];
    lista[0] = 8;
    lista[1] = 10;
    lista[2] = 7;
    lista[3] = 5;
    lista[4] = 3;

    for (int i = 0; i < 5; i++) {
        printf("Elemento en la posicion %i: %i\n", i, lista[i]);
    }
    
    return 0;
}
```
- **🔢Bidimensionales:** Cuando tienen varias filas y columnas, llamados también matiz.
La representación es m[i][j], donde i es el número de filas y j número de columnas.

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

int main() {
    int matriz[3][4];
    matriz[0][0] = 1;
    matriz[0][1] = 5;
    matriz[0][2] = 8;
    matriz[0][3] = 3;
    matriz[1][0] = 2;
    matriz[1][1] = 3;
    matriz[1][2] = 6;
    matriz[1][3] = 8;
    matriz[2][0] = 5;
    matriz[2][1] = 7;
    matriz[2][2] = 9;
    matriz[2][3] = 4;
    
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 4; j++) {
            printf("Fila %i, Columna %i: %i\n", i, j, matriz[i][j]);
        }
    }
    return 0;
}
```
- **🧱Tridimensionales:** Cuando tenemos varias filas,  columnas, y profundidad.
La representación es m[i][j][k], donde i es la profundidad, j el número de filas y k el número de columnas.

```c
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

int main() {
    int tridimencional[2][3][2];
    tridimencional[0][0][0] = 1;
    tridimencional[0][0][1] = 4;
    tridimencional[0][1][0] = 6;
    tridimencional[0][1][1] = 8;
    tridimencional[0][2][0] = 3;
    tridimencional[0][2][1] = 7;

    tridimencional[1][0][0] = 2;
    tridimencional[1][0][1] = 5;
    tridimencional[1][1][0] = 9;
    tridimencional[1][1][1] = 11;
    tridimencional[1][2][0] = 10;
    tridimencional[1][2][1] = 12;

    for (int i = 0; i < 2; i++) { //capas
        for (int j = 0; j < 3; j++) { //filas
            for (int k = 0; k < 2; k++) { //columnas 
                printf("Capa: %i, Fila: %i, Columna: %i: %i\n", i, j, k, tridimencional[i][j][k]);
            }
        }
    }

    return 0;
}
```


### 🔗 Relación entre Programación Modular y Estructuras de Datos Estáticas

La programación modular organiza el código en funciones bien definidas, mientras que las estructuras de datos estáticas permiten almacenar información de manera ordenada y eficiente. Juntas permiten desarrollar programas claros, estructurados y fáciles de mantener.


La programación modular mejora la organización y el mantenimiento del software, y las estructuras de datos estáticas permiten manejar información cuando el tamaño de los datos es conocido. Ambos conceptos son fundamentales en el desarrollo de programas académicos y aplicaciones básicas.

---

## ⚠️ Principales Dificultades

Durante el desarrollo de esta unidad se presentaron algunas dificultades relacionadas principalmente con la **modularidad**, el uso de **funciones** y el manejo de **arreglos**, entre las cuales se destacan:

- 🧩 La correcta **descomposición del programa en módulos**, identificando qué partes debían implementarse como funciones independientes.
- 🔧 La definición adecuada de **funciones**, especialmente en el uso de parámetros, valores de retorno y el alcance de las variables.
- 📦 El manejo correcto de **arreglos**, incluyendo su inicialización, recorrido y acceso a los elementos mediante índices.
- 🔢 La prevención de errores comunes como accesos fuera de rango en los arreglos o el uso incorrecto de datos dentro de las funciones.

---

## 🧠 Reflexión Crítica de los Aprendizajes

Esta unidad permitió comprender la importancia de la **programación modular** como una estrategia fundamental para organizar el código de manera clara y estructurada. El uso adecuado de **funciones** facilitó la reutilización del código y mejoró la legibilidad y el mantenimiento de los programas.

Asimismo, el aprendizaje sobre **arreglos** fortaleció la capacidad para almacenar y manipular múltiples datos de forma ordenada, permitiendo resolver problemas de manera más eficiente. En conjunto, estos conocimientos contribuyeron al desarrollo de un pensamiento lógico y analítico, orientado a la creación de soluciones programáticas más estructuradas y eficientes.


---

### 📂 Tareas Entregadas
Durante la unidad se entregaron las siguientes actividades:
**- APE:**

<p align="center">
  <h5><span style="color:#ff66b2;"> — Tarea 1 —</span> <span style="color:black;"></span></h5>
  <a href="https://github.com/seleeanis/TP-Portafolio/blob/main/APE1_U3.pdf" </a>
    <img src="https://img.shields.io/badge/%20Ver%20-ff69b4?style=for-the-badge&logo=github&logoColor=white" alt="Referencias">
  </a>
   </p>
