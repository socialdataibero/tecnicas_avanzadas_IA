---
title: Perceptrón_Multicapa
category:
  - 🧠 DL
subcategory:
  - None
tags:
  - Etiqueta1
  - Etiqueta2
  - Etiqueta3
status:
  - 🔵 En Progreso
date: 2024-11-12
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: Perceptrón_Multicapa

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
- [x] **Referencias**

---
## 1. Título del Algoritmo

### **Perceptrón multicapa**

---
## 2. Representación Gráfica del Algoritmo

![[perceptron_multicapa_icon.png]]

Referencia: <a href="https://www.flaticon.com/free-icons/neural-network" title="neural network icons">Neural network icons created by Freepik - Flaticon</a> 

---
## 3. Introducción al Algoritmo 

El **perceptrón multicapa** (MLP, por sus siglas en inglés) es una de las arquitecturas de [[Redes_Neuronales_Artificiales]] más utilizadas y populares dentro del aprendizaje profundo. Debe su nombre a su estructura basada en **múltiples capas** de neuronas, típicamente una **capa de entrada** , dos o más **capas ocultas** y una **capa de salida**. Los MLPs son capaces de modelar relaciones complejas y no lineales en los datos (a diferencia del [[Perceptron]] simple), lo que los convierte en herramientas poderosas en diversas tareas del aprendizaje automático, incluyendo, la regresión, la clasificación y  el reconocimiento de patrones. Aunque son modelos muy potentes y versátiles, estos pueden ser computacionalmente intensivos y propensos al sobreajuste (overfitting), lo que ha impulsado el desarrollo de arquitecturas más avanzadas *(Basha et al., 2023; Elansari et al., 2024; Shanthamallu et al., n.d.)*.

---
## 4. Bases Matemáticas del Algoritmo

Matemáticamente, un MLP procesa la información mediante una serie de transformaciones lineales y no lineales. Para cada capa $l$, la entrada se multiplica por una matriz de pesos $W^{(l)}$ y se le añade un vector de *bias*  $\mathbf{b}^{(l)}$, obteniendo así el vector:

$$
\mathbf{z}^{(l)} = W^{(l)} \mathbf{a}^{(l-1)} + \mathbf{b}^{(l)}
$$

donde $\mathbf{a}^{(l-1)}$ es la salida de la capa anterior. A continuación, se aplica una función de activación $\phi^{(l)}$ de manera elemento a elemento para introducir no linealidad, resultando en:

$$
\mathbf{a}^{(l)} = \phi^{(l)}(\mathbf{z}^{(l)})
$$

Este proceso se repite a lo largo de todas las capas ocultas hasta llegar a la capa de salida, donde la activación final representa la predicción del modelo:

$$
\hat{\mathbf{y}} = \mathbf{a}^{(L)}
$$

El entrenamiento del MLP se realiza mediante el algoritmo de **retropropagación**, que ajusta los pesos y sesgos minimizando una función de pérdida. Este ajuste se logra calculando los gradientes de la función de pérdida respecto a cada parámetro y actualizándolos utilizando métodos de optimización *(Basha et al., 2023; Elansari et al., 2024; Shanthamallu et al., n.d.)*.

### 4.1 Ilustración del funcionamiento 

![[perceptron_multicapa_des.png]]

**Referencia:** https://link.springer.com/article/10.1007/s10115-023-01959-7#citeas 

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

1. Basha, Niha Kamal;Bhatia Khan, Surbhi Bhatia Khan, y Abhishek KumarArwa Mashat. _Deep Learning and Its Applications Using Python_. _Urn:Isbn:9781394166466_. John Wiley & Sons, Incorporated, 2023.
2. Elansari, Taoufyq, Mohammed Ouanan, y Hamid Bourray. «A Novel Mathematical Modeling for Deep Multilayer Perceptron Optimization: Architecture Optimization and Activation Functions Selection». _Statistics, Optimization & Information Computing_ 12, n.o 5 (6 de junio de 2024): 1409-24. [https://doi.org/10.19139/soic-2310-5070-1990](https://doi.org/10.19139/soic-2310-5070-1990).
3. Shanthamallu, Uday Shankar, Andreas Spanias, Khalid Sayood, Kenichi Kanatani, Nasser Kehtarnavaz, Abhishek Sehgal, Shane Parris, y Arian Azarang. _Machine and Deep Learning Algorithms and Applications_, s. f.