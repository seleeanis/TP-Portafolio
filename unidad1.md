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
Por su parte, el **diagrama de flujo** representa gráficamente los pasos del algoritmo mediante símbolos estandarizados (óvalos, rombos, rectángulos, flechas, etc.), facilitando su comprensión visual. Aquí el diagrama del ejemplo anterior:

<img width="663" height="633" alt="image" src="https://github.com/user-attachments/assets/23ac93e8-8f85-47e4-ba52-6dc89d417cc4" />
---

#### 🧩 Programación por bloques
La **programación por bloques** es una metodología visual que permite crear programas mediante bloques gráficos que representan instrucciones, sin necesidad de escribir código textual.  
Se usa ampliamente para el aprendizaje inicial, ya que permite comprender la lógica de manera sencilla.  

🧱 **Ejemplos de plataformas:**  
- Scratch 🐱  
- Blockly 🧠  
- Pilas Bloques 📱
  
Ejemplo de la interfaz de Pilas Bloques:


<img width="260" height="170" alt="image" src="https://github.com/user-attachments/assets/b8be3127-67b4-4807-85b9-c5f3b58eb391" />
<img width="285" height="283" alt="image" src="https://github.com/user-attachments/assets/ee92f3cb-4e34-48ce-9f35-39960441ece9" />

<p align="center"> Imagen 1 y 2: Interfaz Pilas Bloques.</p>
 
---

#### 🔁 Ejemplos de algoritmos con estructuras lineales o secuenciales
Una **estructura secuencial** ejecuta las instrucciones en el mismo orden en que aparecen, sin tomar decisiones ni repetir pasos.  
Es la forma más simple de control en la programación y se usa para procesos lineales, como cálculos o lecturas de datos.

### 💻 Código para Sumar dos números

 ### ⚙️ Código en C:
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

