## 📘 Contenidos de la Unidad

### 🔀 Estructuras Condicionales
Las **estructuras condicionales** permiten que un programa tome decisiones según se cumpla o no una condición determinada.  
Durante esta unidad se estudiaron los diferentes tipos de estructuras condicionales, como la **simple**, **doble** y **múltiple**, aplicándolas en la resolución de problemas básicos.

- ✅ Utilizamos los condicionales: `if`,`if...else` y `switch`.

Esto permitió comprender cómo las decisiones influyen en el comportamiento del programa.

Ejemplo de Condicional **If**:
```pseudocode
#include <stdio.h>

int main(){

    int valor1, valor2, suma;

    printf("Ingrese el primer valor:\n");
    scanf("%i", &valor1);
    printf("Ingrese el segundo valor:\n");
    scanf("%i", &valor2);

    if(valor1<=valor2){
       suma=valor1+valor2;
       printf("La suma de los dos numeros es: %i", suma);

    }


   return 0;

}
```

Ejemplo de Condicional **If..else**:
```pseudocode
#include <stdio.h>

int main(){

    int num;

    printf("Ingrese un numero: ");
    scanf("%i", &num);
    getchar();


    primer caso 
    if(num % 2 == 1){
    printf("El numero %i es impar\n", num);
    } else {
     printf("El numero %i es par\n", num);
    }

 return 0;
}
```
Ejemplo de Condicional **Switch**:
```pseudocode
#include <stdio.h>

int main(){

    int dia;

    printf("Ingrese el dia de la semana en numero del 1 al 7: ");
    scanf("%i", &dia);
    getchar();

    switch (dia)
    {
    case 1:
        printf("Es lunes.\n");
        break;
    case 2:
        printf("Es martes.\n");
        break;
    case 3:
        printf("Es miercoles.\n");
        break;
    case 4:
        printf("Es jueves.\n");
        break;
    case 5:
        printf("Es viernes.\n");
        break;
    case 6:
        printf("Es sabado.\n");
        break;
    case 7:
        printf("Es domingo.\n");
        break;
    
    default:
        printf("Numero no valido.");
        break;

    }

    return 0;
}
```
---

### 🔁 Estructuras Repetitivas
Las **estructuras repetitivas** o bucles permiten ejecutar un conjunto de instrucciones varias veces, mientras se cumpla una condición.  
Se analizaron los principales tipos de estructuras repetitivas:
- `while`
- `do-while`
- `for`

Los ejercicios fueron desarrollados utilizando **diagramas de flujo** y posteriormente codificados en **lenguaje C**, reforzando la lógica de repetición y el control de ciclos.

---

### 🔄 Ejercicio Combinado: Estructuras Condicionales y Repetitivas
Como actividad integradora, se desarrolló un ejercicio que combina **estructuras condicionales y repetitivas**, utilizando un lenguaje de alto nivel como **Java o Python**.

#### 📝 Descripción del problema
Se planteó un problema que requería tomar decisiones y repetir procesos de manera controlada, aplicando correctamente ambas estructuras.

#### 🗺️ Diagrama de flujo simplificado
Se elaboró un diagrama de flujo que representa de forma clara la interacción entre condiciones y ciclos, facilitando la comprensión del algoritmo.

#### 💻 Programa
El algoritmo fue implementado en código, respetando la sintaxis y lógica del lenguaje seleccionado, y garantizando que cumpliera con los requerimientos planteados.

#### ✅ Verificación
Se realizaron pruebas con distintos valores de entrada para comprobar el correcto funcionamiento del programa y validar los resultados obtenidos.

---

### ⚠️ Principales Dificultades
Entre las principales dificultades encontradas durante el desarrollo de los contenidos se destacan:
- La correcta formulación de condiciones lógicas.
- El control adecuado de los ciclos repetitivos para evitar bucles infinitos.
- La interpretación correcta del diagrama de flujo al momento de programar.

---

### 🧠 Reflexión Crítica de los Aprendizajes
Esta unidad permitió fortalecer el **pensamiento lógico y analítico**, comprendiendo cómo las estructuras condicionales y repetitivas son fundamentales en la programación.  
Asimismo, facilitó la transición del pensamiento abstracto al código, mejorando la capacidad para resolver problemas de forma estructurada y eficiente.

---

### 📂 Tareas Entregadas
Durante la unidad se entregaron las siguientes actividades:
- Diagramas de flujo de ejercicios condicionales y repetitivos.
- Programas en lenguaje C.
- Ejercicio integrador desarrollado en Java o Python.
- Evidencias de verificación y pruebas de funcionamiento.

