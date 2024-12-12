---
title: Arboles_Decision
category:
  - 🤖 ML
subcategory:
  - Supervisado
  - Clasificacion
  - Regresion
tags:
  - Etiqueta1
  - Etiqueta2
  - Etiqueta3
status:
  - 🔵 En Progreso
date: 2003-12-31
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: Arboles_Decision

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

### **Árboles de Decisión**

---
## 2. Representación Gráfica del Algoritmo

![[decision_tree_icon.png]]
*Referencia:* <a href="https://www.flaticon.com/free-icons/decision-tree" title="decision tree icons">Decision tree icons created by Freepik - Flaticon</a> 

---
## 3. Introducción al Algoritmo 

Los **árboles de decisión** son uno de los métodos más populares del *machine learning* para construir modelos de **regresión** y **clasificación** a través de algoritmos estructurados jerárquicamente de tipo árbol. El funcionamiento de estas técnicas se basa modelar decisiones y sus posibles consecuencias como una estructura de árbol, donde cada nodo interno representa una decisión basada en una característica específica (evaluación condicional), cada rama denota el resultado de esa decisión, y cada nodo hoja corresponde a una predicción final o etiqueta de clase. El proceso comienza en el nodo raíz y recorre el árbol tomando decisiones en cada nodo hasta llegar a una hoja *(Asst. Professor, Department of Computer Science, King Khalid University, Abha, Kingdom of Saudi Arabia. et al., 2023; Li, 2024)*.

Una de las principales ventajas de los árboles de decisión es su simplicidad e interpretabilidad, además de manejar datos tanto numéricos como categóricos y de requerir un preprocesamiento mínimo de los datos. Sin embargo, una de sus desventajas más importantes es su propensión al sobreajuste, (especialmente con árboles complejos), lo que puede reducir su capacidad de generalización en datos no vistos. Ante esto, existen técnicas como la poda, establecer una profundidad máxima del árbol y métodos de ensamblaje como Random Forests y Gradient Boosting suelen emplearse para mejorar su robustez y precisión *(Rodionov & Mukhitdinova, 2023; Shanthamallu et al., n.d.)*.

---
## 4. Bases Matemáticas del Algoritmo

Los árboles de decisión se construyen mediante la partición recursiva del espacio de características para modelar decisiones y resultados. Matemáticamente, el proceso comienza seleccionando la mejor característica y umbral para dividir los datos en cada nodo, optimizando un criterio como:

- **Entropía** para clasificación:
  $$
  H(S) = -\sum_{i} p_i \log p_i
  $$
- **Ganancia de información**:
  $$
  IG(S, A) = H(S) - \sum_{v} \frac{|S_v|}{|S|} H(S_v)
  $$
- **Impureza de Gini**:
  $$
  G(S) = 1 - \sum_{i} p_i^2
  $$

Algoritmos más sofisticados como CART (*Árboles de Clasificación y Regresión*, por sus siglas en inglés) utilizan estas medidas para realizar divisiones binarias recursivas y voraces. El árbol crece minimizando la impureza en cada paso:
$$
\text{División} = \arg\min_{\text{característica, umbral}} \text{Impureza}
$$

Para prevenir el sobreajuste, se aplican técnicas de poda, a menudo minimizando una función de complejidad de costo:
$$
C(T) = C(T') + \alpha |T'|
$$
donde $C(T')$ es el error del subárbol $T'$ y $\alpha$ es un parámetro de regularización.

El modelo final equilibra el sesgo y la varianza, asegurando la generalización mediante la selección de una estructura óptima del árbol a través de métodos como la validación cruzada. 

Referencias: *(Adam et al., 2024; Li, 2024; Shanthamallu et al., n.d.)*
### 4.1 Ilustración del funcionamiento 

![[decision_trees_des.png]]

**Referencia:** https://www.analyticsvidhya.com/blog/2021/08/decision-tree-algorithm/ 

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

Adam, Timo, Marius Ötting, y Rouven Michels. «Markov-Switching Decision Trees». _AStA Advances in Statistical Analysis_ 108, n.o 2 (junio de 2024): 461-76. [https://doi.org/10.1007/s10182-024-00501-6](https://doi.org/10.1007/s10182-024-00501-6).

Asst. Professor, Department of Computer Science, King Khalid University, Abha, Kingdom of Saudi Arabia., Dr. Nirmla Sharma, Sameera Iqbal Muhmmad Iqbal, y Department of Computer Science, King Khalid University, Abha, Kingdom of Saudi Arabia. «Applying Decision Tree Algorithm Classification and Regression Tree (CART) Algorithm to Gini Techniques Binary Splits». _International Journal of Engineering and Advanced Technology_ 12, n.o 5 (30 de junio de 2023): 77-81. [https://doi.org/10.35940/ijeat.E4195.0612523](https://doi.org/10.35940/ijeat.E4195.0612523).

Li, Hang. _Machine Learning Methods_. Singapore: Springer Nature Singapore, 2024. [https://doi.org/10.1007/978-981-99-3917-6](https://doi.org/10.1007/978-981-99-3917-6).

Rodionov, Andrei, y Munavvarkhan Mukhitdinova. «THE ROLE OF A DECISION TREE AS A METHOD OF ARTIFICIAL INTELLIGENCE FOR THE ANALYSIS OF BIG DATA PROBLEMS». _Economics and Innovative Technologies_ 11, n.o 2 (28 de abril de 2023): 400-407. [https://doi.org/10.55439/EIT/vol11_iss2/i39](https://doi.org/10.55439/EIT/vol11_iss2/i39).

Shanthamallu, Uday Shankar, Andreas Spanias, Khalid Sayood, Kenichi Kanatani, Nasser Kehtarnavaz, Abhishek Sehgal, Shane Parris, y Arian Azarang. _Machine and Deep Learning Algorithms and Applications_, s. f.