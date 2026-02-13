# Applied Statistics for Data Science (Engineering & Research Track)

<p align="center">
  <img src="assets/portada%20.gif" alt="Visualización de conceptos: MVN, Bootstrap, Regularización, Grafos y Series Temporales" width="100%">
  <br>
  <sub style="font-size: 14px;">
    🔵 <b>Normal Multivariante</b> (Geometría) &nbsp;|&nbsp;
    🟢 <b>Bootstrap</b> (Inferencia) &nbsp;|&nbsp;
    🟠 <b>Regularización</b> (Sparsity)
    <br>
    🔴 <b>DAGs</b> (Causalidad) &nbsp;|&nbsp;
    🟣 <b>Series Temporales</b> (Procesos Estocásticos)
  </sub>
</p>

---

## 🔗 Accesos rápidos

### ✅ Páginas del curso (GitHub Pages) — una por módulo

[![MÓDULO I — Probabilidad](https://img.shields.io/badge/M%C3%93DULO%20I-probabilidad-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/modulos/probabilidad/)
[![MÓDULO II — Inferencia](https://img.shields.io/badge/M%C3%93DULO%20II-inferencia-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/modulos/inferencia/)
[![MÓDULO III — Learning](https://img.shields.io/badge/M%C3%93DULO%20III-learning-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/modulos/learning/)
[![MÓDULO IV — PGM](https://img.shields.io/badge/M%C3%93DULO%20IV-pgm-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/modulos/pgm/)
[![MÓDULO V — Tiempo](https://img.shields.io/badge/M%C3%93DULO%20V-tiempo-0366d6)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/modulos/tiempo/)

### 🧩 Código del curso (por módulo)

[![src/classroom/probabilidad](https://img.shields.io/badge/src-probabilidad-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/probabilidad)
[![src/classroom/inferencia](https://img.shields.io/badge/src-inferencia-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/inferencia)
[![src/classroom/learning](https://img.shields.io/badge/src-learning-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/learning)
[![src/classroom/pgm](https://img.shields.io/badge/src-pgm-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/pgm)
[![src/classroom/tiempo](https://img.shields.io/badge/src-tiempo-0366d6)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/tree/main/src/classroom/tiempo)

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

## 🗺️ Syllabus detallado

### MÓDULO I — Probabilidad multivariante y geometría
*Prerrequisito: dominio de variables aleatorias univariadas y distribuciones estándar.*

1. **Vectores aleatorios y geometría de datos**
   - Notación matricial: vector de medias \(\mu\) y matriz de covarianza \(\Sigma\).
   - Dependencia lineal vs. independencia estadística.
   - **Bibliografía:** **[Wasserman, Ch. 3]**, **[ESL, Ch. 2.4–2.5]**.

2. **Normal multivariante (MVN)**
   - Definición y propiedades geométricas (elipsoides de densidad).
   - Descomposición espectral (eigenvalues) y blanqueo de datos (*whitening*).
   - MVN como base para Gaussian Processes y PCA.
   - **Bibliografía:** **[ESL, Ch. 4.3]**, **[Wasserman, Ch. 14]**.

3. **Teoría del aprendizaje (concentración de la medida)**
   - Revisión de LLN y CLT desde la convergencia estocástica.
   - Desigualdades de **Chebyshev** y **Hoeffding**: ¿por qué aprenden las máquinas? (cotas de error).
   - **Bibliografía:** **[Wasserman, Ch. 4–5]**.

---

### MÓDULO II — Inferencia computacional y “moderna”
*Enfoque: superar las limitaciones de las pruebas de hipótesis “de tabla” mediante simulación.*

4. **Teoría asintótica y máxima verosimilitud (MLE)**
   - MLE como problema de optimización.
   - Propiedades: consistencia, eficiencia y normalidad asintótica.
   - Información de Fisher y cota de Cramér–Rao (límite de precisión).
   - **Bibliografía:** **[Wasserman, Ch. 9]**.

5. **Bootstrap y métodos de resampling**
   - Estimación del error estándar sin fórmulas cerradas.
   - Bootstrap paramétrico vs. no paramétrico. Intervalos de confianza BCa.
   - **Bibliografía:** **[Wasserman, Ch. 8]**, **[Efron, Ch. 10–11]**.

6. **Tests de hipótesis en alta dimensionalidad**
   - Tests de Wald, Score y Likelihood Ratio Test (LRT).
   - Comparaciones múltiples y riesgo de *p-hacking*.
   - Bonferroni y False Discovery Rate (FDR — Benjamini–Hochberg).
   - **Bibliografía:** **[Wasserman, Ch. 10]**, **[Efron, Ch. 15]**.

---

### MÓDULO III — Aprendizaje estadístico (regresión avanzada)
*Enfoque: trade-off sesgo–varianza y selección de modelos.*

7. **Geometría de mínimos cuadrados (OLS)**
   - Regresión como proyección ortogonal en subespacios lineales.
   - Teorema de Gauss–Markov.
   - Diagnóstico: leverage, distancia de Cook y análisis de residuos.
   - **Bibliografía:** **[ESL, Ch. 3.2]**, **[Wasserman, Ch. 13]**.

8. **Regularización y selección de modelos**
   - Maldición de la dimensionalidad (\(p > n\)).
   - **Ridge (L2):** contracción de coeficientes y priors gaussianos.
   - **Lasso (L1):** sparsity y selección de variables (priors de Laplace).
   - Criterios de información: AIC, BIC y Mallows’ \(C_p\).
   - **Bibliografía:** **[ESL, Ch. 3.4 y Ch. 7]**.

9. **Modelos lineales generalizados (GLM)**
   - Familia exponencial de distribuciones.
   - Función de enlace (*link*): logística (clasificación) y Poisson (conteos).
   - IRLS (Iteratively Reweighted Least Squares).
   - **Bibliografía:** **[ESL, Ch. 4.4]**, **[McCullagh & Nelder / Wasserman, Ch. 13]**.

---

### MÓDULO IV — Modelos estructurados, grafos y tiempo
*Enfoque: modelar dependencias complejas y causalidad.*

10. **Probabilistic Graphical Models (PGMs)**
   - **DAGs:** grafos acíclicos dirigidos y factorización de la conjunta.
   - Independencia condicional y **d-separation** (lectura de grafos).
   - *Plate notation* para modelos jerárquicos.
   - **Bibliografía:** **[Wasserman, Ch. 17]**, **[Bishop, Ch. 8]**.

11. **Inferencia causal**
   - Correlación vs. causación: la escalera de Pearl.
   - Intervenciones: operador \(do(x)\).
   - Confounders, colliders y criterio *back-door*.
   - **Bibliografía:** **[Pearl, Ch. 1–3]**, **[Wasserman, Ch. 19]**.

12. **Inferencia bayesiana y MCMC**
   - Priors conjugados vs. no informativos.
   - La posterior como distribución de creencias.
   - Introducción a Markov Chain Monte Carlo (Metropolis–Hastings).
   - **Bibliografía:** **[BDA3, Ch. 1–3]**, **[Wasserman, Ch. 11]**.

13. **Series temporales (grafos dinámicos)**
   - Procesos estocásticos: estacionariedad y autocorrelación.
   - Modelos ARIMA.
   - Modelos de espacio de estados (SSM) y filtro de Kalman.
   - **Bibliografía:** **[Shumway, Ch. 1–3 y Ch. 6]**.

---

## 🧱 Estructura del repositorio (high-level)

> *Ajustá estos nombres si difieren en tu repo.*

- `docs/` — sitio MkDocs / GitHub Pages (material por módulo)
- `src/classroom/` — notebooks, scripts y prácticas por módulo
- `assets/` — imágenes, gifs y recursos visuales del curso
- `tests/` — tests (si aplica)
- `requirements.txt` / `pyproject.toml` — dependencias

---

## 🛠️ Uso y ejecución

### 1) Clonar el repo

```bash
git clone https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos.git
cd estadisticas-para-ciencia-de-datos
2) Crear entorno e instalar dependencias (Python)
python -m venv .venv
# Linux/macOS:
source .venv/bin/activate
# Windows:
# .venv\Scripts\activate

pip install -U pip
pip install -r requirements.txt
3) Calidad de código (opcional, recomendado)
pre-commit install
pre-commit run --all-files
4) Ejecutar notebooks / prácticas
Si trabajás con Jupyter:

jupyter lab
Si usás VSCode: abrí la carpeta del repo y ejecutá notebooks desde la extensión de Jupyter.

✅ Requisitos y nivel esperado
Probabilidad y estadística clásica (intervalos, tests básicos, ANOVA)

Álgebra lineal (vectores, matrices, autovalores/autovectores)

Programación: Python (recomendado); R/Julia como soporte (opcional)

🤝 Contribuciones
Issues y PRs son bienvenidos. Si vas a proponer cambios grandes (estructura, syllabus o tooling), abrí primero un issue describiendo el objetivo y el impacto.

⚖️ Licencia
Este material se distribuye bajo licencia MIT. Ver el archivo LICENSE.

📌 Referencias (citas cortas)
[Wasserman] Larry Wasserman — All of Statistics

[ESL] Hastie, Tibshirani, Friedman — The Elements of Statistical Learning

[BDA3] Gelman et al. — Bayesian Data Analysis (3rd Ed.)

[Efron] Efron & Hastie — Computer Age Statistical Inference

[Pearl] Judea Pearl — Causality

[Shumway] Shumway & Stoffer — Time Series Analysis and Its Applications
