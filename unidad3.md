# 💻 Programación Modular y Estructuras de Datos Estáticas

---

## 🧩 Programación Modular

La **programación modular** es una técnica de desarrollo de software que consiste en dividir un programa en partes más pequeñas llamadas **módulos** o **funciones**, donde cada una realiza una tarea específica. Esto permite crear programas más organizados, legibles y fáciles de mantener.

### 🔹 Características
- 📌 Divide el programa en módulos independientes  
- ⚙️ Cada módulo cumple una función específica  
- 🔁 Permite reutilizar código  
- 🛠️ Facilita el mantenimiento y la depuración  

### ✅ Ventajas
- ✨ Código más ordenado y claro  
- ❌ Reducción de errores  
- 👥 Facilita el trabajo en equipo  
- 📈 Mejora la escalabilidad del programa  

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

