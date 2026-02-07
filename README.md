# Estadísticas para Ciencia de Datos — Classroom

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

Material docente reproducible para **Estadísticas para Ciencia de Datos** (Nivel Ingeniería/Posgrado).

Este repositorio se centra en la **caja blanca**: fundamentos probabilísticos, **inferencia moderna** (MLE/Fisher/CRLB/bootstrap), **aprendizaje estadístico** (Regularización/GLM/Bias-Variance) y **modelos estructurados** (PGMs: DAGs, causalidad, series temporales y modelos dinámicos).

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

## 📑 Tabla de Contenidos
* [🎯 Público objetivo y requisitos](#-público-objetivo-y-requisitos)
* [🧰 Stack: Python, R y Julia](#-stack-del-curso-python-r-y-julia)
* [📚 Syllabus](#-programa-del-curso)
* [🧠 La perspectiva de Grafos (PGM)](#-grafos-en-todo-el-curso)
* [🛠️ Uso y ejecución](#️-uso-y-ejecución)
* [⚖️ Licencia](#️-licencia)

---

## 🎯 Público objetivo y requisitos

**Dirigido a:** Estudiantes de Ingeniería, Ciencias de la Computación o Investigadores que necesiten una base rigurosa de inferencia y modelado para Machine Learning.

**Requisitos previos:**
- **Cálculo Multivariable:** Gradiente, Hessiano, optimización básica.
- **Álgebra Lineal:** Proyecciones, descomposición espectral (Eigenvalues/SVD), matrices PSD.
- **Probabilidad:** Bayes, esperanza, varianza, variables aleatorias.
- **Programación:** Fluidez en Python y/o R.

---

## 🧰 Stack del curso: Python, R y Julia

El curso adopta un enfoque políglota pero ordenado:

- **🐍 Python (Core):** Notebooks principales, implementación de algoritmos y pipelines de ML.
- **Example R (Inferencia):** Visualización avanzada (`ggplot2`) y estadística clásica rigurosa.
- **🟣 Julia (High-Performance):** Simulaciones intensivas y optimización "desde cero" (White Box).

> **Nota:** El material troncal se ofrece en **Python**. Las implementaciones en R y Julia son complementarias para mostrar las fortalezas de cada lenguaje en investigación.

---

## 📚 Programa del curso

### MÓDULO 0 — Lenguaje Unificador
- Modelo estadístico: DGP, parámetro $\theta$, likelihood $L(\theta;D)$.
- Riesgo poblacional $R(f)$ vs riesgo empírico $\hat R$.
- **Cross-Cutting Theme:** Notación gráfica (Placas, DAGs) y factorización $P(x)=\prod_i P(x_i \mid pa(i))$.

### MÓDULO I — Fundamentos Probabilísticos
- Probabilidad condicional, independencia y Teorema de Bayes.
- **Multivariante:** Matriz de Covarianza $\Sigma$, Normal Multivariante, geometría y descomposición espectral.
- Teoremas Límites: LLN/CLT y desigualdades de concentración (Chebyshev, Hoeffding).

### MÓDULO II — Inferencia Estadística Moderna
- **Estimación:** MoM, MLE, MAP. Propiedades asintóticas.
- **Incertidumbre:** Información de Fisher, Cota de Cramér-Rao.
- **Inferencia Computacional:** Bootstrap (paramétrico/no paramétrico), Jackknife.
- **Testing:** Tests de Wald, LRT y Score. Problema de comparaciones múltiples (Bonferroni, FDR).

### MÓDULO III — Aprendizaje Estadístico
- **Regresión:** OLS desde la geometría (proyecciones). Diagnóstico (leverage, cook's distance).
- **Selección:** AIC/BIC (teoría de la información) y Validación Cruzada.
- **Regularización:** Ridge (L2) y Lasso (L1). Interpretación Bayesiana.
- **GLMs:** Regresión Logística y Poisson. Familia Exponencial.

### MÓDULO IV — Modelos Estructurados: Grafos y Tiempo
- **PGMs (Probabilistic Graphical Models):** Independencia condicional en grafos, d-separation.
- **Causalidad:** Diferencia entre observar $P(y \mid x)$ e intervenir $P(y \mid do(x))$.
- **Series Temporales:** Estacionariedad y modelos ARIMA.
- **Modelos Dinámicos:** HMM (Hidden Markov Models) y Filtro de Kalman (State-Space).

---

## 🧠 Grafos en todo el curso

Este repositorio utiliza **Modelos Gráficos Probabilísticos** como lenguaje visual transversal:

1.  **Placas (Plate Notation):** Para representar datos i.i.d. y modelos jerárquicos.
2.  **DAGs:** Para visualizar dependencias causales y factorización.
3.  **Cadenas:** Para series temporales y procesos de Markov.

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
2) Estructura de carpetas
Plaintext
src/
├── classroom/       # Material docente organizado por módulos
│   ├── probabilidad/
│   ├── inferencia/
│   ├── learning/
│   ├── pgm/         # Grafos y Causalidad
│   └── tiempo/      # Series Temporales
└── labs/            # Laboratorios prácticos y desafíos
⚖️ Licencia
Este material se distribuye bajo la licencia MIT. Siéntete libre de usarlo para docencia o auto-estudio, citando la fuente original.
