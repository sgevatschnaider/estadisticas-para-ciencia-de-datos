Applied Statistics for Data Science (Engineering & Research Track)

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

> *Acceso directo a las carpetas del repositorio con la teoría (simuladores HTML) y el código fuente (Notebooks).*

<p align="center">
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad"><img src="https://img.shields.io/badge/MÓDULO_I-Geometría-0366d6?style=for-the-badge"></a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/inferencia"><img src="https://img.shields.io/badge/MÓDULO_II-Inferencia-0366d6?style=for-the-badge"></a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/learning"><img src="https://img.shields.io/badge/MÓDULO_III-Learning-0366d6?style=for-the-badge"></a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/pgm"><img src="https://img.shields.io/badge/MÓDULO_IV-Estructurados-0366d6?style=for-the-badge"></a>
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/tiempo"><img src="https://img.shields.io/badge/MÓDULO_V-Grafos-0366d6?style=for-the-badge"></a>
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

# MÓDULO I — Vectores Aleatorios y Geometría de Datos

> **Enfoque:** La distribución conjunta como objeto geométrico (subespacios, elipsoides, proyecciones) y la teoría de concentración de la medida.

---

## 📂 Ruta del módulo y Recursos

| Recurso | Enlace al Repositorio |
| :--- | :--- |
| **💻 Código Fuente** | [Ir a carpeta `src/classroom/probabilidad`](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad) |
| **📝 Ejercicios** | [Ver ejercicios](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad/ejercicios) |
| **💡 Soluciones** | [Ver soluciones](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad/soluciones) |

---

## 🗺️ Temario Detallado

### 1. Notación matricial y Geometría ($\mu, \Sigma$)
* **Definiciones:** Vector de medias $\mu = \mathbb{E}[X]$ y matriz de covarianza $\Sigma = \mathbb{E}[(X-\mu)(X-\mu)^\top]$.
* **Propiedades:** Simetría, semidefinida positiva e interpretación geométrica (varianza por direcciones).
* **Proyecciones:** Varianza de $u^\top X$ y métrica inducida.
* *Aplicación:* Feature scaling, Covariance shift, Distancia de Mahalanobis.

### 2. Dependencia Lineal vs. Independencia Estadística
* **Conceptos:** Diferencia entre dependencia lineal (rango, singularidad) e independencia estadística ($p(x,y)=p(x)p(y)$).
* **La falacia de la correlación:** Correlación $\neq$ Independencia (excepto en Gaussianas).
* *Aplicación:* Multicolinealidad en regresión, selección de variables.

### 3. Normal Multivariante (MVN)
* **Definición:** Densidad, forma cuadrática y energía.
* **Geometría:** Elipsoides de densidad y descomposición espectral ($\Sigma = U \Lambda U^\top$).
* **Whitening (Blanqueo):** Transformación $Z=\Lambda^{-1/2}U^\top(X-\mu)$ para decorrelacionar datos.
* *Aplicación:* PCA, Gaussian Processes, Batch Normalization.

### 4. Teoría del Aprendizaje (Concentración de la Medida)
* **Convergencia:** Ley de los Grandes Números (LLN) y Teorema Central del Límite (CLT) vistos como convergencia estocástica.
* **Desigualdades:**
    * **Chebyshev:** Cota básica basada en varianza.
    * **Hoeffding:** Cota exponencial para variables acotadas (fundamental en ML).
* *Aplicación:* Cotas de error en generalización, intervalos de confianza para métricas.

---

## 📚 Bibliografía Específica

* **Wasserman, *All of Statistics*:**
    * Chapter 3: Expectation & Variance.
    * Chapter 4–5: Convergence & Inequalities (Concentration).
    * Chapter 14: Multivariate Models.
* **Hastie et al., *ESL*:**
    * Chapter 2.4–2.5: Statistical Decision Theory / Local Methods.
    * Chapter 3.5: Dimensionality Reduction.
* **Koller & Friedman, *PGM*:**
    * Chapter 2–3: Independence & Factorization.

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

##  Cómo utilizar este material (Instalación y Uso)

Tienes dos formas principales de consumir y ejecutar las clases de este repositorio:

### Opción A: En la Nube (Recomendado)
No necesitas instalar nada en tu computadora.
1. **Simuladores Interactivos:** Haz clic en los botones azules `[![Ver en GitHub]]` de la tabla superior para acceder a los archivos `.html`. Puedes verlos funcionar directamente usando los botones verdes de `[![Ver Simulación Interactiva]]`.
2. **Jupyter Notebooks:** Haz clic en los botones de **Binder** o **Colab** que se encuentran en la parte superior. Esto abrirá un entorno virtual en tu navegador donde podrás ejecutar el código Python celda por celda.

### Opción B: Ejecución Local
Si prefieres tener los archivos en tu máquina:
1. Clona este repositorio:
   ```bash
   git clone [https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git)

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

