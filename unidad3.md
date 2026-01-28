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
🔹 **Enviado por valor:** Se envía el contenido de la variable, ejemplo=5, se envía el 5 a la función que lo utilizara en sus instrucciones, pero la variable original no se altera.
Ejemplo: 

🔹 **Envío por referencia:** Se envía la dirección de memoria de la variable es decir si dentro de la función se realiza algún cambio pues la variable fuera de la función sufrirá este cambio.
Ejemplo:


### 🧪 Ejemplo en lenguaje C
```c
#include <stdio.h>

int sumar(int a, int b) {
    return a + b;
}

int main() {
    int resultado = sumar(5, 3);
    printf("La suma es: %d", resultado);
    return 0;
}
```

### 📦Estructuras de Datos Estáticas

Las estructuras de datos estáticas son aquellas cuyo tamaño se define antes de la ejecución del programa y no puede cambiar durante su funcionamiento. Se almacenan en posiciones de memoria fijas, lo que las hace rápidas y eficientes.

### 🔹 Características

- 📏 Tamaño fijo
- ⚡ Uso eficiente de la memoria
- 🚀 Acceso rápido a los datos
- 🔒 No permiten crecimiento dinámico

### 📚 Tipos comunes

- 🧮 Arreglos (vectores)
- 🗂️ Matrices
- 🧱 Estructuras (struct) con tamaño definido

### 🧪 Ejemplo de arreglo estático en C
```c
int notas[5] = {8, 9, 7, 10, 6};
```

### 🧪 Ejemplo de estructura estática en C
```c
struct Estudiante {
    char nombre[30];
    int edad;
    float promedio;
};
```

### 🔗 Relación entre Programación Modular y Estructuras de Datos Estáticas

La programación modular organiza el código en funciones bien definidas, mientras que las estructuras de datos estáticas permiten almacenar información de manera ordenada y eficiente. Juntas permiten desarrollar programas claros, estructurados y fáciles de mantener.


La programación modular mejora la organización y el mantenimiento del software, y las estructuras de datos estáticas permiten manejar información cuando el tamaño de los datos es conocido. Ambos conceptos son fundamentales en el desarrollo de programas académicos y aplicaciones básicas.

---

### ⚠️ Principales Dificultades
Entre las principales dificultades encontradas se destacan:
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
