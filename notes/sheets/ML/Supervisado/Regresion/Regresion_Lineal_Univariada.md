---
title: Regresion_Lineal_Univariada
category:
  - 🤖 ML
subcategory:
  - Supervisado
  - Regresion
tags:
  - ML
  - Supervisado
  - Numérico
  - Regresión
status:
  - 🔵 En Progreso
date: 29_10_2024
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: Regresion_Lineal_Univariada

## ✅ Estado de Compleción
- [x] **Título del algoritmo**
- [x] **Representación gráfica del algoritmo**
- [x] **Introducción al algoritmo y su relevancia**
- [x] **Bases Matemáticas del Algoritmo**
- [x] **Código de ejemplo en Python**
- [x] **Descripción de los tipos de datos aplicables**
- [x] **Supuestos de datos**
- [ ] **Ejemplos de aplicación práctica**
- [x] **Enlaces a recursos adicionales para profundizar en el tema**

---
## 1. Título del Algoritmo

### **Regresión Lineal Univariada**

---
## 2. Representación Gráfica del Algoritmo

![[regresion.png]]

---
## 3. Introducción al Algoritmo 

La **Regresión Lineal Univariada** es uno de los algoritmos fundamentales en el campo del aprendizaje automático. Su principal objetivo es modelar y analizar la relación entre una sola variable independiente (predictora) y una variable dependiente (respuesta) mediante una línea recta. Entre sus ventajas destacan la simplicidad y facilidad de interpretación, el bajo costo computacional y su papel como base para modelos más complejos como las redes neuronales. Sin embargo, también presenta limitaciones, como la capacidad de solo capturar relaciones lineales, la sensibilidad a valores atípicos y la dependencia de que se cumplan los supuestos del modelo, lo que no siempre ocurre en datos reales.  

---
## 4. Bases Matemáticas del Algoritmo

La función hipótesis del modelo es,

$$
y = w_0 + w_1x
$$
En esta ecuación, $y$ es la variable dependiente, $x$ la variable independiente, $w_0$ es la intersección o *bias*, $w_1$ la pendiente que indica el cambio en $y$ por cada unidad de cambio en $x$. 

El objetivo del entrenamiento de este modelo es determinar los coeficientes $w_0$ y $w_1$ que minimicen la diferencia entre las predicciones del modelo y los valores reales, comúnmente utilizando el método de mínimos cuadrados.

---
## 4. Código de Ejemplo en Python

[Ejemplo Regresión Lineal Univariada](C:\Users\arhui\Documents\projects\TAIA\src\basic_code\Regresion_Univariada.ipynb)

---
## 5.  Tipos de Datos

- Numéricos continuos
---
## 6.  Supuestos de los datos 

- Linealidad 
- Independencia de errores (residuos)
- Normalidad de errores
--- 
## 7. Ejemplos de Aplicación

- Ejemplo 1
- Ejemplo 2
---
## 8. Recursos Adicionales

- [Simulador regresión Lineal](https://phet.colorado.edu/sims/html/least-squares-regression/latest/least-squares-regression_all.html?locale=es)
- [Curso sobre Regresión Lineal](https://www.coursera.org/learn/machine-learning?specialization=machine-learning-introduction)
---
