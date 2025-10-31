## 📘 Contenidos de la Unidad

#### 🧮 Algoritmos, Pseudocódigo y Diagramas de Flujo
Los **algoritmos** son una serie de pasos ordenados que permiten resolver un problema o realizar una tarea específica.  Los usamos en nuestra vida diaria, por ejemplo, el algoritmo para ir a clases:
```pseudocode
1.	Despertarse
2.	Ducharse
3.	Vestirse
4.	Desayunar 
5.	Lavarse los dientes
6.	Alistar los materiales
7.	Salir de casa
8.	Ir a clases
```
El **pseudocódigo** se utiliza para representar un algoritmo de forma estructurada, usando un lenguaje similar al natural, pero con reglas de programación básicas.  Una de las herramientas más útiles y fáciles de utilizar es Pseint, la cual utilizamos en esta unidad.
Ejemplo de pseudocódigo en Pseint para sumar dos números:
```pseudocode
Algoritmo suma_dosNumeros
    Definir a como real;
    Definir b como real;
    Definir suma como real;
    Escribir "Ingrese el primer número:";
    Leer a;
    Escribir "Ingrese el segundo número:";
    Leer b;
    suma = a + b;
    Escribir "La suma es igual a:", suma;
FinAlgoritmo
```
Por su parte, el **diagrama de flujo** representa gráficamente los pasos del algoritmo mediante símbolos estandarizados (óvalos, rombos, rectángulos, flechas, etc.), facilitando su comprensión visual. Aquí el diagrama del ejemplo anterior: (Ver imagen 1)

<p align="center">
<img width="663" height="633" alt="image" src="https://github.com/user-attachments/assets/23ac93e8-8f85-47e4-ba52-6dc89d417cc4" />
</p>
<p align="center"> Imagen 1: Diagrama de flujo Pseint.</p>

---

#### 🧩 Programación por bloques
La **programación por bloques** es una metodología visual que permite crear programas mediante bloques gráficos que representan instrucciones, sin necesidad de escribir código textual.  
Se usa ampliamente para el aprendizaje inicial, ya que permite comprender la lógica de manera sencilla.  

🧱 **Ejemplos de plataformas:**  
- Scratch 🐱  
- Blockly 🧠  
- Pilas Bloques 📱
  
Ejemplo de la interfaz de Pilas Bloques: (Ver imagen 2 y 3)

<p align="center">
<img width="260" height="170" alt="image" src="https://github.com/user-attachments/assets/b8be3127-67b4-4807-85b9-c5f3b58eb391" />
<img width="285" height="283" alt="image" src="https://github.com/user-attachments/assets/ee92f3cb-4e34-48ce-9f35-39960441ece9" />
</p>
<p align="center"> Imagen 2 y 3: Interfaz Pilas Bloques.</p>
 
---
### 💻 Lenguaje C
C es un lenguaje de programación de propósito general, desarrollado a principios de los años 70 por Dennis Ritchie en los laboratorios Bell de AT&T. Fue creado inicialmente para implementar el sistema operativo UNIX, pero su simplicidad, eficiencia y flexibilidad lo han convertido en uno de los lenguajes más influyentes de la historia de la informática.[1]
Aunque es considerado un lenguaje de medio nivel —porque combina características de lenguajes de alto y bajo nivel—, C permite una manipulación directa de la memoria, lo que lo hace ideal para sistemas operativos, controladores de hardware, software embebido y otras aplicaciones que requieren eficiencia cercana al hardware.[1]

En el lenguaje C encontramos las librerías, que son archivos de código para realizar operaciones y cálculos de uso frecuente y son parte de cada compilador. Su extensión es **.h** 
Ejemplo: **stdio.h** 
La cual es indispensable pues contiene los prototipos de funciones y los tipos de datos para manipular sus entradas y salidas.

Es importante recalcar también que en C el programa empieza siempre desde la función **main()**.

Los comandos básicos son:
- Compilar: programa.c -o programa
- Ejecutar: .\programa.exe


### ⚙️ Código en C para sumar dos números:
 ```pseudocode
#include <stdio.h>
#include <float.h>

int main(){


    float valor1 , valor2 , suma ;


    printf("Ingrese el primer numero:\n");
    scanf("%f", &valor1);
    printf("Ingrese el segundo numero:\n");
    scanf("%f", &valor2);

    suma = valor1 + valor2;

    printf("La suma es: %2.f", suma);


return 0;

}
 ```

## 🗺️Tareas entregadas 
-	🧮 Herramientas de algoritmos (pseudocódigo y diagramas de flujo).

- 💻 Instalación de lenguajes de programación (C, Python o Java).

- 🧩 Primer acercamiento a la construcción de algoritmos con estructuras secuenciales en pseudocódigo.

- 🧠 Del diseño del algoritmo a la construcción del programa.
  
  <p align="center">
  <a href="https://drive.google.com/drive/folders/1ts2qCX0A8Ql9N2S3iDyLzKVBrqQIzWiV?usp=drive_link" target="_blank">
    <img src="https://img.shields.io/badge/Abrir%20en%20Google%20Drive-ff69b4?style=for-the-badge&logo=google-drive&logoColor=white" alt="Abrir en Google Drive">
  </a>
</p>

## 💭 Reflexión

En esta unidad comprendí la importancia del uso de PSeInt como herramienta de apoyo para iniciarnos en el mundo de la programación.
Además, aprendí que la práctica constante es esencial para fortalecer nuestras habilidades en distintos lenguajes y mejorar nuestra capacidad para resolver problemas de manera lógica y estructurada.

