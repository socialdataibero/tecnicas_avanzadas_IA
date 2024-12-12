---
title: SVM
category:
  - 🤖 ML
subcategory:
  - Supervisado
  - Clasificacion
  - Regresion
tags:
  - kernel
  - margin
  - support_vectors
  - hyperplane
status:
  - 🔵 En Progreso
date: 24_11_2024
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: SVM

## ✅ Estado de Compleción
- [x] **Título del algoritmo**
- [x] **Representación gráfica del algoritmo**
- [x] **Introducción al algoritmo y su relevancia**
- [x] **Bases Matemáticas del Algoritmo**
- [ ] **Código de ejemplo en Python**
- [x] **Descripción de los tipos de datos aplicables**
- [x] **Supuestos de los datos**
- [x] **Ejemplos de aplicación práctica**
- [x] **Enlaces a recursos adicionales para profundizar en el tema**
- [x] **Referencias**

---
## 1. Título del Algoritmo

### **Máquina de Vectores de Soporte *(SVM)***

---
## 2. Representación Gráfica del Algoritmo

![[svm_icon.png]]

Referencia: http://qingkaikong.blogspot.com/2016/12/machine-learning-7-support-vector.html

---
## 3. Introducción al Algoritmo 

La **Máquina de Vectores de Soporte *(SVM, por sus siglas en inglés)*** se introdujo en los años noventa por Cortes y Vapnik, como una herramienta fundamental en el campo del aprendizaje automático supervisado *(Cortes & Vapnik, 1995)*. Los algoritmos SVM han adquirido relevancia a lo largo de los años por su robustez y flexibilidad en espacios de **alta dimensión** y de datos limitados, así como por su capacidad de manejo de datos **lineales** y **no lineales**, en tareas tanto de **clasificación** como de **regresión** *(Cano Lengua & Papa Quiroz, 2020; Dabas, 2024)*. 

El funcionamiento de una SVM, se basa en la búsqueda de la frontera de separación óptima (**hiperplano**), que mejor separa los puntos de datos entre las clases. Esta frontera maximiza el **margen**, que es la distancia entre el hiperplano y los puntos más cercanos de los datos de cada clase. Estos puntos más cercanos se llaman **vectores de soporte** porque tienen la responsabilidad significativa de definir la posición y orientación del hiperplano. Para el caso de datos no lineales, las SVM transforman el espacio de características original en uno de mayor dimensión donde es posible separar las clases linealmente, a partir de funciones **kernel**.  *(Cortes & Vapnik, 1995; Li, 2024)*. 

Hoy en día, las SVM se aplican en diferentes campos que van desde la clasificación de imágenes hasta la bioinformática. Sin embargo, pese a que se mantienen latentes en la actualidad, su efectividad depende fuertemente de la elección cuidadosa del kernel y de los hiperparámetros, además que pueden requerir gastos computacionales extensivos en aplicaciones a gran escala *(Cano Lengua & Papa Quiroz, 2020; Dabas, 2024)*. 

---
## 4. Bases Matemáticas del Algoritmo

El objetivo clásico e histórico de las SVM, es encontrar un hiperplano que separa dos clases de datos con el **máximo margen** posible. Matemáticamente, el hiperplano se define como: $$ \mathbf{w} \cdot \mathbf{x} + b = 0 $$
donde $\mathbf{w}$ es el vector normal al hiperplano y $b$ es el término de sesgo. El margen $\gamma$ se calcula como: $$ \gamma = \frac{2}{\|\mathbf{w}\|} $$ Maximizar $\gamma$ equivale a minimizar $\|\mathbf{w}\|$. Para asegurar una clasificación correcta, se imponen las restricciones: $$ y_i (\mathbf{w} \cdot \mathbf{x}_i + b) \geq 1, \quad \forall i $$
Este problema de optimización es cuadrático y convexo. Mediante la **formulación dual**, se introducen multiplicadores de Lagrange $\alpha_i$, permitiendo utilizar el **truco del núcleo** (*kernel trick*) para manejar datos no linealmente separables: $$ K(\mathbf{x}_i, \mathbf{x}_j) = \phi(\mathbf{x}_i) \cdot \phi(\mathbf{x}_j) $$ Las SVM también pueden manejar casos donde los datos no son perfectamente separables mediante el **margen suave**, introduciendo variables de holgura $\xi_i$ y un parámetro de regularización $C$: $$ \min \left( \frac{1}{2} \|\mathbf{w}\|^2 + C \sum_{i=1}^m \xi_i \right) $$
**Referencias:**  *(Cano Lengua & Papa Quiroz, 2020; Li, 2024)*
### 4.1 Ilustración del funcionamiento 

