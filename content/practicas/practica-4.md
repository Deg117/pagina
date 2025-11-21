---
title: "Práctica 4"
date: 2025-01-01

---
             Universidad Autónoma De Baja California


# Práctica 4
## Paradigmas de la Programación
**Alumno:** Gastelum Fierro Brian de Jesus  

**Fecha:** 20/11/2025

Introducción

El paradigma lógico es un enfoque de programación donde los problemas se modelan mediante hechos, reglas y consultas, permitiendo que el motor lógico del lenguaje deduzca respuestas mediante inferencia.

En esta práctica se utilizó Prolog, ideal para representar relaciones, trabajar con bases de conocimiento y resolver problemas mediante lógica.

Primera sesión
Hechos, reglas y bases de conocimiento
En la primera sesión se estudiaron los fundamentos del paradigma lógico y la estructura básica de Prolog.
Los temas principales fueron:

1. Hechos

Los hechos describen propiedades o relaciones verdaderas.
Sintaxis: relación(objeto1, objeto2).
Ejemplos vistos:
cat(tom).
lazy(juan).
loves_to_eat(jorge, pasta).
También se revisaron las reglas para escribir hechos:
Nombres en minúsculas.
Argumentos separados por comas.
Terminan con punto.

2. Reglas
   
Se explicó la sintaxis de reglas con operadores , (conjunción) y ; (disyunción).

3. practica 
codigo 
```prolog
% Base de conocimiento
girl(priya).
girl(natasha).
girl(jasmin).
can_cook(priya).

?- girl(priya).
true.
?- girl(X).
X = priya ;
X = natasha ;
X = jasmin ;
false.
?- can_cook(priya).
true.
?- can_cook(X).
X = priya ;
false.
?- girl(X), can_cook(X).
X = priya ;
false.
?- can_cook(natasha).
false.
?- girl(jasmin).
true.
?- girl(maria).
false.
?- girl(X), \+ can_cook(X).
X = natasha ;
X = jasmin ;
false.
```


Conclusiones

El paradigma lógico permite modelar problemas mediante relaciones y reglas, dejando al motor lógico la tarea de encontrar soluciones.

Prolog demuestra ser un lenguaje poderoso para:
construir bases de conocimiento,
aplicar inferencia lógica,
explorar soluciones mediante backtracking,
trabajar con listas, estructuras y recursión.

[Portafolio](https://github.com/Deg117/Portafolio/tree/main/paradigmas_de_la_programacion)