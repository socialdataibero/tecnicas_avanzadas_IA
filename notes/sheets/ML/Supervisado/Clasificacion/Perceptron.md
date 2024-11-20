---
title: Perceptron
category:
  - 🤖 ML
subcategory:
  - Supervisado
  - Clasificacion
tags:
  - ML
  - Supervisado
  - Red_Neuronal
status:
  - ✅ Completado
date: 2024-11-08
asigned_to:
  - "[[Armando]]"
---
--- 
# 📝 Ficha Técnica: Perceptron

## ✅ Estado de Compleción
- [x] **Título del algoritmo**
- [x] **Representación gráfica del algoritmo**
- [x] **Introducción al algoritmo y su relevancia**
- [x] **Bases Matemáticas del Algoritmo**
- [x] **Código de ejemplo en Python**
- [x] **Descripción de los tipos de datos aplicables**
- [x] **Supuestos de los datos**
- [x] **Ejemplos de aplicación práctica**
- [x] **Enlaces a recursos adicionales para profundizar en el tema**
- [x] **Referencias**

---
## 1. Título del Algoritmo

### **Perceptrón**

---
## 2. Representación Gráfica del Algoritmo

![[perceptron_icon.png]]

Referencia: <a href="https://www.flaticon.com/free-icons/perceptron" title="perceptron icons">Perceptron icons created by orvipixel - Flaticon</a>

---
## 3. Introducción al Algoritmo 

El **perceptrón** es uno de los modelos fundamentales en el campo de las [[Redes_Neuronales_Artificiales]], el cual fue introducido por Frank Rosenblatt en los años cincuentas en su famoso paper *(Rosenblatt, 1958)*. Esta estructura está inspirada en el funcionamiento de una neurona biológica, procesando entradas mediante pesos asignados y produciendo una **salida binaria**. Estructuralmente, consiste en una **única capa** de nodos (neurona o TLU) que aplican una función de activación, para clasificar datos en categorías distintas. Aunque su capacidad está limitada a resolver problemas **linealmente separables**, el perceptrón sentó las bases para el desarrollo de arquitecturas más complejas, como los perceptrones multicapa. A pesar de sus limitaciones, el perceptrón es una herramienta educativa e imprescindible en los recursos de enseñanza del aprendizaje automático y profundo *(Du et al., 2022; Li, 2024; Shanthamallu et al., n.d.)*.

---
## 4. Bases Matemáticas del Algoritmo

El **algoritmo del perceptrón** comienza inicializando el vector de pesos $\mathbf{w} = [w_1, w_2, \dots, w_n]$ y el término de sesgo $b$ (también conocido como *bias*) con valores aleatorios. Para cada muestra de entrenamiento con el vector de entrada de características $\mathbf{x} = [x_1, x_2, \dots, x_n]$ y la salida deseada $d$, el algoritmo calcula una suma ponderada $z$ como:

$$
z (\mathbf{x}) = \mathbf{w} \cdot \mathbf{x} + b = \sum_{i=1}^{n} w_i x_i + b
$$

Esta suma se pasa a través de la función de activación $a = a(z)$ para producir la salida predicha $\hat{y}$. Típicamente, la función de activación usada es la **función escalón unitaria**:

$$
\hat{y} = a(z) =
\begin{cases}
1 & \text{si } z > 0 \\
0 & \text{si} \; z \leq 0
\end{cases}
$$

El error se calcula restando la salida predicha de la salida deseada:

$$
\text{Error} = d - \hat{y}
$$

Para minimizar este error, los pesos y el sesgo se actualizan utilizando la tasa de aprendizaje $\eta$:

$$
w_i \leftarrow w_i + \eta \times \text{Error} \times x_i \quad \forall i = 1, 2, \dots, n
$$

$$
b \leftarrow b + \eta \times \text{Error}
$$

Este proceso se repite iterativamente para cada ejemplo de entrenamiento y a lo largo de múltiples épocas hasta que los pesos converjan (es decir, el error sea mínimo) o se alcance un número predefinido de iteraciones. A través de estas actualizaciones, el perceptrón ajusta su línea de decisión para clasificar mejor los datos de entrada *(Du et al., 2022; Li, 2024; Shanthamallu et al., n.d.)*.

### 4.1 Ilustración del funcionamiento (*Opcional*)

![[perceptron_des.png]]

**Referencia:** Imagen tomada de *(Shanthamallu et al., n.d.)*

---
## 5. Código de Ejemplo en Python

Se puede acceder al ejemplo práctico básico de implementación en:

[Clasificador de imágenes](C:\Users\arhui\Documents\projects\TAIA\src\basic_code\Perceptron.ipynb)

---
## 6.  Tipos de Datos

- Esencialmente cualquier tipo de dato siempre que exista una **representación numérica**, ya sea continua o discreta.  

---
## 7.  Supuestos de los datos

- **Separabilidad lineal**
	-  Debe existir un hiperplano que pueda separar perfectamente las dos clases. 
- **Input numérico**
	-  Las características de entrada $x_i$ deben ser numéricas. 

--- 
## 8. Ejemplos de Aplicación

- **Clasificación de Spam en correos electrónicos**: 
	- El perceptrón puede clasificar mensajes como "spam" o "no spam" analizando características como palabras clave, remitente y frecuencia de ciertos términos.
- **Clasificación de imágenes médicas básico**:
	- Ayuda a distinguir entre imágenes de tejidos sanos y anómalos, facilitando el diagnóstico temprano de enfermedades.
---
## 9. Recursos Adicionales

- [Guía completa del perceptrón](https://pabloinsente.github.io/the-perceptron)
- [Simulador de redes neuronales](https://playground.tensorflow.org/#activation=sigmoid&batchSize=7&dataset=gauss&regDataset=reg-plane&learningRate=0.003&regularizationRate=0&noise=25&networkShape=1,2&seed=0.14476&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false) 
	- Puede ser utilizado para simular un perceptrón.
---
## 10. Referencias

1. Du, Ke-Lin, Chi-Sing Leung, Wai Ho Mow, y M. N. S. Swamy. «Perceptron: Learning, Generalization, Model Selection, Fault Tolerance, and Role in the Deep Learning Era». _Mathematics_ 10, n.o 24 (13 de diciembre de 2022): 4730. [https://doi.org/10.3390/math10244730](https://doi.org/10.3390/math10244730).
2. Li, Hang. _Machine Learning Methods_. Singapore: Springer Nature Singapore, 2024. [https://doi.org/10.1007/978-981-99-3917-6](https://doi.org/10.1007/978-981-99-3917-6).
3. Rosenblatt, F. «The Perceptron: A Probabilistic Model for Information Storage and Organization in the Brain.» _Psychological Review_ 65, n.o 6 (1958): 386-408. [https://doi.org/10.1037/h0042519](https://doi.org/10.1037/h0042519).
4. Shanthamallu, Uday Shankar, Andreas Spanias, Khalid Sayood, Kenichi Kanatani, Nasser Kehtarnavaz, Abhishek Sehgal, Shane Parris, y Arian Azarang. _Machine and Deep Learning Algorithms and Applications_, s. f.