![[svm_des.png]]

**Referencia:** https://www.sciencedirect.com/science/article/pii/S2665963822000641

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

- Pueden manejar diversos tipos de datos, siempre que se **representen adecuadamente en forma de vectores de características numéricas**. Estos incluyen:
	-  Numéricos
	-  Categóricos
	-  Texto
	-  Imágenes
	-  Series de tiempo
	- Multimodales
	- etc

---
## 7.  Supuestos de los datos

- **Separabilidad**
	-  Los datos son o pueden (mediante transformaciones) ser separables por un margen claro.
- **Escalado de características**
	-  Las SVM son sensibles a la escala de las características, por lo que es importante escalar 
- **Clases balanceadas**
	- No es un supuesto estricto, pero es recomendado. Un desbalance significativo en las clases puede sesgar el modelo hacia la clase mayoritaria. 


--- 
## 8. Ejemplos de Aplicación

- [weiboanalysis](https://github.com/Zephery/weiboanalysis) es un proyecto que aplica SVM (junto con otros algoritmos) para el **Análisis de sentimientos** y **clasificación de textos**.
- [Speech-Emotion-Recognition](https://github.com/Renovamen/Speech-Emotion-Recognition) es un proyecto que utiliza SVM (entre otras técnicas) para el **reconocimiento de emociones en señales de voz**.
- [HablaImaginada-DeepLearning](https://github.com/EdgarMoyete/HablaImaginada-DeepLearning) propone una arquitectura que combina CNN y LSTM para la clasificación de señales EEG de habla imaginada. Aunque se centra en redes neuronales, también incluye implementaciones de SVM para comparación. 

---
## 9. Recursos Adicionales

- [IBM -SVM](https://www.ibm.com/mx-es/topics/support-vector-machine?utm_source=chatgpt.com) explicación detallada sobre qué es una SVM, tipos, funcionamiento y aplicaciones. 
-  [Aspectos matemáticos en Máquinas de Vectores Soporte (SVM)](https://uvadoc.uva.es/handle/10324/63431?utm_source=chatgpt.com) trabajo de fin de máster analiza detalladamente los aspectos matemáticos subyacentes a la metodología SVM. 
- [SVM Playground](https://aelbaza.github.io/SVMPlayground/?utm_source=chatgpt.com#dataset=circle&noise=10&seed=0.92236&showTestData=false&discretize=false&percTrainData=80&parameterC=11.8&polyDegree=2&gamma=0.5) un simulador interactivo que permite experimentar con SVM directamente en el navegador, ajustando parámetros como el tipo de kernel, el valor de C y el grado del polinomio.

---
## 10. Referencias

 1. Cano Lengua, Miguel Angel, y Erik Alex Papa Quiroz. «A Systematic Literature Review on Support Vector Machines Applied to Classification». En _2020 IEEE Engineering International Research Conference (EIRCON)_, 1-4. Lima, Peru: IEEE, 2020. [https://doi.org/10.1109/EIRCON51178.2020.9254028](https://doi.org/10.1109/EIRCON51178.2020.9254028).

2. Cortes, Corinna, y Vladimir Vapnik. «Support-Vector Networks». _Machine Learning_ 20, n.o 3 (septiembre de 1995): 273-97. [https://doi.org/10.1007/BF00994018](https://doi.org/10.1007/BF00994018).

3. Dabas, Ali. «Application of Support Vector Machines in Machine Learning». Preprints, 2 de agosto de 2024. [https://doi.org/10.36227/techrxiv.172263291.17505159/v1](https://doi.org/10.36227/techrxiv.172263291.17505159/v1).

4. Li, Hang. _Machine Learning Methods_. Singapore: Springer Nature Singapore, 2024. [https://doi.org/10.1007/978-981-99-3917-6](https://doi.org/10.1007/978-981-99-3917-6).