# MÓDULO I — Vectores Aleatorios y Geometría de Datos

> **Enfoque:** La distribución conjunta como objeto geométrico (subespacios, elipsoides, proyecciones, métricas) y la teoría de concentración de la medida.

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
