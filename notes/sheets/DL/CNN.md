---
title: CNN
category:
  - 🧠 DL
subcategory:
  - CV
tags:
  - Etiqueta1
  - Etiqueta2
  - Etiqueta3
status:
  - 🔵 En Progreso
date: 19_11_2024
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: CNN

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

###  **Redes Neuronales Convolucionales *(CNN)*** 

---
## 2. Representación Gráfica del Algoritmo

![[cnn_icon.png]]

Referencia: <a href="https://www.flaticon.es/iconos-gratis/vision-de-maquina" title="vision-de-maquina iconos">Vision-de-maquina iconos creados por Freepik - Flaticon</a> 

---
## 3. Introducción al Algoritmo 

Una **Red Neuronal Convolucional** (*CNN*, por sus siglas en inglés) son un tipo de modelo del aprendizaje profundo, las cuales están diseñadas para procesar datos con **estructura matriciales**. Deben su nombre, debido a que su arquitectura se compone principalmente de **capas convolucionales** que aplican filtros (o **kernels**) para extraer características locales. Otro rasgo relevante de la arquitectura son las **capas de pooling**, las cuales reducen las dimensiones espaciales, optimizando el rendimiento y mitigando el sobreajuste. 

*Los conceptos fundamentales de este tipo de redes, incluyen el campo receptivo, que determina el área de entrada que influye en una neurona específica, y los parámetros de stride y padding, que controlan el desplazamiento y el relleno de los filtros durante la convolución. Los kernels son esenciales para detectar patrones como bordes y texturas, aprendidos automáticamente durante el entrenamiento.

Las CNNs han revolucionado campos como la visión por computadora, permitiendo aplicaciones en **reconocimiento de imágenes**, **detección de objetos**, y **análisis de video**, entre otros. Sus ventajas principales son la extracción automática de características, la eficiencia computacional mediante el compartimiento de parámetros y la capacidad de escalar a entradas de alta dimensión. Sin embargo, enfrentan desafíos como la necesidad de grandes volúmenes de datos y la interpretabilidad de sus decisiones. 

---
## 4. Bases Matemáticas del Algoritmo

 En el corazón funcional y matemático de una CNN es la **operación de convolución**, la cual aplica un filtro sobre la entrada para generar **mapas de características**. Matemáticamente, esta operación se expresa como:

$$
(I * K)(i, j) = \sum_{m=1}^{M} \sum_{n=1}^{N} I(i+m, j+n) \cdot K(m, n)
$$

Para introducir no linealidad y permitir la modelación de relaciones complejas, se utilizan **funciones de activación** como la ReLU, definida por:

$$
\text{ReLU}(x) = \max(0, x)
$$

Durante el entrenamiento, se emplea una **función de pérdida** que mide la discrepancia entre las predicciones de la red y las etiquetas reales. Una común es la entropía cruzada:

$$
L = -\sum_{c=1}^{C} y_c \log(\hat{y}_c)
$$

El proceso de **backpropagation** calcula los gradientes necesarios para ajustar los pesos de la red, utilizando la fórmula:

$$
\frac{\partial L}{\partial w} = \frac{\partial L}{\partial \hat{y}} \cdot \frac{\partial \hat{y}}{\partial w}
$$

Posteriormente, se optimizan los pesos mediante el método de **Descenso de Gradiente Estocástico (SGD)**:

$$
w := w - \eta \frac{\partial L}{\partial w}
$$

Para evitar el sobreajuste, se aplica la **regularización por Dropout**, que desactiva aleatoriamente neuronas durante el entrenamiento:

$$
\text{Dropout}(x) = 
\begin{cases}
0 & \text{con probabilidad } p \\
\frac{x}{1-p} & \text{de otro modo}
\end{cases}
$$


### 4.1 Ilustración del funcionamiento (*Opcional*)

![[cnn_des.png]]

**Referencia:** https://www.analytixlabs.co.in/blog/convolutional-neural-network/

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