# Resumen de Combinatoria, Sucesiones y Matrices

## Combinatoria

### 1. Permutaciones

- **Permutaciones sin repetición**:
  
  La fórmula para calcular el número de formas de ordenar \( r \) elementos de un conjunto de \( n \) elementos es:

  $$P(n, r) = \frac{n!}{(n-r)!}$$

- **Permutaciones con repetición**:
  
  Si los elementos pueden repetirse, la fórmula es:

  $$P_{\text{rep}}(n, r) = n^r$$

### 2. Combinaciones

- **Combinaciones sin repetición**:

  $$C(n, r) = \frac{n!}{r!(n-r)!}$$

- **Combinaciones con repetición**:

  $$C_{\text{rep}}(n, r) = \frac{(n+r-1)!}{r!(n-1)!} $$

### 3. Teorema del Binomio

El teorema del binomio te permite expandir expresiones de la forma \( (a + b)^n \).

$$(a + b)^n = \sum_{k=0}^{n} \binom{n}{k} a^{n-k} b^k $$

Donde \( \binom{n}{k} \) es el coeficiente binomial.

### 4. Principio de Inclusión y Exclusión

Este principio se utiliza cuando necesitamos contar elementos que cumplen varias condiciones, con superposiciones. Por ejemplo, para contar números entre 1 y 100 que son múltiplos de 3 o 5, debemos aplicar inclusión y exclusión para evitar contar dos veces los múltiplos de 15.

---

## Sucesiones

### 1. Sucesión Aritmética

Es una sucesión en la que la diferencia entre términos consecutivos es constante.

- **Fórmula general**:

  $$a_n = a_1 + (n-1) d$$

  Donde \( a_n \) es el \( n \)-ésimo término, \( a_1 \) es el primer término y \( d \) es la diferencia común.

- **Suma de los primeros \( n \) términos**:

  $$S_n = \frac{n}{2} (a_1 + a_n)$$

  O también:

  $$S_n = \frac{n}{2} \left( 2a_1 + (n-1) d \right)$$

### 2. Sucesión Geométrica

Es una sucesión en la que cada término se obtiene multiplicando el término anterior por una constante llamada "razón".

- **Fórmula general**:

  $$a_n = a_1 \cdot r^{(n-1)}$$

  Donde \( r \) es la razón (constante multiplicativa).

- **Suma de los primeros \( n \) términos** (si \( r \neq 1 \)):

  $$S_n = \frac{a_1(1 - r^n)}{1 - r}$$

---

## Matrices

### 1. Definición y Notación

Una **matriz** es un arreglo rectangular de números dispuestos en filas y columnas.

- **Ejemplo** de matriz \( 2 \times 3 \):

$$A = \begin{pmatrix} 1 & 2 & 3 \\
4 & 5 & 6 \end{pmatrix}$$

### 2. Operaciones Básicas con Matrices

- **Suma**: Las matrices solo se pueden sumar si tienen las mismas dimensiones. Se suman elemento por elemento.

- **Multiplicación por un escalar**: Multiplicas cada elemento de la matriz por un número.

- **Multiplicación de matrices**: La multiplicación de matrices requiere que el número de columnas de la primera matriz sea igual al número de filas de la segunda matriz. El elemento \( c_{ij} \) de la matriz producto es la suma de los productos de los elementos de la fila \( i \) de la primera matriz y la columna \( j \) de la segunda matriz.

- **Transposición de una matriz**: La **matriz transpuesta** de una matriz \( A \) se denota por \( A^T \), y consiste en intercambiar las filas y las columnas de \( A \).

### 3. Determinantes y Matrices Inversas

- **Determinante**: El determinante de una matriz cuadrada es un número asociado que nos ayuda a determinar si la matriz es invertible (si su determinante es distinto de cero). Para una matriz \( 2 \times 2 \), la fórmula es:

  $$\text{det}(A) = ad - bc$$

- **Matriz inversa**: La matriz inversa \( A^{-1} \) de una matriz \( A \) es tal que:


  $$  A^{-1} = \frac{1}{\text{det}(A)} \begin{pmatrix}  d & -b \\ -c & a \end{pmatrix} $$



  Asegúrate de verificar que el determinante no sea cero antes de calcular la inversa.

### 4. Sistemas de Ecuaciones Lineales

Los sistemas de ecuaciones lineales se pueden resolver usando matrices. El sistema se representa como:

$AX = $$

Donde \( A \) es la matriz de coeficientes, \( X \) es el vector de incógnitas y \( B \) es el vector de resultados. Para resolver el sistema:

- **Eliminación de Gauss**: Puedes utilizar la eliminación de Gauss para convertir la matriz aumentada en una forma escalonada.

- **Inversa de la matriz**: Si la matriz \( A \) es invertible, puedes resolver el sistema multiplicando ambos lados de la ecuación por \( A^{-1} \):

  $$X = A^{-1} B$$

---

## Resumen Final

- **Combinatoria**: Domina las fórmulas para permutaciones y combinaciones, tanto con repetición como sin repetición, el teorema del binomio y el principio de inclusión y exclusión.
  
- **Sucesiones**: Aprende a manejar sucesiones aritméticas y geométricas, sus fórmulas generales y cómo sumar los primeros \( n \) términos.

- **Matrices**: Familiarízate con las operaciones básicas, el cálculo del determinante, la inversa de matrices, y cómo resolver sistemas de ecuaciones lineales utilizando matrices.

Con estos conceptos, tendrás una buena base para resolver los ejercicios del examen y ejercicios similares. ¡No dudes en pedirme más ejemplos o aclaraciones si los necesitas!
