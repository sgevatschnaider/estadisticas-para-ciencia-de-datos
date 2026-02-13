# MÓDULO I: Probabilidad Multivariante y Geometría de Datos

<p align="center">
  <img src="../../../assets/portada_probabilidad.gif" alt="Visualización: Covarianza y Elipsoides" width="100%">
  <br>
  <sub style="font-size: 14px;">
    <b>Álgebra Lineal Aleatoria</b> &nbsp;|&nbsp;
    <b>Normal Multivariante (MVN)</b> &nbsp;|&nbsp;
    <b>Concentración de la Medida</b>
  </sub>
</p>

---

## 🎯 Objetivos de Aprendizaje (Engineering Track)

Al completar este módulo, dejarás de ver la probabilidad como "lanzar dados" y pasarás a verla como **geometría en alta dimensión**. Podrás:

- **Geometrica de Datos:** Entender la correlación como el coseno del ángulo entre vectores aleatorios (Espacios de Hilbert).
- **Ingeniería de la MVN:** Dominar la **Normal Multivariante**, la distribución más importante en Machine Learning y Filtros de Kalman.
- **Pre-procesamiento:** Implementar **Whitening (Blanqueo)** y PCA desde cero usando descomposición espectral ($\Sigma = U\Lambda U^T$).
- **Detección de Anomalías:** Utilizar la **Distancia de Mahalanobis** para encontrar outliers en dimensiones $d > 3$.
- **Garantías Teóricas:** Aplicar desigualdades de concentración (**Chebyshev, Hoeffding**) para acotar errores en algoritmos de aprendizaje.

---

## 🛠️ Stack Tecnológico

Requisitos para este módulo:

- **Core:** `numpy` (álgebra lineal), `scipy.stats` (distribuciones).
- **Visualización:** `matplotlib`, `seaborn` (estática), `plotly` (interactiva 3D).
- **Simulación:** `statsmodels` (opcional).

```bash
# Instalación del entorno
pip install numpy scipy matplotlib seaborn plotly pandas

```

---

## 🧪 Laboratorio Interactivo (Notebooks & Apps)

Esta sección contiene los recursos principales. Los **Notebooks** combinan teoría dura (Wasserman/Kenett) con código, y las **Apps HTML** son simuladores visuales standalone.

| 📄 Recurso | 📥 Acceso |
| --- | --- |
| **01. La Geometría de la Aleatoriedad** <br>

<br>

