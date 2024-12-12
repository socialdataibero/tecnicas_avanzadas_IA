---
title: K-means
category:
  - 🤖 ML
subcategory:
  - No supervisado
  - Clustering
tags:
  - Etiqueta1
  - Etiqueta2
  - Etiqueta3
status:
  - 🔵 En Progreso
date: 2003-12-02
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: K-means

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

### **K-means**

---
## 2. Representación Gráfica del Algoritmo

![[k_means_icon.png]]

Referencia: https://holypython.com/k-means/k-means-history/

---
## 3. Introducción al Algoritmo 

**K-means** es un algoritmo fundamental de aprendizaje automático no supervisado utilizado para agrupar datos en conjuntos distintos basados en similitudes de características. El objetivo principal es particionar un conjunto de datos en k clústeres predefinidos, donde cada punto de datos pertenece al clúster con la media más cercana, que actúa como el *centróide* del clúster.

Aspectos clave de K-means incluyen su eficiencia computacional, lo que lo hace adecuado para conjuntos de datos grandes, y su simplicidad en la implementación. Sin embargo, presenta limitaciones como la necesidad de especificar el número de clústeres (k) por adelantado y la sensibilidad a la ubicación inicial de los centróides, lo que puede afectar el resultado final del agrupamiento. Además, K-means asume que los clústeres son esféricos y de tamaño igual, lo que puede no ser válido para todos los conjuntos de datos.

K-means se aplica ampliamente en diversos dominios, incluyendo segmentación de clientes, compresión de imágenes y reconocimiento de patrones, debido a su capacidad para descubrir estructuras inherentes dentro de los datos. A pesar de su simplicidad, una consideración cuidadosa de los métodos de inicialización y los pasos de preprocesamiento, como el escalado de características, puede mejorar significativamente su rendimiento y fiabilidad.

---
## 4. Bases Matemáticas del Algoritmo

Las bases matemáticas del algoritmo K-means se centran en la partición óptima de un conjunto de datos en **k** clústeres, minimizando la variabilidad intra-clúster. El objetivo principal es minimizar la **suma de las distancias cuadráticas** entre los puntos de datos y sus respectivos centróides. Esto se expresa mediante la función objetivo:

$$
J = \sum_{i=1}^{k} \sum_{x \in C_i} \|x - \mu_i\|^2
$$

donde:

- $k$ es el número de clústeres.
- $C_i$ es el conjunto de puntos asignados al clúster $i$.
- $\mu_i$ es el centróide del clúster $i$.
- $\|x - \mu_i\|$ representa la distancia Euclidiana entre el punto $x$ y el centróide $\mu_i$.

El algoritmo K-means sigue un enfoque iterativo conocido como **algoritmo de Lloyd**:

1. **Inicialización**: Selección de $k$ centróides iniciales, a menudo de forma aleatoria.
2. **Asignación**: Cada punto $x$ se asigna al clúster cuyo centróide $\mu_i$ minimiza $\|x - \mu_i\|^2$.
3. **Actualización**: Recalcular cada centróide $\mu_i$ como la media de todos los puntos asignados al clúster $i$:

   $$
   \mu_i = \frac{1}{|C_i|} \sum_{x \in C_i} x
   $$

4. **Convergencia**: Repetir los pasos de asignación y actualización hasta que los centróides ya no cambien significativamente o se alcance un número máximo de iteraciones.

Matemáticamente, K-means busca una solución de optimización no convexa, por lo que puede converger a un mínimo local dependiendo de la inicialización. La elección de la métrica de distancia y la normalización de los datos también son aspectos cruciales que afectan el rendimiento y la exactitud del algoritmo.


### 4.1 Ilustración del funcionamiento (*Opcional*)

![[k_means_des.png]]

**Referencia:** https://www.analyticsvidhya.com/blog/2020/10/a-simple-explanation-of-k-means-clustering/

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