## 📘 Contenidos de la Unidad

### 🔀 Estructuras Condicionales
Las **estructuras condicionales** permiten que un programa tome decisiones según se cumpla o no una condición determinada.  
Durante esta unidad se estudiaron los diferentes tipos de estructuras condicionales, como la **simple**, **doble** y **múltiple**, aplicándolas en la resolución de problemas básicos.

- ✅ Utilizamos los condicionales: `if`,`if...else`,`if...else..if` y `switch`.

- **`if`**  
  Se utiliza cuando se necesita evaluar una sola condición.  
  Si la condición es verdadera, se ejecuta un bloque de instrucciones; si es falsa, el programa continúa sin ejecutar dicho bloque.

- **`if...else`**  
  Permite evaluar una condición y ejecutar un bloque de instrucciones si esta es verdadera, y otro bloque diferente si la condición es falsa.  
  Se emplea cuando existen dos posibles caminos de ejecución.

- **`if...else...if`**  
  Se usa cuando es necesario evaluar **varias condiciones** de manera secuencial.  
  El programa ejecuta el bloque correspondiente a la primera condición que resulte verdadera; si ninguna se cumple, se puede incluir un bloque `else` final.

- **`switch`**  
  Es una estructura de selección múltiple que se utiliza cuando se compara una misma variable contra distintos valores posibles.  
  Facilita la lectura del código y organiza mejor las decisiones cuando existen muchas opciones.
  
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

<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/b6c4023d-0634-4bc0-badb-6253a5477755"
       width="480"
       alt="Figura 1: Diagrama de flujo del algoritmo de suma">
</p>


<p align="center">
  <em> Imagen 1: Diagrama de flujo de código con estructura condicional <code>if</code>.</em>
</p>


Ejemplo de Condicional **if..else**:
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
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/bfff0604-f3b7-4d64-822a-d8bee06bc23c"
       width="480"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 2: Diagrama de flujo del algoritmo Par o Impar <code>if..else</code>.</em>
</p>

Ejemplo de Condicional **if..else..if**:
```pseudocode
#include <stdio.h>

int main(){
    float num1, num2;
    char op;

    printf("Ingrese el primer numero: ");
    scanf("%f", &num1);
    getchar();

    printf("Ingrese el segundo numero: ");  
    scanf("%f", &num2);
    getchar();

    printf("Ingrese el operador +, -, * o /: ");
    scanf("%c", &op);
    getchar();

    if (op == '+'){
        printf("El resultado es: %2.f", num1+num2);
    }else if (op == '-'){
        printf("El resultado es: %2.f", num1-num2);
    }else if (op == '*'){
        printf("El resultado es: %2.f", num1*num2);
    }else if (op == '/'){
        printf("El resultado es: %2.f", num1/num2);
    }else{
        printf("Operador no valido.\n");
    }
        
    return 0;
}
```

<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/bb8e35e4-5904-44a5-9402-8376054ac4ed"
       width="800"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 3: Diagrama de flujo del algoritmo Operaciones <code>if..else..if</code>.</em>
</p>


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
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/298f4b56-99d6-4ab5-87e4-9811ca416d3f"
       width="800"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 4: Diagrama de flujo del algoritmo Semana <code>switch</code>.</em>
</p>

---

### 🔁 Estructuras Repetitivas
Las **estructuras repetitivas** o bucles permiten ejecutar un conjunto de instrucciones varias veces, mientras se cumpla una condición.  
- ✅ Se analizaron los principales tipos de estructuras repetitivas: `while`, `do-while` y `for`.

- **`while`**  
  Ejecuta un bloque de instrucciones **mientras la condición sea verdadera**.  
  La condición se evalúa *antes* de entrar al ciclo, por lo que es posible que **no se ejecute ninguna vez** si la condición inicial es falsa.
  
- **`do-while`**  
  Similar al `while`, pero con una diferencia importante: **el bloque se ejecuta al menos una vez**, ya que la condición se evalúa *después* de ejecutar las instrucciones.  
  Se usa cuando se necesita que la acción ocurra mínimo una vez antes de validar la condición.

- **`for`**  
  Se utiliza cuando se conoce de antemano el número de repeticiones.  
  Integra en una sola línea la **inicialización**, la **condición** y el **incremento o decremento**, permitiendo recorrer rangos o ejecutar iteraciones de forma más ordenada y controlada.

