---
title: Bosque_Aleatorio
category:
  - 🤖 ML
subcategory:
  - Supervisado
  - Regresion
  - Clasificacion
tags:
  - Etiqueta1
  - Etiqueta2
  - Etiqueta3
status:
  - 🔵 En Progreso
date: 2003-11-30
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: Bosque_Aleatorio

## ✅ Estado de Compleción
- [x] **Título del algoritmo**
- [x] **Representación gráfica del algoritmo**
- [x] **Introducción al algoritmo y su relevancia**
- [x] **Bases Matemáticas del Algoritmo**
- [ ] **Código de ejemplo en Python**
- [ ] **Descripción de los tipos de datos aplicables**
- [ ] **Supuestos de los datos**
- [ ] **Ejemplos de aplicación práctica**
- [ ] **Enlaces a recursos adicionales para profundizar en el tema**
- [ ] **Referencias**

---
## 1. Título del Algoritmo

### **Bosques Aleatorios (*Random Forest*)**

---
## 2. Representación Gráfica del Algoritmo

![[random_forest_icon.png]]

Referencia: https://thenounproject.com/icon/random-forest-1503830/ 

---
## 3. Introducción al Algoritmo 

Random Forest es un algoritmo de aprendizaje automático poderoso y versátil que pertenece a la familia del aprendizaje en conjunto. Desarrollado por Leo Breiman y Adele Cutler, construye múltiples árboles de decisión durante el entrenamiento y produce la moda de sus clasificaciones o la predicción promedio para tareas de regresión. Al aprovechar la técnica de bagging (agregación bootstrap), Random Forest reduce la varianza y mitiga el sobreajuste, mejorando la generalización del modelo. 

Cada árbol en el bosque se entrena con un subconjunto aleatorio de los datos y un subconjunto aleatorio de características, promoviendo la diversidad entre los árboles y aumentando la robustez. Este método sobresale en el manejo de grandes conjuntos de datos con alta dimensionalidad y puede gestionar eficazmente tanto variables numéricas como categóricas. Además, Random Forest proporciona información valiosa sobre la importancia de las características, ayudando en la selección e interpretación de las mismas. Son resistentes al ruido y capaces de capturar relaciones no lineales complejas. 

Debido a su facilidad de uso, escalabilidad y alto rendimiento en diversos dominios—desde finanzas y salud hasta análisis de imágenes y textos—Random Forest se ha convertido en un elemento básico en el conjunto de herramientas de aprendizaje automático. Su capacidad para ofrecer predicciones precisas con una mínima configuración de hiperparámetros lo hace especialmente atractivo tanto para principiantes como para profesionales experimentados.


---
## 4. Bases Matemáticas del Algoritmo

Las bases matemáticas del algoritmo Random Forest se sustentan en el aprendizaje en conjunto, específicamente mediante la técnica de bagging (agregación bootstrap). Matemáticamente, se generan múltiples árboles de decisión $T_1, T_2, \cdots, T_n$, donde cada árbol $T_i$ se entrena sobre una muestra de datos obtenida mediante remuestreo con reemplazo de los datos originales \( D \). Para cada división en un árbol, se selecciona aleatoriamente un subconjunto de características \( m \) de las \( p \) disponibles, lo que introduce diversidad entre los árboles y reduce la correlación entre ellos.

La predicción final para clasificación se obtiene mediante la moda de las predicciones individuales:
$$
\hat{y} = \text{mode}\{T_1(x), T_2(x), \ldots, T_n(x)\}
$$
Para regresión, se calcula el promedio:
$$
\hat{y} = \frac{1}{n} \sum_{i=1}^{n} T_i(x)
$$
La reducción de la varianza se logra al promediar múltiples árboles, lo que minimiza el sobreajuste característico de los árboles individuales. Las medidas de impureza, como el índice de Gini o la entropía, se utilizan para determinar las mejores divisiones en cada nodo. Además, el cálculo de la importancia de las variables se realiza evaluando la disminución de impureza o el incremento en el error fuera de la muestra al permutar cada característica.

El algoritmo Random Forest optimiza la precisión y robustez del modelo mediante la combinación de diversidad y agregación, aprovechando principios estadísticos y probabilísticos para manejar alta dimensionalidad y complejidad en los datos.

### 4.1 Ilustración del funcionamiento 

![[random_forest_des.png]]

**Referencia:** https://anasbrital98.github.io/blog/2021/Random-Forest/ 

---
## 5. Código de Ejemplo en Python

 >**Instrucciones**: Incluir un bloque de código funcional en Python que ilustre la implementación básica del algoritmo. Asegúrese de que el código esté bien documentado.

```python
# Code example in Python

def code_exaple()
	pass
````

---
## 6.  Tipos de Datos

>*Instrucciones:* Detallar los tipos de datos con los que el algoritmo trabaja mejor (por ejemplo, datos tabulares, series de tiempo, imágenes, texto, etc.). Indique también si requiere preprocesamiento de datos específico.

- Tipo 1
- Tipo 2

---
## 7.  Supuestos de los datos

>*Instrucciones:* Para aplicar los algoritmos, muchas veces los datos requieren cumplir ciertas condiciones. En caso de ser así, listarlos. 

- Supuesto 1
- Supuesto 2
--- 
## 8. Ejemplos de Aplicación

> *Instrucciones:* Presentar uno o más ejemplos de problemas reales en los que se haya utilizado el algoritmo con éxito. Pueden incluirse ejemplos típicos de aplicación del algoritmo.

- Ejemplo 1
- Ejemplo 2
---
## 9. Recursos Adicionales

> *Instrucciones:* Proporcionar enlaces a artículos, libros, cursos o tutoriales que permitan profundizar en el estudio del algoritmo.

- [enlace 1](https://www.ibm.com/topics/support-vector-machine#:~:text=A%20support%20vector%20machine%20(SVM,in%20an%20N%2Ddimensional%20space.)
---
## 10. Referencias

- Referencia 1
- Referencia 2