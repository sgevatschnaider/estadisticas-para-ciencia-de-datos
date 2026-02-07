# Estadísticas para Ciencia de Datos — Classroom

# Applied Statistics for Data Science (Engineering & Research Track)

[![src/classroom/probabilidad](https://img.shields.io/badge/src-probabilidad-0366d6)](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom/tree/main/src/classroom/probabilidad)
[![src/classroom/inferencia](https://img.shields.io/badge/src-inferencia-0366d6)](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom/tree/main/src/classroom/inferencia)
[![src/classroom/learning](https://img.shields.io/badge/src-learning-0366d6)](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom/tree/main/src/classroom/learning)
[![src/classroom/pgm](https://img.shields.io/badge/src-pgm-0366d6)](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom/tree/main/src/classroom/pgm)
[![src/classroom/tiempo](https://img.shields.io/badge/src-tiempo-0366d6)](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom/tree/main/src/classroom/tiempo)

<p align="center">
  <a href="https://USUARIO.github.io/Estadisticas-Ciencia-de-Datos-Classroom/" target="_blank" rel="noopener">
    <img alt="Live docs — GitHub Pages" src="https://img.shields.io/badge/Live%20docs-GitHub%20Pages-2b3137?style=for-the-badge&logo=github" />
  </a>
  &nbsp;
  <a href="#" target="_blank" rel="noopener">
    <img alt="Live demos — Binder" src="https://img.shields.io/badge/Live%20demos-Binder-f5a250?style=for-the-badge&logo=jupyter" />
  </a>
</p>

Material docente de nivel **Posgrado / Ingeniería Avanzada** para Ciencia de Datos.

Este curso asume conocimientos previos de estadística clásica (ANOVA, Tests de Hipótesis básicos) y se centra en la **"Caja Blanca"** de la ingeniería moderna: inferencia computacional, geometría de los datos, regularización y modelos gráficos probabilísticos.

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

## 📚 Bibliografía Base (The Canon)

Las referencias bibliográficas en el programa corresponden a las siguientes obras maestras:

* **[Wasserman]**: *All of Statistics: A Concise Course in Statistical Inference* (Larry Wasserman).
* **[ESL]**: *The Elements of Statistical Learning* (Hastie, Tibshirani & Friedman).
* **[BDA3]**: *Bayesian Data Analysis, 3rd Ed.* (Gelman, Carlin, et al.).
* **[Efron]**: *Computer Age Statistical Inference* (Efron & Hastie).
* **[Pearl]**: *Causality: Models, Reasoning, and Inference* (Judea Pearl).
* **[Shumway]**: *Time Series Analysis and Its Applications* (Shumway & Stoffer).

---

## 🗺️ Syllabus Detallado

### MÓDULO I: PROBABILIDAD MULTIVARIANTE Y GEOMETRÍA
*Prerrequisito: Se asume dominio de variables aleatorias univariadas y distribuciones estándar.*

1.  **Vectores Aleatorios y Geometría de Datos**
    * Notación matricial: Vector de medias $\mu$ y Matriz de Covarianza $\Sigma$.
    * Dependencia lineal vs. Independencia estadística.
    * *Bibliografía:* **[Wasserman, Ch. 3]**, **[ESL, Ch. 2.4-2.5]**.
2.  **La Normal Multivariante (MVN)**
    * Definición y propiedades geométricas (elipsoides de densidad).
    * Descomposición Espectral (Eigenvalues) y blanqueo de datos (Whitening).
    * La MVN como base para Gaussian Processes y PCA.
    * *Bibliografía:* **[ESL, Ch. 4.3]**, **[Wasserman, Ch. 14]**.
3.  **Teoría del Aprendizaje (Concentración de la Medida)**
    * Revisión de LLN y CLT desde la convergencia estocástica.
    * Desigualdades de **Chebyshev** y **Hoeffding**: ¿Por qué aprenden las máquinas? (Cotas de error).
    * *Bibliografía:* **[Wasserman, Ch. 4-5]**.

### MÓDULO II: INFERENCIA COMPUTACIONAL Y "MODERNA"
*Enfoque: Superar las limitaciones de las pruebas de hipótesis de "tabla" mediante simulación.*

4.  **Teoría Asintótica y Máxima Verosimilitud (MLE)**
    * El MLE como problema de optimización.
    * Propiedades: Consistencia, Eficiencia y Normalidad Asintótica.
    * Información de Fisher y Cota de Cramér-Rao (Límite de precisión).
    * *Bibliografía:* **[Wasserman, Ch. 9]**.
5.  **El Bootstrap y Métodos de Resampling**
    * Estimación del Error Estándar sin fórmulas cerradas.
    * Bootstrap Paramétrico vs. No Paramétrico. Intervalos de confianza BCa.
    * *Bibliografía:* **[Wasserman, Ch. 8]**, **[Efron, Ch. 10-11]**.
6.  **Tests de Hipótesis en Alta Dimensionalidad**
    * Test de Wald, Score y Likelihood Ratio Test (LRT).
    * El problema de las comparaciones múltiples: P-Hacking.
    * Corrección de Bonferroni y False Discovery Rate (FDR - Benjamini-Hochberg).
    * *Bibliografía:* **[Wasserman, Ch. 10]**, **[Efron, Ch. 15]**.

### MÓDULO III: APRENDIZAJE ESTADÍSTICO (REGRESIÓN AVANZADA)
*Enfoque: Trade-off Sesgo-Varianza y selección de modelos.*

7.  **Geometría de Mínimos Cuadrados (OLS)**
    * Regresión como proyección ortogonal en subespacios lineales.
    * Teorema de Gauss-Markov.
    * Diagnóstico: Leverage, Distancia de Cook y Análisis de Residuos.
    * *Bibliografía:* **[ESL, Ch. 3.2]**, **[Wasserman, Ch. 13]**.
8.  **Regularización y Selección de Modelos**
    * La maldición de la dimensionalidad ($p > n$).
    * **Ridge Regression (L2):** Contracción de coeficientes y priors Gaussianos.
    * **Lasso (L1):** Sparsity y selección de variables (priors de Laplace).
    * Criterios de Información: AIC, BIC y Mallows’ Cp.
    * *Bibliografía:* **[ESL, Ch. 3.4 & Ch. 7]**.
9.  **Modelos Lineales Generalizados (GLM)**
    * Familia Exponencial de distribuciones.
    * Función de enlace (Link function): Logística (Clasificación) y Poisson (Conteos).
    * Algoritmo IRLS (Iteratively Reweighted Least Squares).
    * *Bibliografía:* **[ESL, Ch. 4.4]**, **[McCullagh & Nelder (Clásico) / Wasserman Ch. 13]**.

### MÓDULO IV: MODELOS ESTRUCTURADOS, GRAFOS Y TIEMPO
*Enfoque: Modelar dependencias complejas y causalidad.*

10. **Probabilistic Graphical Models (PGMs)**
    * **DAGs:** Grafos Acíclicos Dirigidos y factorización de la conjunta.
    * Independencia Condicional y **D-Separation** (lectura de grafos).
    * Plate Notation para modelos jerárquicos.
    * *Bibliografía:* **[Wasserman, Ch. 17]**, **[Bishop, Ch. 8]**.
11. **Inferencia Causal**
    * Correlación vs. Causación: La escalera de Pearl.
    * Intervenciones: El operador $do(x)$.
    * Confounders, Colliders y el criterio "Back-door".
    * *Bibliografía:* **[Pearl, Ch. 1-3]**, **[Wasserman, Ch. 19]**.
12. **Inferencia Bayesiana y MCMC**
    * Priors Conjugados vs. No Informativos.
    * La Posterior como distribución de creencias.
    * Muestreo: Introducción a Markov Chain Monte Carlo (Metropolis-Hastings).
    * *Bibliografía:* **[BDA3, Ch. 1-3]**, **[Wasserman, Ch. 11]**.
13. **Series Temporales (Grafos Dinámicos)**
    * Procesos Estocásticos: Estacionariedad y Autocorrelación.
    * Modelos ARIMA.
    * Modelos de Espacio de Estados (SSM) y Filtro de Kalman.
    * *Bibliografía:* **[Shumway, Ch. 1-3 & Ch. 6]**.

---

## 🛠️ Uso y ejecución

### 1) Clonar e instalar dependencias

```bash
git clone [https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom.git](https://github.com/USUARIO/Estadisticas-Ciencia-de-Datos-Classroom.git)
cd Estadisticas-Ciencia-de-Datos-Classroom

# Crear entorno virtual (Recomendado)
python -m venv .venv
source .venv/bin/activate  # En Windows: .venv\Scripts\activate

# Instalar dependencias
pip install -U pip
pip install -r requirements.txt

# Instalar hooks de git (para calidad de código)
pre-commit install