Ejemplo de Boucle **While**:
```pseudocode
#include <stdio.h>

int main() {
    int contador = 0;
    int acumulador = 0;

    while ( contador <= 5){
        acumulador = acumulador + contador;
        contador ++;
    }

    printf("El valor sumado es: %d\n", acumulador);

    return 0;
}
```
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/f1224194-42a9-4a53-801b-eb62c8771ee2"
       width="480"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 5: Diagrama de flujo del algoritmo Suma <code>while</code>.</em>
</p>

Ejemplo de Boucle **Do..while**:
```pseudocode
#include <stdio.h>

int main(){

    int contador = 1;

    printf("Tabla del 2:\n");

    do {
        printf("2 x %i = %i\n", contador, 2 * contador);
        contador = contador + 1;
    } while (contador <= 12);

    return 0;
}
```
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/e079d5f7-1133-4a15-a6f6-d4ac40e51538"
       width="480"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 6: Diagrama de flujo del algoritmo Tabla del 2 <code>do..while</code>.</em>
</p>
Ejemplo de Boucle **Do..while**:

```pseudocode
#include <stdio.h>

int main (){
    int cont;
    for (int cont = 10; cont  >= 1; cont--){
        printf("El numero es : %d\n", cont);
    }

    return 0;
}
```
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/b1009f01-125f-432b-b0c0-41d804c40a57"
       width="480"
       alt="Figura 2: Diagrama de flujo del algoritmo Par o Impar">
</p>


<p align="center">
  <em> Imagen 7: Diagrama de flujo del algoritmo Temperatura <code>for</code>.</em>
</p>

---

### 🔄 Ejercicio Combinado: Estructuras Condicionales y Repetitivas
Como actividad integradora, se desarrolló un ejercicio que combina **estructuras condicionales y repetitivas**, utilizando **Python**.

#### 📝 Descripción del problema
Escribe un programa en Python que:
- Pida al usuario la cantidad de estudiantes que desea registrar.
- Para cada estudiante, solicite 3 notas.
- Calcule el promedio de cada estudiante.
- Use un condicional para determinar si el estudiante aprueba (promedio ≥ 7) o reprueba.
- Al final, muestre: Cuántos estudiantes aprobaron, cuántos reprobaron y el promedio general del curso.

#### 🗺️ Diagrama de flujo simplificado
<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/57945e9c-1893-462b-8ae4-dd5d10ecbc20"
       width="800"
</p>

<p align="center">
  <em> Imagen 8: Diagrama de flujo del algoritmo en lenguaje Python .</em>
</p>

#### 💻 Programa
```pseudocode
# Contadores
aprobados = 0
reprobados = 0
suma_promedios = 0

cantidad = int(input("Ingrese la cantidad de estudiantes: "))

for i in range(1, cantidad + 1):
    print(f"\nEstudiante {i}")
    
    # Pedimos 3 notas
    nota1 = float(input("Ingrese la nota 1: "))
    nota2 = float(input("Ingrese la nota 2: "))
    nota3 = float(input("Ingrese la nota 3: "))
    
    # Promedio del estudiante
    promedio = (nota1 + nota2 + nota3) / 3
    suma_promedios += promedio

    # Condicional para determinar si aprueba
    if promedio >= 7:
        print("El estudiante aprueba.")
        aprobados += 1
    else:
        print("El estudiante reprueba.")
        reprobados += 1

# Promedio general del curso
promedio_general = suma_promedios / cantidad

print("\n--- RESULTADOS ---")
print(f"Estudiantes aprobados: {aprobados}")
print(f"Estudiantes reprobados: {reprobados}")
print(f"Promedio general del curso: {promedio_general:.2f}")
```

#### ✅ Verificación

<p align="center">
  <img 
       src="https://github.com/user-attachments/assets/4feb05e8-e559-44e9-89ac-97b919002acb"
       width="800"
</p>

<p align="center">
  <em> Imagen 9: Captura de pantalla de la terminal de VSCode  .</em>
</p>
  
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

**- AA:**

Tarea 1:

<p align="center">
  <a href="https://drive.google.com/drive/u/1/folders/1U90Ip_W-uANIrvghMSaW_h1hnPdydN8y" 
     target="_blank"
     style="
        background:#ff74b7;
        color:white;
        padding:10px 22px;
        border-radius:12px;
        text-decoration:none;
        font-weight:bold;
        font-size:16px;
        ">
    Ver
  </a>
</p>

