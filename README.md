# Applied Statistics for Data Science (Engineering & Research Track)

<p align="center">
  <img src="assets/portada%20.gif" alt="Visualización de conceptos: Geometría de Datos, Inferencia, Learning, Modelos Estructurados y Grafos" width="100%">
  <br>
  <sub style="font-size: 14px;">
    🔵 <b>Geometría & MVN</b> (Mód. I) &nbsp;|&nbsp;
    🟢 <b>Inferencia Comp.</b> (Mód. II) &nbsp;|&nbsp;
    🟠 <b>Regularización & ML</b> (Mód. III)
    <br>
    🔴 <b>Causalidad & Tiempo</b> (Mód. IV) &nbsp;|&nbsp;
    🟣 <b>Grafos & Complejidad</b> (Mód. V)
  </sub>
</p>

---

## 📑 Tabla de Contenidos
1. [Accesos rápidos](#accesos-rápidos)
2. [Descripción](#-descripción)
3. [Bibliografía base](#-bibliografía-base)
4. [Propósito del curso](#-propósito-del-curso)
5. [Syllabus detallado](#️-syllabus-detallado)
6. [Cómo utilizar este material](#-cómo-utilizar-este-material-instalación-y-uso)
7. [Estructura del repositorio](#-estructura-del-repositorio-high-level)
8. [Uso y ejecución](#️-uso-y-ejecución)
9. [Requisitos y nivel esperado](#-requisitos-y-nivel-esperado)
10. [Contribuciones](#-contribuciones)
11. [Licencia](#️-licencia)

---

## 🔗 Accesos rápidos

> Acceso directo a las carpetas del repositorio con la teoría (simuladores HTML) y el código fuente (Notebooks).

<p align="center">
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad">
    <img src="https://img.shields.io/badge/MÓDULO_I-Geometría-0366d6?style=for-the-badge" alt="MÓDULO I">
  </a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/inferencia">
    <img src="https://img.shields.io/badge/MÓDULO_II-Inferencia-0366d6?style=for-the-badge" alt="MÓDULO II">
  </a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/learning">
    <img src="https://img.shields.io/badge/MÓDULO_III-Learning-0366d6?style=for-the-badge" alt="MÓDULO III">
  </a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/pgm">
    <img src="https://img.shields.io/badge/MÓDULO_IV-Estructurados-0366d6?style=for-the-badge" alt="MÓDULO IV">
  </a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/tiempo">
    <img src="https://img.shields.io/badge/MÓDULO_V-Grafos-0366d6?style=for-the-badge" alt="MÓDULO V">
  </a>
</p>

<p align="center">
  <a href="https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/" target="_blank" rel="noopener">
    <img alt="Live docs — GitHub Pages" src="https://img.shields.io/badge/Live%20docs-GitHub%20Pages-2b3137?style=for-the-badge&logo=github" />
  </a>
  &nbsp;
  <a href="https://mybinder.org/v2/gh/sgevatschnaider/estadisticas-para-ciencia-de-datos/main" target="_blank" rel="noopener">
    <img alt="Live demos — Binder" src="https://img.shields.io/badge/Live%20demos-Binder-f5a250?style=for-the-badge&logo=jupyter" />
  </a>
  &nbsp;
  <a href="https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/" target="_blank" rel="noopener">
    <img alt="Open in — Colab" src="https://img.shields.io/badge/Open%20in-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" />
  </a>
</p>

---

## 🎯 Descripción

Material docente de nivel **Ingeniería** para Ciencia de Datos.

El curso asume conocimientos previos de estadística clásica (por ejemplo: ANOVA y tests de hipótesis básicos) y se centra en la **caja blanca** de la ingeniería estadística moderna: inferencia computacional, geometría de los datos, regularización y modelos gráficos probabilísticos (PGMs), con extensión a causalidad y series temporales.

<p align="center">
  <a href="https://www.python.org/">
    <img alt="Python" src="https://img.shields.io/badge/python-3.10%2B-blue">
  </a>
  <a href="https://www.r-project.org/">
    <img alt="R" src="https://img.shields.io/badge/R-4.x-276DC3">
  </a>
  <a href="https://julialang.org/">
    <img alt="Julia" src="https://img.shields.io/badge/Julia-1.x-9558B2">
  </a>
  <a href="https://github.com/psf/black">
    <img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
  </a>
  <a href="LICENSE">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg">
  </a>
</p>

---

## 📚 Bibliografía Base

Las referencias bibliográficas del programa se organizan en dos capas:

1. **The Canon**: textos vertebrales del curso (conceptos, métodos y marco unificado).  
2. **Foundations / Backbone**: fundamentos matemáticos y multivariantes que sostienen el nivel “Engineering & Research Track”.

### The Canon (textos centrales)

- **[Wasserman]** — Larry Wasserman, *All of Statistics: A Concise Course in Statistical Inference*.  
- **[ESL]** — Trevor Hastie, Robert Tibshirani, Jerome Friedman, *The Elements of Statistical Learning: Data Mining, Inference, and Prediction*.  
- **[BDA3]** — Andrew Gelman, John B. Carlin, Hal S. Stern, David B. Dunson, Aki Vehtari, Donald B. Rubin, *Bayesian Data Analysis (3rd Ed.)*.  
- **[Efron]** — Bradley Efron, Trevor Hastie, *Computer Age Statistical Inference: Algorithms, Evidence, and Data Science*.  
- **[Bishop]** — Christopher M. Bishop, *Pattern Recognition and Machine Learning*.  
- **[KollerFriedman]** — Daphne Koller, Nir Friedman, *Probabilistic Graphical Models: Principles and Techniques*.  
- **[Pearl]** — Judea Pearl, *Causality: Models, Reasoning, and Inference*.  
- **[ShumwayStoffer]** — Robert H. Shumway, David S. Stoffer, *Time Series Analysis and Its Applications*.  

### Foundations / Mathematical Backbone (rigor y soporte formal)

Estas referencias sostienen resultados de convergencia, concentración, multivariante y geometría usados a lo largo del curso:

- **[AxlerMeasure]** — Sheldon Axler, *Measure, Integration & Real Analysis* (teoría de medida e integración).  
- **[Rosenthal]** — Jeffrey Seth Rosenthal, *A First Look at Rigorous Probability Theory (2nd Ed.)* (probabilidad rigurosa y herramientas asintóticas).  
- **[Mardia]** — K. V. Mardia, J. T. Kent, J. M. Bibby, *Multivariate Analysis: Probability and Mathematical Statistics* (MVN, Wishart, teoría multivariante clásica).  
- **[HardleSimarFengler]** — Wolfgang Karl Härdle, Léopold Simar, Matthias R. Fengler, *Applied Multivariate Statistical Analysis* (multivariante aplicado y métodos modernos).  
- **[Chikuse]** — Yasuko Chikuse, *Statistics on Special Manifolds* (Stiefel/Grassmann, estadística en variedades).  
- **[RotondiPedroniPievatolo]** — Alberto Rotondi, Paolo Pedroni, Antonio Pievatolo, *Probability, Statistics and Simulation: With Application Programs Written in R* (Monte Carlo y verificación computacional).  

### Lecturas complementarias (según profundidad y orientación)

- **[KenettZacksGedeck]** — Ron S. Kenett, Shelemyahu Zacks, Peter Gedeck, *Modern Statistics: A Computer-Based Approach with Python* (enfoque computacional aplicado).  

---

## 🎯 Propósito del curso

Conectar **probabilidad multivariante + álgebra lineal + inferencia computacional** con la **geometría de los datos** usada hoy en **ML/IA**: reducción de dimensión, regularización, modelos estructurados, grafos y métodos de simulación/optimización.

---

## 🗺️ Syllabus detallado

## MÓDULO I — Vectores Aleatorios y Geometría de Datos

> **Enfoque:** la distribución conjunta como objeto geométrico (subespacios, elipsoides, proyecciones) y la concentración de la medida.

### 📂 Ruta del módulo y Recursos

| Recurso | Enlace al Repositorio |
| :--- | :--- |
| **💻 Código Fuente** | [Ir a carpeta `src/classroom/probabilidad`](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad) |

### 🗺️ Temario Detallado

#### 1. Notación matricial y geometría (μ, Σ)
- **Definiciones:** vector de medias μ = E[X] y matriz de covarianza Σ = E[(X − μ)(X − μ)ᵀ].  
- **Propiedades:** simetría, semidefinida positiva e interpretación geométrica (varianza por direcciones).  
- **Proyecciones:** varianza de uᵀX y métrica inducida.  
- **Aplicación:** feature scaling, covariance shift, distancia de Mahalanobis.

#### 2. Dependencia lineal vs. independencia estadística
- **Conceptos:** diferencia entre dependencia lineal (rango, singularidad) e independencia estadística (p(x,y) = p(x)p(y)).  
- **La falacia de la correlación:** correlación ≠ independencia (excepto en distribuciones gaussianas).  
- **Aplicación:** multicolinealidad en regresión, selección de variables.

#### 3. Normal multivariante (MVN)
- **Definición:** densidad y forma cuadrática.  
- **Geometría:** elipsoides de densidad y descomposición espectral: Σ = UΛUᵀ.  
- **Whitening (blanqueo):** Z = Λ^(−1/2) Uᵀ (X − μ) para decorrelacionar datos.  
- **Aplicación:** PCA, Gaussian Processes, Batch Normalization.

#### 4. Teoría del aprendizaje (concentración de la medida)
- **Convergencia:** LLN y CLT como convergencia estocástica y aproximación gaussiana.  
- **Desigualdades:** Chebyshev (cota por varianza) y Hoeffding (cota exponencial para variables acotadas).  
- **Aplicación:** cotas de generalización, intervalos de confianza para métricas.

### 📚 Bibliografía Específica — Módulo I

El módulo se apoya en textos de probabilidad rigurosa, teoría multivariante y fundamentos geométricos del aprendizaje estadístico.

**Wasserman — *All of Statistics***
- Chapter 3: Expectation and Variance  
- Chapter 4–5: Convergence of Random Variables and Inequalities  
- Chapter 14: Multivariate Models  

**Rosenthal — *A First Look at Rigorous Probability Theory***
- Secciones sobre modos de convergencia y resultados LLN/CLT  
- Secciones sobre desigualdades y herramientas asintóticas  

**Mardia, Kent & Bibby — *Multivariate Analysis***
- Normal multivariante y propiedades geométricas  
- Wishart y modelos multivariantes clásicos  

**Härdle, Simar & Fengler — *Applied Multivariate Statistical Analysis***
- PCA y reducción de dimensión  
- Métodos multivariantes aplicados y geometría de datos  

**Hastie, Tibshirani & Friedman — *The Elements of Statistical Learning***
- Chapter 2.4–2.5: Statistical Decision Theory  
- Chapter 3.5: Dimensionality Reduction  
- Secciones sobre bias–variance tradeoff  

**Koller & Friedman — *Probabilistic Graphical Models***
- Chapter 2–3: Conditional Independence and Factorization  

**Chikuse — *Statistics on Special Manifolds* (opcional / Research Track)**
- Stiefel y Grassmann manifolds  
- Marco geométrico para extender modelos más allá de lo euclídeo  

---

## MÓDULO II — Inferencia computacional y moderna

> **Enfoque:** superar límites de tests clásicos mediante optimización y simulación.

#### 5. Teoría asintótica y máxima verosimilitud (MLE)
- MLE como problema de optimización (gradiente y Hessiano; estimación numérica).  
- Consistencia, eficiencia, información de Fisher y cota de Cramér–Rao.  
- **Aplicación en DS/ML:** regresión logística (cross-entropy), entrenamiento de modelos probabilísticos (Naive Bayes, HMM).  
- **Bibliografía:** **[Wasserman, Ch. 9]**, **[Efron & Hastie, Ch. 2]**.

#### 6. Bootstrap y métodos de resampling
- Estimación del error estándar sin fórmulas cerradas.  
- Bootstrap paramétrico vs. no paramétrico; intervalos BCa.  
- **Aplicación en DS/ML:** incertidumbre en métricas (F1, AUC), bagging (Random Forest), stability selection.  
- **Bibliografía:** **[Wasserman, Ch. 8]**, **[Efron & Hastie, Ch. 10–11]**.

#### 7. Tests de hipótesis en alta dimensionalidad
- Tests de Wald, Score y Likelihood Ratio Test (LRT).  
- Comparaciones múltiples: Bonferroni y FDR (Benjamini–Hochberg).  
- **Aplicación en DS/ML:** A/B testing a escala, selección de features en alta dimensión (genómica, texto).  
- **Bibliografía:** **[Wasserman, Ch. 10]**, **[Efron & Hastie, Ch. 15]**, **[ESL (capítulos de alta dimensión)]**.

---

## MÓDULO III — Aprendizaje estadístico (regresión avanzada)

> **Enfoque:** trade-off sesgo–varianza, geometría de proyecciones y selección de modelos.

#### 8. Geometría de mínimos cuadrados (OLS)
- Regresión como proyección ortogonal; matriz sombrero H.  
- Teorema de Gauss–Markov y diagnóstico (leverage, distancia de Cook).  
- **Aplicación en DS/ML:** baselines interpretables, detección de puntos influyentes en producción.  
- **Bibliografía:** **[ESL, Ch. 3.2]**, **[Wasserman, Ch. 13]**.

#### 9. Regularización y selección de modelos
- Maldición de la dimensionalidad y sobreajuste.  
- Ridge (L2): contracción y conexión con priors gaussianos.  
- Lasso (L1): sparsity y conexión con priors Laplace; Elastic Net.  
- Criterios de información: AIC y BIC; validación cruzada como alternativa práctica.  
- **Aplicación en DS/ML:** estabilidad en modelos, selección automática de variables, early stopping.  
- **Bibliografía:** **[ESL, Ch. 3.4 y Ch. 7]**, **[Efron & Hastie, Ch. 7 y 16]**.

#### 10. Modelos lineales generalizados (GLM)
- Familia exponencial y funciones de enlace (logística y Poisson).  
- Algoritmo IRLS (Iteratively Reweighted Least Squares).  
- **Aplicación en DS/ML:** clasificación calibrada, modelado de conteos/demanda.  
- **Bibliografía:** **[ESL, Ch. 4.4]**, **[Efron & Hastie, Ch. 8]**.

---

## MÓDULO IV — Modelos estructurados, causalidad y tiempo

> **Enfoque:** modelar dependencias complejas, inferencia bayesiana y dinámica.

#### 11. Probabilistic Graphical Models (PGMs)
- DAGs: factorización de la conjunta, independencia condicional y d-separation.  
- Plate notation para modelos jerárquicos.  
- **Aplicación en DS/ML:** Naive Bayes, HMMs, modelos jerárquicos.  
- **Bibliografía:** **[Koller & Friedman, Ch. 2–4]**, **[Bishop, Ch. 8]**.

#### 12. Inferencia causal
- Correlación vs. causalidad; intervenciones y operador do(·).  
- Confounders, colliders y criterio back-door.  
- **Aplicación en DS/ML:** A/B testing, uplift modeling, mitigación de sesgos.  
- **Bibliografía:** **[Pearl, Ch. 1–3]**, **[Wasserman, Ch. 16–17]**.

#### 13. Inferencia bayesiana y MCMC
- Priors conjugados vs. no informativos; posterior como actualización de creencias.  
- MCMC: Metropolis–Hastings y diagnóstico básico.  
- **Aplicación en DS/ML:** Bayesian logistic regression, Bayesian optimization, cuantificación de incertidumbre.  
- **Bibliografía:** **[BDA3, Ch. 1–3]**, **[Efron & Hastie, Ch. 13]**.

#### 14. Series temporales y modelos dinámicos
- Estacionariedad, autocorrelación y modelos ARIMA.  
- State Space Models (SSM) y filtro de Kalman.  
- **Aplicación en DS/ML:** forecasting (demanda, finanzas), tracking (IoT), comparación con RNNs.  
- **Bibliografía:** **[Shumway & Stoffer, Ch. 1–3 y 6]**, **[Bishop, Ch. 13]**.

---

## MÓDULO V — Geometría moderna: grafos, complejidad y búsqueda

> **Enfoque:** expandir la geometría más allá de lo euclídeo (grafos), dinámica local (autómatas) y optimización no convexa.

#### 15. Teoría de grafos para ciencia de datos
- Matrices de adyacencia, conectividad, caminos, BFS/DFS.  
- **Aplicación en DS/ML:** PageRank, comunidades, recomendadores, detección de fraude.  
- **Bibliografía:** **[Material de cátedra]**.

#### 16. Espectros de grafos y geometría (spectral graph theory)
- Espectro del Laplaciano; autovalores y autovectores.  
- **Aplicación en DS/ML:** spectral clustering, graph embeddings, fundamentos de GNNs.  
- **Bibliografía:** **[Material de cátedra]**, con referencias cruzadas a conceptos de espectro en **[ESL]** y **[Bishop]**.

#### 17. Modelos sobre grafos y unificación
- Markov blankets, MRF (Markov Random Fields) y factor graphs.  
- Inferencia aproximada (loopy belief propagation).  
- **Aplicación en DS/ML:** CRFs (secuencias), segmentación, denoising.  
- **Bibliografía:** **[Koller & Friedman]**, **[Bishop, Ch. 8]**.

#### 18. Algoritmos evolutivos y programación genética (GP)
- Optimización sin gradiente en paisajes no convexos.  
- GP: búsqueda en espacios de programas (symbolic regression).  
- **Aplicación en DS/ML:** AutoML, ecuaciones interpretables, neuroevolution.  
- **Bibliografía:** **[Material de cátedra: Evolutivos/GP]**.

#### 19. Autómatas celulares (CA) y dinámica local
- Reglas locales y emergencia global; dinámica en grillas.  
- **Aplicación en DS/ML:** simulación de propagación (epidemias, tráfico), modelos generativos discretos.  
- **Bibliografía:** **[Material de cátedra: Autómatas Celulares]**.

---

## 💻 Cómo utilizar este material (Instalación y Uso)

Tienes dos formas principales de consumir y ejecutar las clases de este repositorio.

### Opción A: En la nube (recomendado)
No necesitas instalar nada en tu computadora.

1. **Simuladores interactivos:** navega a los HTML desde las carpetas del repo o desde **GitHub Pages**.  
2. **Jupyter Notebooks:** usa los botones de **Binder** o **Colab** para abrir un entorno virtual y ejecutar el código celda por celda.

### Opción B: Ejecución local
Si prefieres tener los archivos en tu máquina:

1. Clona este repositorio:
   ```bash
   git clone https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git
   cd estadisticas-para-ciencia-de-datos
🧱 Estructura del repositorio (high-level)

docs/ — sitio GitHub Pages (material por módulo)

src/classroom/ — notebooks, scripts y prácticas por módulo

assets/ — imágenes, gifs y recursos visuales del curso

tests/ — tests (si aplica)

requirements.txt / pyproject.toml — dependencias

🛠️ Uso y ejecución
1) Clonar el repositorio
git clone https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git
cd estadisticas-para-ciencia-de-datos
2) Crear entorno e instalar dependencias (Python)
python -m venv .venv

# Activar entorno (Linux/macOS):
source .venv/bin/activate

# Activar entorno (Windows):
# .venv\Scripts\activate

pip install -U pip
pip install -r requirements.txt
3) Calidad de código (opcional, recomendado)
pre-commit install
pre-commit run --all-files
4) Ejecutar notebooks / prácticas

Si trabajas con Jupyter Lab:

jupyter lab

Si usas VSCode:

Abre la carpeta del repositorio y ejecuta los archivos .ipynb con la extensión de Jupyter.

✅ Requisitos y nivel esperado
Matemática

Probabilidad y estadística clásica (intervalos, tests básicos, ANOVA).

Álgebra lineal (vectores, matrices, autovalores/autovectores).

Programación

Python (lenguaje principal).

R / Julia como soporte opcional.

🤝 Contribuciones

Issues y Pull Requests son bienvenidos.

Si vas a proponer cambios grandes (estructura, syllabus o tooling), por favor abre primero un Issue describiendo el objetivo y el impacto.

⚖️ Licencia

Este material se distribuye bajo licencia MIT. Ver el archivo LICENSE
 para más detalles.

