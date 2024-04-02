# Teoría de conjuntos con Python

La teoría de conjuntos es un area fundamental de las matematicas que trata sobre las propiedades y relaciones entre conjuntos, que son colecciones bien definidos de objetos. Python, como lenguaje de programación versatil, ofrece varias formas de trabajar con conjuntos y aplicar conceptos de teoría de conjuntos


## Creación de conjuntos

En python, puedes crear un conjunto utilizando llaves [] o la función set()


```python
A = {1, 2, 3, 4, 5}
```


```python
B = {3, 4, 5, 6, 7}
```


```python
C = set([3, 6, 12, 15])
```

## Listas vs conjuntos


```python
lista = [1, 2, 3, 4, 5, 1, 2, 3, 4, 5]
```


```python
lista


```




    [1, 2, 3, 4, 5, 1, 2, 3, 4, 5]




```python
conjunto = set(lista)

```


```python
conjunto
```




    {1, 2, 3, 4, 5}



## Operaciones

Python proporciona operadores y métodos para realizar operaciones basicas de conjuntos como unión, intersección, diferencia y diferencia simétrica.

### Unión

Formalmente, si A y B son conjuntos, la unión de A y B se define como el conjunto C que contiene todos los elementos que pertenecen a A, a B, o a ambos.
Matemáticamente, esto se puede expresar como:

$$
    C = A \cup B = {x:x \in A \quad x \in B}
$$

En Python, la operación de unión puede realizarse utilizando el operador | o el método unión()


```python
A | B
```




    {1, 2, 3, 4, 5, 6, 7}




```python
A.union(B)
```




    {1, 2, 3, 4, 5, 6, 7}



### Intersección

La intersección de conjuntos, en teoría de conjuntos, es una operación que combina dos o más conjuntos para crear un nuevo conjunto que contiene solo los elementos que pertenecen a todos los conjuntos originales. En otras palabras, la intersección es el conjunto de elementos que son comunes a todos los conjuntos.

Si A y B son conjuntos, la intersección de A y B se define como el conjunto C que contiene solo los elementos que pertenecen a ambos conjuntos A y B.

Matemáticamente, esto se puede expresar como:

$$
C = A \cap B = {x : x \in A \text{ y } x \in B}
$$

En Python, la operación de intersección puede realizarse utilizando el operador & o el método intersection(B)



```python
A & B

```




    {3, 4, 5}




```python
A.intersection(B)
```




    {3, 4, 5}



### Diferencia

Si A y B son conjuntos, la diferencia de A y B se define como el conjunto C que contiene todos los elementos que pertenecen a A pero no a B.

Matemáticamente, esto se puede expresar como:

$$
C = A - B = {x:x \in A \quad x \notin B}
$$

En Python, la operación de diferencia se puede realizar utilizando el operador - o el método difference():



```python
A - B
```




    {1, 2}




```python
A.difference(B)
```




    {1, 2}



### Diferencia simétrica

Formalmente, si A y B son conjuntos, la diferencia simétrica de A y B se define como el conjunto C que contiene todos los elementos que pertenecen a uno solo de los conjuntos A o B, pero no a ambos.

Matemáticamente, esto se puede expresar como:

$$
C = A \triangle B = \{x : x \in A \text{ y } x \notin B \text{ o } x \in B \text{ y } x \notin A\}
$$

En Python, la operación de diferencia simétrica puede realizarse utilizando el operador ^ o el método diferencia_simetrica().


```python
A ^ B
```




    {1, 2, 6, 7}




```python
C = A.symmetric_difference(B)
```


```python

```