<br> <details><summary><strong>Resumen:</strong> <em>(clic para expandir)</em></summary><p>Basado en <strong>Wasserman (Cap. 3)</strong>. Dejamos atrás la probabilidad básica para entrar en el álgebra lineal. Visualizamos las variables aleatorias como vectores. Definimos la covarianza como un producto interno y la correlación como un ángulo. Incluye simulaciones de cómo la matriz de covarianza  deforma el espacio.</p></details> | [](https://www.google.com/search?q=./01_Geometria_de_la_Aleatoriedad.ipynb) [](https://www.google.com/search?q=https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/01_Geometria_de_la_Aleatoriedad.ipynb) |
| **02. La Normal Multivariante (MVN) y Whitening** <br>

<br>

<br> <details><summary><strong>Resumen:</strong> <em>(clic para expandir)</em></summary><p>El corazón del módulo. Estudiamos la densidad  de la MVN, sus isocontornos elípticos y la descomposición espectral. Implementamos el proceso de <strong>"Whitening"</strong> (decorrelación + estandarización) fundamental para el Deep Learning. Referencia cruzada con <strong>Kenett (Modern Statistics)</strong> para la implementación computacional.</p></details> | [](https://www.google.com/search?q=./02_Normal_Multivariante_y_Whitening.ipynb) [](https://www.google.com/search?q=https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/02_Normal_Multivariante_y_Whitening.ipynb) |
| **APP HTML: Simulador de Elipsoides de Confianza** <br>

<br>

<br> <details><summary><strong>Resumen:</strong> <em>(clic para expandir)</em></summary><p>Visualización web interactiva (D3.js/Plotly). Permite manipular los valores de la matriz de covarianza  en tiempo real y observar cómo rota y se estira la nube de puntos 3D. Visualiza planos de corte y distancias de Mahalanobis interactivas.</p></details> | [](https://www.google.com/search?q=./apps/simulador_mvn.html) |
| **03. Concentración de la Medida (Teoría del Aprendizaje)** <br>

<br>

<br> <details><summary><strong>Resumen:</strong> <em>(clic para expandir)</em></summary><p>¿Por qué funciona el Machine Learning? Basado en <strong>Wasserman (Cap. 4 y 5)</strong>. Exploramos la Ley de los Grandes Números y, más importante, las cotas de error no asintóticas (Desigualdades de Hoeffding y Mill). Simulamos "la carrera de la convergencia" para ver cuán rápido convergen los estimadores en la práctica.</p></details> | [](https://www.google.com/search?q=./03_Concentracion_de_la_Medida.ipynb) [](https://www.google.com/search?q=https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/03_Concentracion_de_la_Medida.ipynb) |

---

## 📐 Fundamentos Teóricos (The Canon)

### 1. Vector de Medias y Matriz de Covarianza

Dada una variable aleatoria vectorial :

> **Intuición Ingenieril:**  contiene la información de la "forma" de los datos. Si  (Identidad), los datos son una esfera perfecta (ruido blanco isotrópico).

### 2. Distancia de Mahalanobis

La distancia euclidiana miente en altas dimensiones si las variables están correlacionadas. Usamos la métrica natural de la distribución:

Esta distancia es **invariante a escalas y rotaciones**. En el notebook 02 veremos cómo usarla para detectar anomalías bancarias o de sensores.

---

## 💻 Snippets de Código Esenciales

### Generación de Datos MVN y Rotación (Python)

```python
import numpy as np
import matplotlib.pyplot as plt

# 1. Definir parámetros
mu = [0, 0]
sigma = [[1, 0.8], 
         [0.8, 1]]  # Alta correlación positiva

# 2. Muestreo (Ingeniería Inversa: Cholesky)
n = 1000
L = np.linalg.cholesky(sigma) # Descomposición de Cholesky
z = np.random.normal(size=(n, 2)) # Ruido blanco no correlacionado
x = z @ L.T + mu # Transformación afín: colorear el ruido

# 3. Visualización rápida
plt.scatter(x[:,0], x[:,1], alpha=0.5)
plt.title(f"MVN con correlación {sigma[0][1]}")
plt.axis('equal')
plt.show()

```

---

## 📚 Bibliografía Específica del Módulo

Este módulo se construye sobre los siguientes textos canónicos (disponibles en la carpeta de referencias):

1. **[Wasserman]** *All of Statistics*
* *Capítulo 3:* Random Vectors (Base geométrica).
* *Capítulo 4:* Convergence (Fundamento del aprendizaje).
* *Capítulo 14:* Multivariate Models (La teoría de la MVN).


2. **[Kenett & Zacks]** *Modern Statistics: A Computer-Based Approach*
* *Capítulo 2:* Data Visualization (Enfoque computacional).


3. **[Rotondi]** *Probability, Statistics and Simulation*
* *Capítulo 4:* Simulation of Random Variables (Métodos de Monte Carlo).



---

## 🗺️ Roadmap del Módulo

1. **Semana 1:** Vectores aleatorios, matrices de covarianza y visualización de correlaciones.
2. **Semana 2:** La Normal Multivariante a fondo. Diagonalización y PCA.
3. **Semana 3:** Desigualdades y límites. ¿Cuántos datos necesito? (Hoeffding).
4. **Proyecto Final:** Detector de anomalías basado en Mahalanobis sobre dataset real.

---

## ⚠️ Errores Comunes (Troubleshooting)

* **Matriz Singular:** Si `np.linalg.inv(Sigma)` falla, tu matriz de covarianza no es invertible (tienes variables colineales). *Solución:* Usar `np.linalg.pinv` (pseudoinversa).
* **Maldición de la Dimensionalidad:** En alta dimensión, casi todos los puntos parecen "lejanos" (concentración en la corteza). No confíes en la intuición 2D/3D ciegamente.
* **Interpretación de Correlación:**  implica independencia **solo** si la distribución es Gaussiana. En otros casos, puede haber dependencia no lineal.

```

### 💡 Mejoras aplicadas respecto al modelo de Grafos:

1.  **Enfoque Matemático/Visual:** He reemplazado los grafos por conceptos de geometría lineal (matrices, elipsoides), que es la base de este módulo.
2.  **Interacción "Dropdown":** He mantenido las etiquetas `<details>` y `<summary>` para que el README se vea limpio, pero puedas desplegar la descripción teórica de cada notebook.
3.  **Enlaces a Colab:** He dejado las rutas preparadas (`.../blob/main/src/classroom/probabilidad/...`). Cuando subas los archivos `.ipynb` a esas carpetas, los botones funcionarán automáticamente.
4.  **Sección "Snippet":** Agregué un ejemplo de código real usando descomposición de Cholesky, que demuestra "Saber hacer" (Ingeniería) sobre solo teoría.

```
