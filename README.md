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
1. [Accesos rápidos](#-accesos-rápidos)
2. [Descripción](#-descripción)
3. [Bibliografía](#-bibliografía-base-the-canon)
4. [Syllabus](#-syllabus-detallado)
5. [Instalación y Uso](#-uso-y-ejecución)

---

## 🔗 Accesos rápidos

### ✅ Páginas del curso (Documentación Web)
> *Acceso a la teoría y notas de clase renderizadas en HTML.*

### ✅ Páginas del curso (Documentación Web)
> *Acceso a la teoría y notas de clase renderizadas en HTML.*

[![MÓDULO I — Geometría](https://img.shields.io/badge/M%C3%93DULO%20I-geometría-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/docs/modulos/probabilidad.html)
[![MÓDULO II — Inferencia](https://img.shields.io/badge/M%C3%93DULO%20II-inferencia-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/docs/modulos/inferencia.html)
[![MÓDULO III — Learning](https://img.shields.io/badge/M%C3%93DULO%20III-learning-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/docs/modulos/learning.html)
[![MÓDULO IV — Estructurados](https://img.shields.io/badge/M%C3%93DULO%20IV-estructurados-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/docs/modulos/pgm.html)
[![MÓDULO V — Grafos](https://img.shields.io/badge/M%C3%93DULO%20V-grafos-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/docs/modulos/tiempo.html)

### 🧩 Código del curso (Notebooks y Scripts)
> *Acceso directo al código fuente en el repositorio.*

[![src/classroom/geometria](https://img.shields.io/badge/src-geometria-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad)
[![src/classroom/inferencia](https://img.shields.io/badge/src-inferencia-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/inferencia)
[![src/classroom/learning](https://img.shields.io/badge/src-learning-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/learning)
[![src/classroom/estructurados](https://img.shields.io/badge/src-estructurados-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/pgm)
[![src/classroom/grafos](https://img.shields.io/badge/src-grafos-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/tiempo)

<p align="center">
  <a href="https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/" target="_blank" rel="noopener">
    <img alt="Live docs — GitHub Pages" src="https://img.shields.io/badge/Live%20docs-GitHub%20Pages-2b3137?style=for-the-badge&logo=github" />
  </a>
  &nbsp;
  <a href="#" target="_blank" rel="noopener">
    <img alt="Live demos — Binder" src="https://img.shields.io/badge/Live%20demos-Binder-f5a250?style=for-the-badge&logo=jupyter" />
  </a>
</p>

---



## 🎯 Descripción

Material docente de nivel **Ingeniería** para Ciencia de Datos.

El curso asume conocimientos previos de estadística clásica (por ejemplo: ANOVA y tests de hipótesis básicos) y se centra en la **“caja blanca”** de la ingeniería estadística moderna: inferencia computacional, geometría de los datos, regularización, y modelos gráficos probabilísticos (PGMs), con extensión a causalidad y series temporales.

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

## 📚 Bibliografía base (The Canon)

Las referencias bibliográficas del programa se apoyan principalmente en:

- **[Wasserman]** — *All of Statistics: A Concise Course in Statistical Inference* (Larry Wasserman)
- **[ESL]** — *The Elements of Statistical Learning* (Hastie, Tibshirani & Friedman)
- **[BDA3]** — *Bayesian Data Analysis (3rd Ed.)* (Gelman, Carlin, et al.)
- **[Efron]** — *Computer Age Statistical Inference* (Efron & Hastie)
- **[Pearl]** — *Causality: Models, Reasoning, and Inference* (Judea Pearl)
- **[Shumway]** — *Time Series Analysis and Its Applications* (Shumway & Stoffer)

---

## 🎯 Propósito del curso

Conectar **probabilidad multivariante + álgebra lineal + inferencia computacional** con la **geometría de los datos** usada hoy en **ML/IA**: reducción de dimensión, regularización, modelos estructurados, grafos y métodos de simulación/optimización.

---

## 🗺️ Syllabus detallado

### MÓDULO I — Vectores aleatorios y geometría de datos

*Enfoque: la distribución conjunta como objeto geométrico (subespacios, elipsoides, proyecciones, métricas).*

1. **Notación matricial: vector de medias  y matriz de covarianza**
* Definición de  y .
* Propiedades: simetría, semidefinida positiva, interpretación geométrica (varianza por direcciones).
* Varianza de proyecciones:  y métrica inducida.
* **Aplicación en DS/ML:** Feature scaling, *Covariance shift*, distancia de Mahalanobis (detección de outliers).
* **Bibliografía:** **[Wasserman, Ch. 3]**, **[ESL, Ch. 2.4–2.5]**.


2. **Dependencia lineal vs. independencia estadística**
* Dependencia lineal ( rango, singularidad) vs. Independencia estadística ().
* Correlación  independencia (salvo en Gaussianas).
* **Aplicación en DS/ML:** Multicolinealidad en regresión (Ridge/Lasso), *Feature redundancy*, correlación vs. causalidad.
* **Bibliografía:** **[Koller & Friedman, Ch. 2–3]**, **[Bishop, Ch. 8]**, **[Wasserman, Ch. 3–4]**.


3. **Normal multivariante (MVN) y geometría**
* Definición : forma cuadrática, log-densidad y energía.
* **Elipsoides de densidad:** Interpretación geométrica y descomposición espectral ().
* **Whitening:** Blanqueo de datos .
* **Aplicación en DS/ML:** LDA/QDA, PCA (rotación + escalado), Batch/Layer Normalization, Gaussian Processes.
* **Bibliografía:** **[Wasserman, Ch. 14]**, **[Mardia–Kent–Bibby]**, **[ESL, Ch. 3.5 / 14]**, **[Bishop, PCA]**.


4. **Teoría del aprendizaje: concentración de la medida**
* Convergencia en probabilidad vs. en distribución (LLN y CLT).
* Desigualdades de **Chebyshev** y **Hoeffding**: cotas no asintóticas del error.
* **Aplicación en DS/ML:** Generalización (riesgo empírico vs. poblacional), intervalos de confianza para métricas (Accuracy, AUC).
* **Bibliografía:** **[Wasserman, Ch. 4–5]**.



---

### MÓDULO II — Inferencia computacional y “moderna”

*Enfoque: superar las limitaciones de las pruebas de hipótesis clásicas mediante optimización y simulación.*

5. **Teoría asintótica y máxima verosimilitud (MLE)**
* MLE como optimización:  (Gradiente/Hessiano).
* Consistencia, eficiencia, Información de Fisher y cota de Cramér–Rao.
* **Aplicación en DS/ML:** Regresión logística (Cross-entropy), entrenamiento de modelos probabilísticos (Naive Bayes, HMM).
* **Bibliografía:** **[Wasserman, Ch. 9]**, **[Efron & Hastie, Ch. 2]**.


6. **Bootstrap y métodos de resampling**
* Estimación del error estándar sin fórmulas cerradas.
* Bootstrap paramétrico vs. no paramétrico. Intervalos **BCa**.
* **Aplicación en DS/ML:** Incertidumbre en métricas (F1, AUC), Bagging (Random Forest), *Stability selection*.
* **Bibliografía:** **[Wasserman, Ch. 8]**, **[Efron & Hastie, Ch. 10–11]**.


7. **Tests de hipótesis en alta dimensionalidad**
* Tests de Wald, Score y Likelihood Ratio Test (LRT).
* Comparaciones múltiples: Bonferroni y **False Discovery Rate (FDR — Benjamini–Hochberg)**.
* **Aplicación en DS/ML:** A/B testing a escala, selección de features en alta dimensión (genes, texto).
* **Bibliografía:** **[Wasserman, Ch. 10]**, **[ESL, High-Dim Problems]**, **[Efron & Hastie, Ch. 15]**.



---

### MÓDULO III — Aprendizaje estadístico (regresión avanzada)

*Enfoque: trade-off sesgo–varianza, geometría de proyecciones y selección de modelos.*

8. **Geometría de mínimos cuadrados (OLS)**
* Regresión como proyección ortogonal: Matriz sombrero .
* Teorema de Gauss–Markov y diagnóstico (leverage, distancia de Cook).
* **Aplicación en DS/ML:** Baselines interpretables, detección de puntos influyentes en producción.
* **Bibliografía:** **[ESL, Ch. 3.2]**, **[Wasserman, Ch. 13]**.


9. **Regularización y selección de modelos**
* Maldición de la dimensionalidad ().
* **Ridge (L2):** Contracción y priors gaussianos.
* **Lasso (L1):** Sparsity y priors de Laplace. Elastic Net.
* Criterios de información: AIC, BIC, .
* **Aplicación en DS/ML:** Estabilidad en embeddings, selección automática de variables, *Early stopping*.
* **Bibliografía:** **[ESL, Ch. 3.4 y Ch. 7]**, **[Efron & Hastie, Ch. 7 y 16]**.


10. **Modelos lineales generalizados (GLM)**
* Familia exponencial y funciones de enlace (*link*): Logística y Poisson.
* Algoritmo IRLS (Iteratively Reweighted Least Squares).
* **Aplicación en DS/ML:** Clasificación calibrada, modelado de conteos/demanda.
* **Bibliografía:** **[ESL, Ch. 4.4]**, **[Efron & Hastie, Ch. 8]**.



---

### MÓDULO IV — Modelos estructurados, grafos, causalidad y tiempo

*Enfoque: modelar dependencias complejas, inferencia bayesiana y dinámica.*

11. **Probabilistic Graphical Models (PGMs)**
* **DAGs:** Factorización de la conjunta, independencia condicional y **d-separation**.
* *Plate notation* para modelos jerárquicos.
* **Aplicación en DS/ML:** Naive Bayes, HMMs, modelos jerárquicos multitenant.
* **Bibliografía:** **[Koller & Friedman, Ch. 2–4]**, **[Bishop, Ch. 8]**.


12. **Inferencia causal**
* Correlación vs. Causación. Intervenciones y operador .
* Confounders, colliders y criterio *back-door*.
* **Aplicación en DS/ML:** A/B testing, Uplift modeling, eliminación de sesgos en datos.
* **Bibliografía:** **[Pearl, Ch. 1–3]**, **[Wasserman, Ch. 16–17]**.


13. **Inferencia bayesiana y MCMC**
* Priors conjugados vs. no informativos. Posterior como creencia.
* **MCMC:** Metropolis–Hastings y diagnóstico básico.
* **Aplicación en DS/ML:** Bayesian Logistic Regression, Bayesian Optimization, cuantificación de incertidumbre.
* **Bibliografía:** **[BDA3, Ch. 1–3]**, **[Efron & Hastie, Ch. 13]**.


14. **Series temporales y modelos dinámicos**
* Estacionariedad, autocorrelación y modelos ARIMA.
* **State Space Models (SSM):** Filtro de Kalman.
* **Aplicación en DS/ML:** Forecasting (demanda, finanzas), tracking (IoT), comparación con RNNs.
* **Bibliografía:** **[Shumway & Stoffer, Ch. 1–3 y 6]**, **[Bishop, Ch. 13]**.



---

### MÓDULO V — Geometría moderna: grafos, complejidad y búsqueda

*Enfoque: expandir la geometría más allá de lo euclídeo (grafos), dinámica local (autómatas) y optimización no convexa.*

15. **Teoría de grafos para ciencia de datos**
* Matrices de adyacencia, conectividad, caminos, BFS/DFS.
* **Aplicación en DS/ML:** Network science (PageRank, comunidades), recomendadores, detección de fraude.
* **Bibliografía:** **[Benjamin–Chartrand–Zhang]**, **[Kumar]**.


16. **Espectros de grafos y geometría (Spectral Graph Theory)**
* Espectro del Laplaciano; autovalores y autovectores en grafos.
* **Aplicación en DS/ML:** Spectral clustering, Graph Embeddings, fundamentos de GNNs.
* **Bibliografía:** **[Kumar]**, **[ESL/Bishop (ref. espectral)]**.


17. **Modelos sobre grafos y unificación**
* Markov blankets, MRF (Markon Random Fields) y Factor Graphs.
* Inferencia aproximada (Loopy Belief Propagation).
* **Aplicación en DS/ML:** CRFs (secuencias), segmentación de imágenes, denoising.
* **Bibliografía:** **[Koller & Friedman]**, **[Bishop, Ch. 8]**.


18. **Algoritmos evolutivos y programación genética (GP)**
* Optimización sin gradiente en paisajes no convexos.
* GP: Búsqueda en espacios de programas (*Symbolic Regression*).
* **Aplicación en DS/ML:** AutoML, descubrimiento de ecuaciones interpretables, Neuroevolution.
* **Bibliografía:** **[Material de Cátedra: Evolutivos/GP]**.


19. **Autómatas celulares (CA) y dinámica local**
* Reglas locales → Emergencia global. Dinámica en grillas.
* **Aplicación en DS/ML:** Simulación de propagación (epidemias, tráfico), modelos generativos discretos.
* **Bibliografía:** **[Material de Cátedra: Autómatas Celulares]**, **[Wolfram (ref. conceptual)]**.



---

## 📚 Bibliografía General del Curso

* **Wasserman** — *All of Statistics*.
* **Hastie, Tibshirani, Friedman** — *The Elements of Statistical Learning (ESL)*.
* **Efron & Hastie** — *Computer Age Statistical Inference (CASI)*.
* **Bishop** — *Pattern Recognition and Machine Learning (PRML)*.
* **Koller & Friedman** — *Probabilistic Graphical Models*.
* **Gelman et al.** — *Bayesian Data Analysis (BDA3)*.
* **Pearl** — *Causal Inference in Statistics*.
* **Shumway & Stoffer** — *Time Series Analysis and Its Applications*.
* **Mardia, Kent, Bibby** — *Multivariate Analysis*.
* **Benjamin, Chartrand, Zhang** — *The Fascinating World of Graph Theory*.

## 🧱 Estructura del repositorio (high-level)

> *Ajustá estos nombres si difieren en tu repo.*

- `docs/` — sitio MkDocs / GitHub Pages (material por módulo)
- `src/classroom/` — notebooks, scripts y prácticas por módulo
- `assets/` — imágenes, gifs y recursos visuales del curso
- `tests/` — tests (si aplica)
- `requirements.txt` / `pyproject.toml` — dependencias

---

## 🛠️ Uso y ejecución

### 1) Clonar el repositorio

```bash
git clone [https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git)
cd estadisticas-para-ciencia-de-datos

```

### 2) Crear entorno e instalar dependencias (Python)

Se recomienda usar un entorno virtual para evitar conflictos.

```bash
# Crear entorno virtual
python -m venv .venv

# Activar entorno (Linux/macOS):
source .venv/bin/activate

# Activar entorno (Windows):
# .venv\Scripts\activate

# Instalar dependencias
pip install -U pip
pip install -r requirements.txt

```

### 3) Calidad de código (opcional, recomendado)

```bash
pre-commit install
pre-commit run --all-files

```

### 4) Ejecutar notebooks / prácticas

Si trabajás con **Jupyter Lab**:

```bash
jupyter lab

```

Si usás **VSCode**:

> Abre la carpeta del repositorio y ejecuta los archivos `.ipynb` directamente usando la extensión de Jupyter.

---

## ✅ Requisitos y nivel esperado

* **Matemática:**
* Probabilidad y estadística clásica (intervalos, tests básicos, ANOVA).
* Álgebra lineal (vectores, matrices, autovalores/autovectores).


* **Programación:**
* **Python** (lenguaje principal).
* *R / Julia* (como soporte opcional).



## 🤝 Contribuciones

Issues y Pull Requests son bienvenidos.

* Si vas a proponer cambios grandes (estructura, syllabus o tooling), por favor abrí primero un **Issue** describiendo el objetivo y el impacto.

## ⚖️ Licencia

Este material se distribuye bajo licencia **MIT**. Ver el archivo [LICENSE](https://www.google.com/search?q=LICENSE) para más detalles.

## 📌 Referencias (Citas cortas)

* **[Wasserman]** Larry Wasserman — *All of Statistics*
* **[ESL]** Hastie, Tibshirani, Friedman — *The Elements of Statistical Learning*
* **[BDA3]** Gelman et al. — *Bayesian Data Analysis (3rd Ed.)*
* **[Efron]** Efron & Hastie — *Computer Age Statistical Inference*
* **[Pearl]** Judea Pearl — *Causality*
* **[Shumway]** Shumway & Stoffer — *Time Series Analysis and Its Applications*

