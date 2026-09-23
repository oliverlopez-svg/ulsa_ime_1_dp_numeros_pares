# Práctica 2: Guardar los números pares
## 1. Descripción del problema (Fase 1)
<!-- Explica con tus palabras qué hace tu programa y para qué serviría en la vida real. Máximo 4 líneas. -->
arr contiene 5 numeros y define cuales son pares e impares, tambien definir su indice. Ignorar los impares, guardar los pares

_____

## 2. Entradas y salidas (Fase 1)
<!-- Define cada entrada y cada salida, con su tipo de dato y su objetivo. -->
entrada: 5 numeros en 5 indices
salida: definir los pares e impares y marcar los datos incorrectos. Todo con su indice. Ignorar los impares y guardar los pares con indice

**Entradas:**
1. _____ 5 numeros

**Salidas:**
1. _____  pares
2. _____sus índices
(errores en caso de dato incorrecto)


## 3. Restricciones e invariante (Fase 1 y 2)

**Restricciones** (¿qué debe cumplirse?):
- _____no decimales
- _____solo terminos numericos

**Tamaño del arreglo y por qué** (piensa en el peor caso):
_____5, en caso de que todos sean pares. o no se rellene nada por datos incorrectos

**¿El 0 y los negativos son pares? ¿Por qué?**
_____no, se marcan como errores en este caso

**Invariante** (¿qué es verdad después de cada vuelta del ciclo?):
_____pasa al siguiente numero 

## 4. Casos resueltos a mano (Fase 1)

| Caso | Números | Pares guardados | Posición de cada par |
|---|---|---|---|
| 1 | 3, 8, 5, 2, 7 | __8,2___ | __2,4___ |
| 2 | 10,20,25,30,35| __10,20,30___ | __1,2,4___ |
| 3 | __7,14,21,28,35___ | __14,28___ | __2,4___ |

## 5. Receta en pseudocódigo (Fase 2)
<!-- Tu receta va en el archivo RECETA.md. Aquí solo responde las dos preguntas. -->
 1 pedir numero
   2 total pares=0
   contador=0
   cantidad=5
   3 MIENTRAS contador<cantidad
   numero-leer entero ("ingresar numero)
   SI al 2 dividirlo entre 2 == 0 ENTONCES 
   pares [totalpares] - numero
   total pares = total pares +1
   Fin MIENTRAS
   4 i-0
   5 mientras i<totalpares> HACER
   mostrar pares [i]
   i- i+1 
   FIN MIENTRAS


**¿Probé mi receta a mano con un caso?** Sí 
**¿Tuve que corregirla?** _____si

## 6. Cómo compilar y ejecutar (Fase 3)

```bash
g++ -Wall -Wextra -std=c++17 main.cpp -o numeros_pares
./numeros_pares
```

## 7. Ejemplo de ejecución (Fase 3)
<!-- Pega aquí lo que muestra tu programa en pantalla con un caso normal. -->

rooney@MacBook-Neo-de-Oliver ulsa_ime_1_dp_numeros_pares % ./main
Ingresa el numero 1: 10
Ingresa el numero 2: 15
Ingresa el numero 3: 20
Ingresa el numero 4: 25
Ingresa el numero 5: 30

Cantidad de numeros pares: 3

## 8. Experimentos (Fase 3)

**Experimento A: ¿qué apareció al imprimir las 5 posiciones del arreglo? ¿Por qué?**
la suma, por que de eso es el codigo
_____

**Experimento B: ¿qué pasó al usar la variable del ciclo como posición del arreglo? ¿Por qué?** cambio por que agregamos variables
_____

## 9. Tabla de pruebas (Fase 4)

| Caso | Números | Esperado | Obtenido | ¿Pasó? |
|---|---|---|---|---|
| Mezcla | 1, 2, 3, 4, 5 | 2 pares: 2, 4 | _____ | _____ |
| Posiciones distintas | 3, 8, 5, 2, 7 | 2 pares: 8, 2 | _____ | _____ |
| Todos pares | 2, 4, 6, 8, 10 | 5 pares | _____ | _____ |
| Todos impares | 1, 3, 5, 7, 9 | 0 pares | _____ | _____ |
| Con cero y negativos | 0, -3, -4, 7, 1 | 2 pares: 0, -4 | _____ | _____ |
| Entrada inválida | `hola` o `3.5` | vuelve a pedir | _____ | _____ |
| Caso propio 1  10 15 20 25 30 
| Caso propio 2  1 2 3 4 6

## 10. Bitácora de mejoras (Fase 4)

| # | ¿Qué falló o qué quise mejorar? | ¿Qué cambié? | ¿Funcionó? |
|---|---|---|---|
| 1 | _____ | _____ | _____ | cambie la sintaxis del codigo
| 2 | _____ | _____ | _____ |

**Reto elegido (opcional):** _____

## 11. Dudas para el profesor (Fase 3)

| Duda | Lo que ya intenté |
|---|---|
| _____ | _____ |

## 12. Reflexión final

**¿Qué aprendí con esta práctica?**
_____ a usar u while y hacer una receta mejor

**Ahora que terminé, ¿qué cambiaría de mi proceso?**
_____ la forma de probar manualmente el pseudocodigo

**¿Qué fue lo más difícil y cómo lo resolví?**
_____el codigo, con ayuda y explicaciones de chatgpt

**¿Qué pregunta me quedó sin responder?**
_____ la forma de hacer una receta mas formal

**¿Por qué no puedo usar la variable del ciclo para guardar en el arreglo?**
_____ por que una indica que numero pedimos y otra la posicion del arreglo

## 13. Lista de verificación antes de entregar (Fase 5)

- [ ] Llené todas las secciones (no quedan `_____`)
- [ ] Mi programa compila sin advertencias
- [ ] Probé todos los casos de la tabla
- [ ] Hice los Experimentos A y B y dejé el código correcto al terminar
- [ ] No modifiqué `utilerias.h`
- [ ] Hice al menos 3 commits con mensajes claros
- [ ] Hice `git push` y verifiqué mi fork en GitHub
- [ ] Entregué el enlace de mi fork en Classroom