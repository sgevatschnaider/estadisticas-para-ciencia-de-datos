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
|---|---|
| **Variables Aleatorias y Teoría de la Medida (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Cuaderno teórico en Python que traduce las intuiciones visuales a la formalidad matemática pura. Define rigurosamente la variable aleatoria como una función medible (pushforward), explora la descomposición de Lebesgue, transformaciones con Jacobiano, esperanza matemática y geometría en el espacio L2.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/87ab9a48374af5483e119978bfa60eb0bf0535bd/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/87ab9a48374af5483e119978bfa60eb0bf0535bd/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb) |

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Fase 1: Del Bit al Continuo (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo que demuestra la equivalencia fundamental entre tirar una moneda (bits) y construir un número real en el intervalo [0,1]. Rompe la intuición discreta y establece la base para entender cómo secuencias infinitas definen variables continuas, un concepto vital para PRNGs y transformadas inversas.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_moneda.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_moneda.html) |
| **Fase 2: Conjuntos Cilíndricos (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Herramienta visual que explica cómo fijar condiciones finitas iniciales crea "bloques" de volumen exacto (conjuntos cilíndricos) en el espacio continuo. Prepara la intuición para comprender las σ-álgebras y cómo se atrapan porciones de medida probabilística, simulando 10,000 secuencias en tiempo real.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_cilindros.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_cilindros.html) |
| **Fase 3: La Paradoja del Cero (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador que escala el problema del cumpleaños al infinito para ilustrar el colapso de la probabilidad puntual. Demuestra interactivamente que el hecho de que un evento continuo tenga probabilidad de cero (medida de Lebesgue nula) no significa que sea topológicamente imposible.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_paradoja_del_cero.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_paradoja_del_cero.html) |
| **Fase 4: Árbol Binario en Disco de Poincaré (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Representación avanzada que sitúa el espacio muestral de secuencias como un Grafo de Cayley incrustado en geometría hiperbólica. Ilustra visualmente cómo el espacio muestral continuo reside en el límite infinito (el polvo de Cantor), dándole una interpretación geométrica rigurosa al azar.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_poincare_tree.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_poincare_tree.html) |
| **Fase 5: Variables Aleatorias y Teoría de la Medida (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Cuaderno teórico en Python que traduce las intuiciones visuales a la formalidad matemática pura. Define rigurosamente la variable aleatoria como una función medible (pushforward), explora la descomposición de Lebesgue, transformaciones con Jacobiano, esperanza matemática y geometría en el espacio L2.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb) |
| **Fase 6: La Máquina de la Creación (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Aplicación práctica de toda la teoría anterior utilizando el Teorema de la Transformada Inversa. El simulador muestra cómo una distribución uniforme generada en [0,1] se mapea a través de la función probit para hacer emerger la Campana de Gauss en tiempo real.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_creation_machine.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_creation_machine.html) |
| **Fase 7: El Guardián de las Colas (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo sobre las desigualdades de concentración de Markov y Chebyshev. Permite explorar visualmente cómo acotar probabilidades en las colas sin conocer la distribución subyacente, y demuestra el concepto de cota ajustada mediante un caso límite con distribuciones mixtas (Spike).</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Chebyshev_Markov.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Chebyshev_Markov.html) |
| **Fase 8: La Fábrica de Átomos (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Laboratorio visual que explica la diferencia fundamental entre censurar y truncar datos. Muestra cómo colapsar valores extremos crea masas puntuales ("átomos") en distribuciones continuas, ilustrando intuitivamente la necesidad matemática de la Teoría de la Medida de Lebesgue.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Fabrica_de_atomos.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Fabrica_de_atomos.html) |
| **Fase 9: El Juego de las Monedas Infinitas (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador avanzado que contrasta las integrales de Riemann y Lebesgue. A través de la Función de Dirichlet y la construcción de Conjuntos Cilíndricos mediante lanzamientos de moneda, demuestra cómo Lebesgue agrupa por preimagen para unificar el concepto de Esperanza Matemática.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_lebesgue_monedas.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_lebesgue_monedas.html) |

---
## 🎥 Material Audiovisual Complementario (The Video Lectures)

Para consolidar la intuición geométrica y las demostraciones formales de los simuladores, esta es la curaduría definitiva de clases en video. Ideal para repasar conceptos complejos de topología, teoría de la medida y econometría aplicados a la ciencia de datos.

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Teoría de la Medida e Integral de Lebesgue**<br><sub>*Complemento visual para entender por qué la integración de Riemann falla en el continuo y cómo Lebesgue agrupa por preimagen.*</sub> | **Cofiber**<br><sub>*Understanding Measure Theory...*</sub><br><br>**The Bright Side of Mathematics**<br><sub>*Measure Theory (Curso Completo)*</sub> | [Ver Video](https://www.youtube.com/watch?gHUZFXvy4yE) <br><br> [Ver Playlist](https://www.youtube.com/playlist?list=PLBh2i93oe2qvMVqAzsX1Kuv6-4fjazZ8j) |
| **Desigualdades de Concentración**<br><sub>*La demostración rigurosa de Markov y Chebyshev, fundamental para entender las cotas de error en algoritmos.*</sub> | **Steve Brunton**<br><sub>*Chebyshev's Inequality in Probability*</sub><br><br>**MIT OpenCourseWare**<br><sub>*Prof. John Tsitsiklis (Lecture 20)*</sub> | [Ver Video](https://www.youtube.com/watch?v=otCHN3s52ho) <br><br> [Ver Video](https://www.youtube.com/watch?v=nrDkb2MAwSA) |
| **Método de la Transformada Inversa**<br><sub>*La matemática detrás de la simulación de variables aleatorias usando la función cuantil ($F^{-1}$).*</sub> | **Ben Lambert**<br><sub>*An introduction to inverse transform...*</sub><br><br>**ritvikmath**<br><sub>*Inverse Transform Sampling*</sub> | [Ver Video](https://www.youtube.com/watch?v=rnBbYsysPaU) <br><br> [Ver Video](https://www.youtube.com/watch?v=9ixzzPQWuAY) |
| **Topología del Continuo y Medida Cero**<br><sub>*Paradojas del espacio muestral continuo, mapeos infinitos y por qué probabilidad 0 $\neq$ imposible.*</sub> | **3Blue1Brown**<br><sub>*Probabilities of continuous spaces*</sub><br><br>**Vsauce**<br><sub>*How To Count Past Infinity*</sub> | [Ver Video](https://www.youtube.com/watch?v=ZA4JkHKZM50) <br><br> [Ver Video](https://www.youtube.com/watch?v=SrU9YDoXE88) |
| **Censura vs. Truncamiento (Econometría)**<br><sub>*Entendiendo la formación de átomos (masas puntuales) en las colas, esencial para los Modelos Tobit.*</sub> | **Anders Munk-Nielsen**<br><sub>*The Tobit Model*</sub><br><br>**Jake Clifton / Ben Lambert**<br><sub>*Econometrics II (Playlist)*</sub> | [Ver Video](https://www.youtube.com/watch?v=IwsE8Rr6l6E) <br><br> [Ver Playlist](https://www.youtube.com/playlist?list=PLLZ4uVeiDmR_rzu-uYl9A5BrmvTKtH_aB) |

---

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

