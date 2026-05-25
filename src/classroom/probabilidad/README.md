<p align="center">
  <a href="https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/33d808b9c5770d90cf926cb5d35e3ced649d4eee/src/classroom/probabilidad/images/Gif_%20bayes%20y%20gauss.gif">
    <img src="https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/33d808b9c5770d90cf926cb5d35e3ced649d4eee/src/classroom/probabilidad/images/Gif_%20bayes%20y%20gauss.gif" 
         alt="Visualización de inferencia bayesiana y Procesos Gaussianos: reconstrucción probabilística de una superficie continua a partir de puntos observados" 
         width="100%">
  </a>
  <br>
  <sub style="font-size: 14px;">
    🔵 <b>Bayes</b>: hipótesis a priori, evidencia y actualización posterior &nbsp;|&nbsp;
    🟠 <b>Proceso Gaussiano</b>: distribución sobre funciones &nbsp;|&nbsp;
    🟢 <b>Incertidumbre</b>: reconstrucción probabilística desde observaciones parciales
  </sub>
</p>

---

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

| 📄 Recurso                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | 📥 Acceso                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Fase 1: Del Bit al Continuo (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo que demuestra la equivalencia fundamental entre tirar una moneda (bits) y construir un número real en el intervalo [0,1]. Rompe la intuición discreta y establece la base para entender cómo secuencias infinitas definen variables continuas, un concepto vital para PRNGs y transformadas inversas.</p></details>                    | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_moneda.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_moneda.html)                       |
| **Fase 2: Conjuntos Cilíndricos (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Herramienta visual que explica cómo fijar condiciones finitas iniciales crea "bloques" de volumen exacto (conjuntos cilíndricos) en el espacio continuo. Prepara la intuición para comprender las σ-álgebras y cómo se atrapan porciones de medida probabilística, simulando 10,000 secuencias en tiempo real.</p></details>                               | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_cilindros.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_cilindros.html)                 |
| **Fase 3: La Paradoja del Cero (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador que escala el problema del cumpleaños al infinito para ilustrar el colapso de la probabilidad puntual. Demuestra interactivamente que el hecho de que un evento continuo tenga probabilidad de cero (medida de Lebesgue nula) no significa que sea topológicamente imposible.</p></details>                                                       | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_paradoja_del_cero.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_paradoja_del_cero.html) |
| **Fase 4: Árbol Binario en Disco de Poincaré (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Representación avanzada que sitúa el espacio muestral de secuencias como un Grafo de Cayley incrustado en geometría hiperbólica. Ilustra visualmente cómo el espacio muestral continuo reside en el límite infinito (el polvo de Cantor), dándole una interpretación geométrica rigurosa al azar.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/f5d628420572917ffd49460e97d179e475fa464d/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Hiperbolico.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Hiperbolico.html) |
| **Fase 5: Variables Aleatorias y Teoría de la Medida (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Cuaderno teórico en Python que traduce las intuiciones visuales a la formalidad matemática pura. Define rigurosamente la variable aleatoria como una función medible (pushforward), explora la descomposición de Lebesgue, transformaciones con Jacobiano, esperanza matemática y geometría en el espacio L2.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/notebooks/01_Fundamentos_Matematicos_Probabilidad.ipynb)                                                            |
| **Fase 6: La Máquina de la Creación (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Aplicación práctica de toda la teoría anterior utilizando el Teorema de la Transformada Inversa. El simulador muestra cómo una distribución uniforme generada en [0,1] se mapea a través de la función probit para hacer emerger la Campana de Gauss en tiempo real.</p></details>                                                                     | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_creation_machine.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_creation_machine.html)   |
| **Fase 7: El Guardián de las Colas (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo sobre las desigualdades de concentración de Markov y Chebyshev. Permite explorar visualmente cómo acotar probabilidades en las colas sin conocer la distribución subyacente, y demuestra el concepto de cota ajustada mediante un caso límite con distribuciones mixtas (Spike).</p></details>                                    | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Chebyshev_Markov.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Chebyshev_Markov.html)   |
| **Fase 8: La Fábrica de Átomos (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Laboratorio visual que explica la diferencia fundamental entre censurar y truncar datos. Muestra cómo colapsar valores extremos crea masas puntuales ("átomos") en distribuciones continuas, ilustrando intuitivamente la necesidad matemática de la Teoría de la Medida de Lebesgue.</p></details>                                                         | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Fabrica_de_atomos.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Fabrica_de_atomos.html)                           |
| **Fase 9: El Juego de las Monedas Infinitas (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador avanzado que contrasta las integrales de Riemann y Lebesgue. A través de la Función de Dirichlet y la construcción de Conjuntos Cilíndricos mediante lanzamientos de moneda, demuestra cómo Lebesgue agrupa por preimagen para unificar el concepto de Esperanza Matemática.</p></details>                                           | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge\&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_lebesgue_monedas.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_lebesgue_monedas.html)   |
| **Fase 10: Modelo Tobit y Variable Dependiente Limitada (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo que introduce el modelo Tobit para analizar variables dependientes limitadas bajo censura. Explica de forma visual la diferencia entre censura y truncamiento, la lógica de la variable latente, el sesgo de MCO cuando existe efecto techo, la estimación por máxima verosimilitud y la interpretación de efectos marginales. Culmina con una simulación Monte Carlo que compara MCO y Tobit, mostrando cómo el estimador Tobit recupera con mayor fidelidad los parámetros verdaderos en presencia de censura.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/6080f8a1ee27e78d43fdebbcca607c6dd6d5eb19/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad__Modelo_Tobit.html) <br><br> [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad__Modelo_Tobit.html) |
---
## 🎥 Material Audiovisual Complementario (The Video Lectures)

Para consolidar la intuición geométrica y las demostraciones formales de los simuladores, esta es la curaduría definitiva de clases en video. Ideal para repasar conceptos complejos de topología, teoría de la medida y econometría aplicados a la ciencia de datos.

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Teoría de la Medida e Integral de Lebesgue**<br><sub>*Complemento para entender por qué la integración de Riemann falla en el continuo y cómo Lebesgue agrupa por preimagen.*</sub> | **The Bright Side of Mathematics**<br><sub>*Measure Theory (Curso Completo)*</sub> | [![Ver Playlist](https://img.shields.io/badge/Playlist-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLBh2i93oe2qvMVqAzsX1Kuv6-4fjazZ8j) |
| **Desigualdades de Concentración**<br><sub>*La demostración rigurosa de Markov y Chebyshev, fundamental para entender las cotas de error en algoritmos.*</sub> | **Steve Brunton**<br><sub>*Chebyshev's Inequality*</sub><br><br>**MIT OpenCourseWare**<br><sub>*Prof. John Tsitsiklis (Lecture 20)*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=otCHN3s52ho) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=nrDkb2MAwSA) |
| **Método de la Transformada Inversa**<br><sub>*La matemática detrás de la simulación de variables aleatorias usando la función cuantil ($F^{-1}$).*</sub> | **Ben Lambert**<br><sub>*Inverse transform sampling*</sub><br><br>**ritvikmath**<br><sub>*Inverse Transform Sampling*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=rnBbYsysPaU) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=9ixzzPQWuAY) |
| **Topología del Continuo y Medida Cero**<br><sub>*Paradojas del espacio muestral continuo, mapeos infinitos y por qué probabilidad 0 $\neq$ imposible.*</sub> | **3Blue1Brown**<br><sub>*Probabilities of continuous spaces*</sub><br><br>**Vsauce**<br><sub>*How To Count Past Infinity*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ZA4JkHKZM50) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=SrU9YDoXE88) |
| **Censura vs. Truncamiento (Econometría)**<br><sub>*Entendiendo la formación de átomos (masas puntuales) en las colas, esencial para los Modelos Tobit.*</sub> | **Anders Munk-Nielsen**<br><sub>*The Tobit Model*</sub><br><br>**Jake Clifton / Ben Lambert**<br><sub>*Econometrics II (Playlist)*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=IwsE8Rr6l6E) <br><br> [![Ver Playlist](https://img.shields.io/badge/Playlist-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLLZ4uVeiDmR_rzu-uYl9A5BrmvTKtH_aB) |

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Glosario Avanzado: Probabilidad & Teoría de la Medida** <br> <details><summary><strong>Resumen:</strong> <small><em>(haz clic para expandir)</em></small></summary><p>Diccionario interactivo con 46 términos rigurosos que fundamentan la probabilidad moderna. Abarca desde la integral de Lebesgue y la terna de Kolmogorov, hasta la paradoja del cero y las desigualdades de concentración. Incluye definiciones matemáticas precisas y ejemplos concretos esenciales para ciencia de datos.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Glosario.html) <br> [![Ver Glosario Interactivo](https://img.shields.io/badge/Ver%20Glosario-Interactivo-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Glosario.html) |
| **Cuestionario Académico: Probabilidad Moderna** <br> <details><summary><strong>Resumen:</strong> <small><em>(haz clic para expandir)</em></small></summary><p>Evaluación interactiva de 20 preguntas diseñada para desafiar y consolidar la intuición estadística. Contrasta los enfoques de integración de Riemann y Lebesgue, explora el comportamiento de distribuciones continuas vs. discretas, y pone a prueba el dominio sobre los teoremas límite y tiempos de parada.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/main/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Cuestionario.html) <br> [![Ver Cuestionario Interactivo](https://img.shields.io/badge/Ver%20Cuestionario-Interactivo-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_Cuestionario.html) |

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Estadística para Ciencia de Datos – MÓDULO I (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Notebook interactivo en Python que desarrolla la geometría de la media y la matriz de covarianza desde una perspectiva algebraica, estadística y visual. Explica cómo la covarianza determina elipsoides de dispersión, introduce el blanqueo (whitening) como transformación que esferiza los datos, presenta PCA como criterio variacional de máxima varianza, formaliza la distancia de Mahalanobis como métrica inducida por la matriz de precisión y extiende el análisis hacia regularización, covariance shift y concentración direccional en alta dimensión. El contenido combina teoría matemática, simulación numérica, generación de gráficos y presentación HTML embebida dentro del notebook.</p></details> | [![Ver en GitHub](https://img.shields.io/badge/Ver%20en-GitHub-blue?style=for-the-badge&logo=github)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/96aa0491842eb6bdba5dd22a665cbe3732234138/src/classroom/probabilidad/notebooks/Estad%C3%ADstica_para_ciencia_de_datos_M%C3%93DULO_I.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/96aa0491842eb6bdba5dd22a665cbe3732234138/src/classroom/probabilidad/notebooks/Estad%C3%ADstica_para_ciencia_de_datos_M%C3%93DULO_I.ipynb) |

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Módulo 1: Notación Matricial y Geometría (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Lección interactiva sobre la geometría de la media y la matriz de covarianza en vectores aleatorios. Reúne visualizaciones de elipsoides de dispersión, PCA, whitening, distancia de Mahalanobis, feature scaling, covariance shift, concentración subgaussiana y divergencia KL para mostrar cómo la covarianza estructura la forma, la distancia y la incertidumbre en ciencia de datos.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo_1_%20Matricial%20y%20Geometr%C3%ADa_Notacion_Matricial.html) |
| **Módulo 1: Matricial y Geometría del Elipsoide (Visualización Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización educativa 3D centrada en la geometría del elipsoide como superficie cuadrática y como objeto estadístico. Permite manipular interactivamente los semiejes, explorar casos notables, observar secciones planas y vincular la ecuación canónica con autovalores, autovectores y elipsoides de nivel en estadística multivariada.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo_1_%20Matricial%20y%20Geometr%C3%ADa_elipsoide.html) |
| **Módulo 1: Dron con CMA-ES (Simulación Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación interactiva de optimización evolutiva con CMA-ES aplicada a la navegación de un dron en un entorno con obstáculos. Ilustra cómo la estrategia adapta su matriz de covarianza para aprender trayectorias eficientes hacia un objetivo, mientras el usuario modifica parámetros del algoritmo y observa métricas y modos de visualización en tiempo real.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo_1_%20Matricial%20y%20Geometr%C3%ADa_Dron.cma-es.html) |
| **Módulo 1: Explicación Interactiva de CMA-ES** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Lección interactiva que explica de manera visual e intuitiva el algoritmo CMA-ES a partir del simulador del dron. Desarrolla la lógica de la media de búsqueda, la matriz de covarianza, la escala global de exploración, la población candidata, la selección de élite, la función de fitness con penalizaciones y la convergencia del algoritmo. Integra álgebra lineal, geometría del elipsoide y optimización evolutiva en una presentación didáctica diseñada para comprender cómo CMA-ES aprende una distribución de búsqueda adaptativa.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/01_Fundamentos_Matematicos_Probabilidad_cmaes_explicacion_interactiva.html) |

## 📝 Dependencia lineal, independencia estadística y geometría de datos

Esta sección reúne una serie de materiales HTML interactivos orientados a estudiar, de manera articulada, cómo se relacionan la estructura algebraica de los datos, las nociones de dependencia e independencia, y su interpretación geométrica en espacios de distinta dimensión.

El recorrido está organizado como una secuencia pedagógica: primero se introduce la diferencia entre dependencia lineal e independencia estadística como conceptos que no deben confundirse; luego se explora el papel del elipsoide y de la geometría de datos para interpretar covarianza, dispersión y alineación; a continuación se profundiza en la dependencia lineal como fenómeno de colapso geométrico y reducción dimensional, junto con una lectura complementaria sobre el teseracto como extensión de la intuición geométrica hacia dimensiones superiores; y finalmente se incorporan un glosario conceptual y un cuestionario integrador para consolidar vocabulario técnico, relaciones entre conceptos y comprensión general del módulo.
| 📄 Recurso | 📥 Acceso |
|---|---|
| **Dependencia lineal vs. independencia estadística** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso interactivo desarrolla la diferencia entre dependencia lineal e independencia estadística desde una perspectiva algebraica, geométrica y aplicada. Explica cómo ambas nociones no deben confundirse, analiza su relación con correlación, caso gaussiano y multicolinealidad, y muestra por qué son conceptos centrales en regresión, selección de variables y análisis de datos. Es un material útil para comprender la diferencia entre estructura algebraica de los datos y relaciones probabilísticas entre variables.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia_lineal_independencia_estadistica.html) |
| **Dependencia lineal: elipsoide y geometría de datos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este material presenta el elipsoide como objeto geométrico central en la geometría de datos. Explica cómo la matriz de covarianza y la descomposición espectral permiten interpretar dependencia lineal, multicolinealidad e independencia estadística a partir de la forma, orientación y degeneración del elipsoide. El recurso conecta álgebra lineal, estadística multivariada y visualización geométrica, mostrando cómo los autovalores y autovectores describen dispersión, anisotropía y alineación de los datos.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia%20lineal_elipsoide_geometria_datos.html) |
| **Dependencia lineal como colapso geométrico** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso interactivo presenta la dependencia lineal como un fenómeno de colapso geométrico: los vectores dejan de generar nuevas direcciones y el espacio efectivo se reduce a un subespacio de menor dimensión. A través de una visualización dinámica del rango, los vectores generadores y las ecuaciones de dependencia, el material permite comprender de manera intuitiva cómo la pérdida de independencia se traduce en singularidad, reducción dimensional y disminución de la riqueza estructural de los datos. Es una pieza especialmente útil para conectar combinaciones lineales, rango matricial y representación geométrica en una misma narrativa visual.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I%20_punto%202_Colapso.html) |
| **Teseracto: más allá de la dimensión visible** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este artículo ofrece una aproximación conceptual al teseracto como extensión natural del cubo hacia una cuarta dimensión. Su interés no reside solo en presentar una figura geométrica llamativa, sino en invitar a pensar cómo se generalizan las formas, las relaciones espaciales y las simetrías cuando se supera el marco intuitivo de las tres dimensiones. El texto resulta especialmente útil como complemento de los recursos sobre colapso geométrico, hipercubos y representación multidimensional, porque aporta una mirada más reflexiva sobre la visualización de objetos de alta dimensión y sobre los límites de nuestra intuición espacial. En conjunto, propone un puente sugerente entre imaginación geométrica, formalización matemática y comprensión de estructuras complejas.</p></details> | [![Artículo / Blog](https://img.shields.io/badge/Artículo-Blog-orange?style=for-the-badge&logo=blogger)](https://economiayetica.blogspot.com/2025/04/teseracto-mas-alla-de-la-dimension_10.html) |
| **Dependencia lineal e independencia: geometría de los datos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este HTML ofrece una visión integradora de la geometría de los datos al representar observaciones como puntos, variables como vectores y relaciones entre columnas como ángulos, proyecciones y subespacios. El recorrido muestra cómo la dependencia lineal puede interpretarse visualmente a partir de colapsos sobre rectas o planos, y cómo el rango resume la dimensión efectiva del sistema de datos. La propuesta resulta especialmente valiosa porque articula intuición geométrica, álgebra lineal y análisis estadístico, ayudando a comprender cuándo una variable aporta una dirección genuinamente nueva y cuándo simplemente reproduce información ya contenida en otras.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I%20_punto%202_Dependencia_lineal%20e%20independencia.html) |
| **Glosario: dependencia lineal, independencia estadística, correlación y multicolinealidad** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este glosario reúne y organiza los conceptos fundamentales vinculados con dependencia lineal, independencia estadística, correlación y multicolinealidad. Presenta definiciones claras, precisiones terminológicas y relaciones entre los conceptos principales, sirviendo como material de consulta y apoyo para el estudio de álgebra lineal, geometría de datos y estadística. Es especialmente útil como referencia rápida para consolidar vocabulario técnico y comprender diferencias conceptuales clave.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia_lineal_glosario.html) |
| **Cuestionario: dependencia lineal, independencia estadística y geometría de datos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este cuestionario interactivo reúne 20 preguntas con respuestas desarrolladas sobre dependencia lineal, independencia estadística, correlación, multicolinealidad y geometría de datos. El material está pensado para repasar los conceptos centrales del módulo de manera guiada, relacionando la interpretación algebraica, probabilística y geométrica de los datos. Resulta especialmente útil como instrumento de autoevaluación, estudio previo a exámenes y consolidación conceptual de los contenidos trabajados en los recursos teóricos del módulo.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Modulo%20I%20_punto%202_Cuestionario.html) |

## 📝 Distribución, distancia, geometría y paseos aleatorios

Esta sección reúne un **notebook base en Google Colab** y una serie de **materiales HTML interactivos** orientados a estudiar, de manera articulada, cómo se relacionan la **distribución de los datos**, la **noción de distancia**, la **geometría del espacio** y el **comportamiento asintótico de procesos aleatorios**.  
El recorrido está organizado en una secuencia pedagógica: primero se presenta el mapa conceptual general del módulo; luego se explora cómo distintas métricas inducen distintas geometrías; después se analiza el papel de la covarianza y de la distancia de Mahalanobis en contextos aplicados; a continuación se introduce la geometría hiperbólica como alternativa al espacio euclídeo; y finalmente se estudian simulaciones de paseos aleatorios bidimensionales, tanto en su convergencia hacia una normal bivariada como en su vínculo con la constante π.

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Notebook base en Google Colab: distribución, distancia y geometría de los datos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este notebook constituye el eje conceptual del módulo. Organiza de manera progresiva la relación entre distribución, métrica, geometría y modelado, mostrando cómo los datos pueden entenderse como puntos en un espacio cuya estructura no es neutral. A lo largo del recorrido se desarrollan la noción de distribución en <code>R^k</code>, el papel de las métricas y de la familia de Minkowski, las limitaciones del espacio euclídeo para representar ciertas estructuras y la importancia de la geometría hiperbólica en contextos jerárquicos. Funciona como material integrador y como punto de partida para interpretar los HTML interactivos específicos que acompañan esta sección.</p></details> | [![Google Colab](https://img.shields.io/badge/Colab-Abrir%20Notebook-orange?style=for-the-badge&logo=google-colab)](https://colab.research.google.com/drive/13HSXMoNuOoKXLmsfb7dks9VOYNwTYvX-?usp=sharing) |
| **Bolas unitarias: L₁, L₂ y L∞** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso interactivo muestra que la distancia entre puntos no es un concepto único, sino que depende de la métrica elegida. A través de la comparación entre las bolas unitarias asociadas a las normas <code>L₁</code>, <code>L₂</code> y <code>L∞</code>, el material permite visualizar cómo cambia la forma de la cercanía geométrica según el criterio utilizado. La propuesta resulta especialmente útil para comprender que las métricas inducen geometrías distintas y que esa diferencia repercute en la interpretación espacial de los datos, en la forma de las regiones de decisión y en la lógica de numerosos algoritmos de machine learning, optimización y análisis multivariado.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/M%C3%93DULO%20I%E2%80%94%20%28MVN%29_bolas_unitarias.html) |
| **Crédito fantasma: distancia euclídea vs. Mahalanobis** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este HTML desarrolla una aplicación geométrica y estadística de gran valor analítico: la diferencia entre medir cercanía con distancia euclídea y medirla teniendo en cuenta la estructura de covarianza de los datos. A partir de un caso estilizado de scoring y observaciones anómalas, el recurso muestra por qué un punto puede parecer próximo al centro bajo un criterio ingenuo y, sin embargo, resultar atípico cuando se utiliza la distancia de Mahalanobis. El material conecta elipses de nivel, matrices de covarianza, anisotropía, detección de outliers y análisis de riesgo, y funciona como una excelente introducción aplicada a la geometría estadística de la distribución normal multivariada.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/M%C3%93DULO%20I%E2%80%94%20%28MVN%29_credito_fantasma.html) |
| **Crecimiento de un árbol: espacio euclídeo vs. hiperbólico** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso permite entender de manera visual por qué el espacio euclídeo no siempre es adecuado para representar estructuras con crecimiento exponencial o fuerte jerarquía. Mediante la comparación entre un árbol embebido en el plano y su representación en el disco de Poincaré, el HTML muestra cómo el espacio hiperbólico ofrece una geometría más compatible con taxonomías, grafos jerárquicos y sistemas ramificados. El material es particularmente valioso porque traduce una idea abstracta en una intuición visual concreta: cuando la estructura de los datos crece más rápido que el volumen disponible en el espacio euclídeo, la representación se deforma, mientras que la geometría hiperbólica conserva mejor la organización global.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/M%C3%93DULO%20I%E2%80%94%20%28MVN%29_hiperbolico.html) |
| **Paseo aleatorio en ℤ² y convergencia a una normal bivariada** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este HTML ilustra cómo una dinámica discreta definida sobre una grilla bidimensional puede generar, tras la normalización adecuada, una estructura continua de tipo gaussiano. A través de simulaciones de múltiples trayectorias en <code>ℤ²</code>, el recurso permite observar la nube empírica de posiciones finales, su reescalamiento y su aproximación a una normal bivariada. De este modo, el material ofrece una visualización intuitiva del Teorema Central del Límite en dimensión dos y conecta proceso discreto, covarianza, simetría, densidad límite y comportamiento agregado. Es una pieza clave para mostrar cómo reglas locales simples producen regularidades globales profundamente estructuradas.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/M%C3%93DULO%20I%E2%80%94%20%28MVN%29_paseo_aleatorio_Z2.html) |
| **Paseo aleatorio en ℤ² y estimación de π** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso muestra una conexión clásica y sorprendente entre probabilidad discreta, recurrencia y una de las constantes fundamentales de la matemática. A partir del análisis del paseo aleatorio bidimensional y de la probabilidad de retorno al origen, el HTML permite explorar cómo aparecen estimaciones numéricas de <code>π</code> asociadas al comportamiento asintótico de <code>p₂ₙ(0,0)</code>. La visualización vincula simulación, estructura de la grilla, difusión y ley límite, destacando que procesos aleatorios definidos por reglas extremadamente simples pueden contener relaciones profundas con resultados analíticos de gran elegancia. Es un excelente cierre de la secuencia porque integra intuición geométrica, fenómeno probabilístico y aproximación numérica en un mismo marco conceptual.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/M%C3%93DULO%20I%E2%80%94%20%28MVN%29_paseo-aleatorio-pi.html) |

---
## 📝 El infinito en un grafo

| 📄 Recurso | 📥 Acceso |
|---|---|
| **El grafo infinito en ℤ² (Notebook en Google Colab)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este cuaderno en Google Colab desarrolla el estudio del grafo infinito sobre <code>ℤ²</code> como extensión natural de una grilla finita. Presenta la definición formal del grafo, sus propiedades estructurales —conectividad, regularidad, bipartición, simetrías y ausencia de borde— y su relación con el paseo aleatorio simple. El material funciona como base teórica y computacional para comprender la recurrencia en dimensión dos, la probabilidad de retorno al origen y la conexión entre grafos, probabilidad y análisis.</p></details> | [![Google Colab](https://img.shields.io/badge/Google%20Colab-Abrir-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/159n9ZP_CJnUuUNF-bSCnIQyTLaxwUGuL?usp=sharing) |
| **Paseo aleatorio y número π (HTML interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso interactivo explora el paseo aleatorio simple sobre <code>ℤ²</code> y su vínculo con la constante <code>π</code>. La simulación visualiza la difusión empírica sobre la grilla, estima probabilidades de retorno al origen y compara numéricamente la ley asintótica <code>p₂ₙ(0,0) ∼ 1/(πn)</code>. Además, incorpora estimadores de <code>π</code> basados en sumas acumuladas y ajustes sobre los datos simulados, gráficos de convergencia, bandas de error, controles de velocidad, suavizado y cambio de tema visual. Es un material ideal para conectar teoría probabilística, evidencia computacional e intuición geométrica en un entorno interactivo.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML%20Interactivo-Abrir-1F6FEB?style=for-the-badge&logo=googlechrome&logoColor=white)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/ed2889f391d8528c8d64999358e88fe6129cc5d9/src/classroom/graphs/recursos/paseo-aleatorio-pi.html) |
| **Tres actos del paseo aleatorio (HTML interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso propone una puesta en escena visual del paseo aleatorio a través de tres estructuras sucesivas: una malla pequeña <code>3×3</code>, una malla grande <code>31×31</code> y un toro discreto <code>T²</code>. La simulación muestra cómo cambia la experiencia del caminante cuando la frontera domina, cuando se aleja y cuando desaparece mediante identificación topológica. Incluye transiciones entre actos, ejecución paso a paso o automática, control de velocidad, cambio de tema visual, estadísticas en tiempo real —pasos, nodos visitados, grado, cobertura y presencia en borde— y una cámara dinámica en el caso toroidal. Es un recurso especialmente útil para comparar de manera intuitiva el efecto estructural del borde, la homogeneidad local y la diferencia entre una red finita acotada y una red sin fronteras aparentes.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML%20Interactivo-Abrir-1F6FEB?style=for-the-badge&logo=googlechrome&logoColor=white)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/501879b80b140ccea63475397dc7c8a9ea2f73af/src/classroom/graphs/recursos/tres_actos_paseo_aleatorio.html) |
| **Caminante aleatorio en una malla finita (HTML interactivo)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este material interactivo permite explorar un paseo aleatorio simple sobre una malla finita de tamaño variable. El usuario puede modificar la dimensión de la grilla, ajustar la velocidad de ejecución y alternar entre distintos modos de visualización, como mapa de calor, trayectoria o vista limpia. La interfaz incorpora estadísticas en tiempo real —pasos realizados, cantidad de nodos visitados, grado del nodo actual, cobertura de la malla, máximo de visitas por nodo y posición del caminante— junto con controles para avanzar paso a paso, automatizar el recorrido, reiniciar o limpiar la simulación. El recurso resulta especialmente valioso para comprender cómo la estructura local del grafo condiciona las decisiones del caminante y cómo emergen patrones de exploración, recurrencia y cobertura en una red discreta.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML%20Interactivo-Abrir-1F6FEB?style=for-the-badge&logo=googlechrome&logoColor=white)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/501879b80b140ccea63475397dc7c8a9ea2f73af/src/classroom/graphs/recursos/random_walk_3x3.html) |
| **Del borde al infinito: de una malla 3×3 al grafo ℤ² y su vínculo con π (Artículo en blog)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este artículo desarrolla un recorrido conceptual y divulgativo que parte de una malla <code>3×3</code> como laboratorio visual del paseo aleatorio y avanza hacia la red infinita <code>ℤ²</code>, donde desaparecen los efectos de borde y emerge una estructura homogénea. A partir de allí introduce la pregunta por el retorno al origen, explica por qué este solo puede estudiarse en tiempos pares y presenta la relación asintótica <code>p₂ₙ(0,0) ∼ 1/(πn)</code>, mostrando cómo una dinámica discreta sobre grafos conduce de manera natural hacia una constante central de la geometría continua. El texto funciona como un puente entre intuición visual, teoría de grafos, probabilidad y comportamiento asintótico, y resulta especialmente valioso para mostrar que lo discreto y lo continuo pueden formar parte de una misma historia matemática.</p></details> | [![Artículo en Blog](https://img.shields.io/badge/Blog-Art%C3%ADculo-FF6F00?style=for-the-badge&logo=blogger&logoColor=white)](https://economiayetica.blogspot.com/2026/03/caminante-aleatorio-en-grafo-malla.html) |

## 📝 Procesos Gaussianos: Inferencia, geometría probabilística y optimización

Esta sección reúne un **notebook base en Google Colab** y una serie de **materiales HTML interactivos** orientados a estudiar, de manera articulada, cómo se relacionan la **inferencia bayesiana**, las **funciones de covarianza (kernels)**, la **cuantificación de la incertidumbre** y el uso de **modelos probabilísticos sustitutos**. 
El recorrido está organizado en una secuencia pedagógica: primero se sientan las bases de la regresión y la transición de *prior* a *posterior*; luego se explora visualmente el papel del kernel como generador de estructura geométrica; después se analiza la selección bayesiana de hiperparámetros mediante la verosimilitud marginal; a continuación, se aplican estos conceptos a la optimización bayesiana y a la emulación de funciones costosas; y finalmente, se expande el marco teórico conectando los procesos gaussianos con estructuras complejas como algoritmos evolutivos, dinámicas sobre grafos, autómatas celulares y programación genética.

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Procesos Gaussianos (Notebook en Google Colab)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Notebook central de estudio sobre procesos gaussianos. Reúne el desarrollo conceptual del tema, articula la relación entre media, covarianza, kernels e inferencia posterior, y sirve como eje organizador del resto de los simuladores interactivos.</p></details> | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1NEbQL0qxzL7E5nEpSRQWnmPUvk8nmsZY?usp=sharing) |
| **Procesos Gaussianos: comparación entre geometrías** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización interactiva que muestra la continuidad entre la normal multivariante y los procesos gaussianos: desde la geometría elipsoidal definida por la covarianza en espacios finitos hasta la interpretación de los GP como distribuciones sobre funciones. Incluye kernels, proyecciones finitas, descomposición espectral, regresión gaussiana, aplicaciones y consideraciones prácticas.</p></details> | [![Ver Recurso Interactivo](https://img.shields.io/badge/Ver%20Recurso-Interactivo-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Procesos_gaussianos_%20comparacion%20entre%20geometr%C3%ADas.html) |
| **Procesos Gaussianos (Simulador Principal)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo principal para explorar regresión con procesos gaussianos. Permite alternar entre prior y posterior, agregar observaciones, cambiar kernels, ajustar hiperparámetros como longitud de escala, varianza de señal y ruido, y visualizar en tiempo real la media predictiva y las bandas de incertidumbre.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano.html) |
| **Visualizador de Kernels (Sección 3)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Herramienta visual para entender el papel del kernel como generador de estructura geométrica y probabilística. Muestra la matriz \(K(x,x')\) como heatmap, permite variar hiperparámetros y comparar cómo cambia la forma de las funciones muestreadas cuando se modifica la noción de similitud entre entradas.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_kernel.html) |
| **Verosimilitud Marginal GP (Sección 5)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación dedicada a la log-verosimilitud marginal \( \log p(y \mid X,\theta) \) como función de los hiperparámetros del modelo. Permite visualizar cómo el GP equilibra ajuste a los datos y complejidad efectiva, mostrando de manera intuitiva por qué la selección bayesiana de hiperparámetros surge del propio modelo.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano__marginal_likelihood.html) |
| **Optimización Bayesiana (Simulador)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador de búsqueda secuencial del mínimo de una función costosa mediante un GP y funciones de adquisición. Permite observar cómo el modelo decide dónde evaluar a continuación, equilibrando exploración y explotación, y cómo el criterio elegido guía la estrategia de decisión.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_bayesian_optimization_simulator.html) |
| **Modelo Sustituto / Emulador (Sección 8)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación de un surrogate model para emular una función costosa mediante un proceso gaussiano. Muestra el diseño secuencial de experimentos, la actualización del posterior, la curva de adquisición y métricas como error del emulador y regret, ilustrando cómo un GP puede reemplazar evaluaciones caras por inferencia probabilística eficiente.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_modelo_sustituto_emulador.html) |
| **Glosario de Procesos Gaussianos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Glosario interactivo con los conceptos fundamentales del tema: covarianza, normal multivariante, kernel, regresión GP, verosimilitud marginal, RKHS, optimización bayesiana y conexiones con redes neuronales. Funciona como material de consulta y repaso conceptual del módulo completo.</p></details> | [![Ver Recurso Interactivo](https://img.shields.io/badge/Ver%20Recurso-Interactivo-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Proceso_Gaussiano__glosario.html) |
| **Cuestionario de Procesos Gaussianos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Cuestionario interactivo de repaso con preguntas y respuestas desarrolladas sobre los principales ejes del módulo. Está pensado para consolidar comprensión teórica, reforzar intuiciones matemáticas y servir como herramienta de autoevaluación al final del recorrido.</p></details> | [![Ver Recurso Interactivo](https://img.shields.io/badge/Ver%20Recurso-Interactivo-green?style=for-the-badge&logo=blogger)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Proceso_Gaussiano__cuestionario_procesos_gaussianos.html) |
| **Algoritmo Genético + Procesos Gaussianos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo de optimización asistida por modelo sustituto. Ilustra cómo un algoritmo genético actúa como motor de búsqueda global, apoyándose en una función de adquisición derivada de un proceso gaussiano para equilibrar exploración y explotación sin consultar continuamente una función real costosa.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_Algoritmo_Genetico.html) |
| **Proceso Gaussiano sobre Grafos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Implementación de un proceso gaussiano indexado por nodos de un grafo. Permite explorar cómo topologías de red definen la covarianza probabilística a través de distintos kernels (Heat kernel, Regularized Laplacian, Graph-distance RBF) para tareas como regresión en redes e imputación de valores.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_Grafos.html) |
| **Proceso Gaussiano + Autómata Celular** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Demo interactiva que combina la microdinámica discreta de un autómata celular con la reconstrucción de un campo macroscópico continuo mediante un proceso gaussiano. Permite visualizar el suavizado espacial, la interpolación en zonas no observadas y la cuantificación explícita de la incertidumbre.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_automatas_celulares.html) |
| **Proceso Gaussiano + Programación Genética** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación que explora el uso de programación genética para descubrir y evolucionar automáticamente funciones de covarianza (kernels) válidas. Construye expresiones simbólicas combinando kernels base para adaptar la geometría probabilística del modelo a los datos y reducir el error predictivo.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge&logo=blogger)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/main/src/classroom/probabilidad/html/Proceso_Gaussiano_programacion_genetica.html) |

---
| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Fundamentos de Procesos Gaussianos y Geometría Probabilística**<br><sub>*La intuición matemática de cómo pasamos de una Distribución Normal Multivariante a una distribución sobre infinitas funciones.*</sub> | **Mutual Information**<br><sub>*Gaussian Processes*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=UBDgSHPxVME) |
| **Introducción a la Regresión con Procesos Gaussianos**<br><sub>*Implementación y comprensión de las predicciones: cómo el modelo entrega una media (μ) y bandas de incertidumbre (± 2σ).*</sub> | **paretos**<br><sub>*Easy introduction to gaussian process regression*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=iDzaoEwd0N0) |
| **Modelos Probabilísticos sobre Funciones**<br><sub>*Desglose didáctico de cómo los GPs cuantifican la incertidumbre al definir distribuciones directamente sobre curvas.*</sub> | **DataMListic**<br><sub>*Gaussian Processes*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=BTEbaPoZ08Y) |
| **Optimización Bayesiana y Diseño Secuencial**<br><sub>*Explicación paso a paso del uso de modelos sustitutos (surrogate models) y funciones de adquisición para encontrar mínimos globales.*</sub> | **paretos**<br><sub>*Bayesian Optimization (Bayes Opt)*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=M-NTkxfd7-8) |
| **El Dilema de Exploración vs. Explotación**<br><sub>*Construcción de modelos para funciones desconocidas y la lógica estratégica detrás de funciones de adquisición como LCB o EI.*</sub> | **DataMListic**<br><sub>*Bayesian Optimization*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=Kq6_kzlwSUQ) |

📝 Inferencia Bayesiana: aprendizaje secuencial, incertidumbre y decisión óptima

Esta sección reúne un notebook base en Google Colab y una serie de materiales HTML interactivos orientados a estudiar, de manera integrada, cómo la inferencia bayesiana permite actualizar conocimiento, cuantificar incertidumbre y tomar decisiones óptimas bajo información parcial.

El recorrido se estructura como una secuencia conceptual progresiva: en primer lugar, se presentan los fundamentos de la actualización bayesiana, mostrando cómo la combinación entre prior, verosimilitud y datos observados da lugar a la distribución posterior; posteriormente, se analiza el rol de los modelos probabilísticos como representaciones de creencias sobre funciones desconocidas, incorporando explícitamente la incertidumbre en la predicción; luego, se introduce la lógica de aprendizaje secuencial, donde cada nueva observación modifica el estado del conocimiento y redefine el espacio de decisión.

A continuación, estos principios se aplican a la optimización bayesiana, donde la incertidumbre deja de ser solo una medida descriptiva y pasa a ser un componente activo en la toma de decisiones, a través de funciones de adquisición que equilibran exploración y explotación. Finalmente, el marco se amplía hacia contextos más complejos, donde la inferencia bayesiana se integra con simulación, búsqueda adaptativa y modelos sustitutos, permitiendo abordar problemas donde la evaluación directa es costosa, incompleta o ruidosa.

En conjunto, los materiales permiten comprender a la inferencia bayesiana no solo como un método estadístico, sino como un paradigma general de aprendizaje y decisión en sistemas complejos.

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Notebook: Procesos estocásticos y optimización bayesiana** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>El notebook desarrolla una secuencia de 10 puntos clave. Comienza con los fundamentos de los procesos estocásticos bajo el enfoque bayesiano, analizando el rol fundamental de los kernels (RBF, Matérn) y la inferencia posterior. Luego, introduce la metodología de la optimización bayesiana, explicando cómo el modelo sustituto probabilístico y las funciones de adquisición (Expected Improvement, Probability of Improvement, UCB) gestionan el balance matemático entre exploración y explotación. Finalmente, aborda comparaciones rigurosas con otros algoritmos (deterministas y evolutivos), sus ventajas en eficiencia muestral, extensiones metodológicas y aplicaciones en machine learning y diseño experimental.</p></details> | [![Google Colab](https://img.shields.io/badge/Colab-Abrir%20Notebook-orange?style=for-the-badge&logo=google-colab)](https://colab.research.google.com/drive/1DKc5cpFmsZyh0euzDjmynyt-ottqDRJ0?usp=sharing) |

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Proceso Gaussiano Bayesiano: Modelo Sustituto y Emulador (Simulación Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación interactiva centrada en el uso de un Proceso Gaussiano como modelo sustituto de una función costosa. Permite visualizar cómo el emulador aprende secuencialmente a partir de evaluaciones limitadas, mostrando simultáneamente la función real, la media posterior, la banda de incertidumbre y la función de adquisición. Incluye control sobre hiperparámetros como longitud de escala, varianza del kernel, ruido de observación, presupuesto experimental y criterio de adquisición, además de métricas como RMSE, incertidumbre media, mejor observación y regret. Es un recurso especialmente útil para enseñar emulación, diseño secuencial de experimentos y la lógica exploración–explotación en optimización bayesiana.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/5d4b5a6584b04d7389e3f0a25aac3c8a6a367866/src/classroom/probabilidad/html/Proceso_Gaussiano_%20Bayesiano_modelo_sustituto_emulador.html) |
| **Proceso Gaussiano Bayesiano: Optimization Simulator (Visualización Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización interactiva orientada a explicar la optimización bayesiana sobre una función unidimensional mediante un Proceso Gaussiano y funciones de adquisición como LCB y Expected Improvement. El recurso muestra la estimación posterior del GP, las bandas de confianza, el mejor punto encontrado, el siguiente experimento sugerido y el presupuesto utilizado, permitiendo ajustar parámetros como κ, ξ, la longitud de escala del kernel y el número máximo de observaciones. Su diseño enfatiza la lectura conceptual de cada paso del algoritmo y ayuda a comprender cómo la adquisición combina predicción e incertidumbre para decidir dónde evaluar después. Resulta ideal para cursos de aprendizaje estadístico, diseño adaptativo y optimización de funciones costosas.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/5d4b5a6584b04d7389e3f0a25aac3c8a6a367866/src/classroom/probabilidad/html/Proceso_Gaussiano_%20Bayesiano_optimization_simulator.html) |
| **Proceso Gaussiano Bayesiano: Evaluación Comparativa de Estrategias de Búsqueda (Lección Interactiva)** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Lección interactiva dedicada a comparar de manera rigurosa tres estrategias de búsqueda y optimización: Grid Search, Random Search y Bayesian Optimization con Proceso Gaussiano. Presenta distintos escenarios bidimensionales, como presupuestos bajos, funciones multimodales y superficies con ruido, y permite analizar cómo varía el desempeño de cada método a lo largo de las evaluaciones. Incorpora mapas del objetivo, trayectorias de exploración, visualización de la adquisición bayesiana, curvas de convergencia promedio y benchmarks sobre múltiples semillas para comparar medias, medianas, dispersión y cantidad de victorias por método. Es un material especialmente valioso para mostrar, en términos experimentales y visuales, cuándo la optimización bayesiana supera a enfoques clásicos y cuándo su ventaja depende del escenario, del presupuesto y de la adquisición elegida.</p></details> | [![Ver Simulación Interactiva](https://img.shields.io/badge/Ver%20Simulaci%C3%B3n-Interactiva-green?style=for-the-badge\&logo=blogger)](https://github.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/blob/5d4b5a6584b04d7389e3f0a25aac3c8a6a367866/src/classroom/probabilidad/html/Proceso_Gaussiano_%20Bayesiano_evaluacion.html) |

## 📝 Random Walks: estructura estocástica, recurrencia, absorción y simulación

Esta sección reúne un **cuaderno base en Google Colab** y una colección de **materiales HTML interactivos** dedicados al estudio progresivo de las **caminatas aleatorias**. El recorrido está pensado para avanzar desde la formulación elemental del *random walk* como suma de incrementos aleatorios hasta sus conexiones con problemas clásicos de probabilidad, propiedades asintóticas y dispositivos de simulación numérica.

La secuencia articula distintos niveles de análisis. En una primera instancia se introducen los fundamentos combinatorios y probabilísticos que permiten describir trayectorias, contar caminos admisibles y estudiar distribuciones asociadas. Luego se profundiza en los **momentos del proceso**, la **deriva**, la **fluctuación** y la diferencia entre crecimiento medio y dispersión. Sobre esa base se incorporan problemas estructurales centrales, como la **recurrencia**, la **transitoriedad**, el **retorno al origen**, la **ruina del jugador** y los **tiempos de parada**, mostrando cómo estas nociones se formalizan mediante probabilidades de hitting, ecuaciones en diferencias y estados absorbentes. Finalmente, el conjunto se complementa con **simuladores interactivos** que permiten contrastar teoría y experimento, explorar parámetros y fortalecer la intuición matemática mediante visualización dinámica.

<br>

### Fundamentos generales

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Cuaderno Interactivo en Google Colab**<br><br><details><summary><strong>Resumen</strong></summary><p>Cuaderno interactivo educativo que introduce el estudio de las caminatas aleatorias desde sus fundamentos teóricos e históricos en tiempo discreto, para luego desarrollar el modelo desde perspectivas probabilísticas, geométricas y estructurales. El recorrido incluye la formulación del <em>random walk</em> como suma de incrementos aleatorios, su interpretación como cadena de Markov, el análisis de propiedades como fluctuación, recurrencia, transitoriedad y tiempos de retorno, y su conexión con problemas clásicos como la ruina del jugador y los puentes aleatorios. Posteriormente, el material explora el paso al régimen continuo, mostrando la relación entre caminatas aleatorias reescaladas, procesos gaussianos y movimiento browniano, hasta culminar con herramientas de simulación computacional orientadas a fortalecer la intuición matemática mediante visualizaciones interactivas, experimentación numérica y una presentación didáctica pensada para el aprendizaje activo.</p></details> | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1B5wiZPjW-LSzt8f-dTZMe5aSjPfweTGf?usp=sharing) |
| **Random Walk · Cuestionario Académico Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Cuestionario interactivo diseñado para consolidar el estudio formal de las caminatas aleatorias mediante preguntas desarrolladas que articulan definiciones, propiedades estructurales, resultados clásicos y conexiones conceptuales con procesos gaussianos, movimiento browniano, cadenas de Markov y técnicas combinatorias. Su formato favorece tanto el repaso como la profundización teórica.</p></details> | [![Ver Cuestionario](https://img.shields.io/badge/Ver%20Cuestionario-Interactivo-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_Cuestionario.html) |
| **Random Walk · Glosario Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Glosario avanzado dedicado a los conceptos fundamentales y extensiones del <em>random walk</em>. Reúne definiciones rigurosas, intuiciones matemáticas y ejemplos concretos sobre incrementos, deriva, recurrencia, transitoriedad, tiempos de primer paso, puentes aleatorios, teoremas límite, procesos de Markov y escalamiento browniano, entre otros términos clave para el estudio moderno de las caminatas aleatorias.</p></details> | [![Ver Glosario](https://img.shields.io/badge/Ver%20Glosario-Interactivo-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk__Glosario.html) |
| **Random Walk · Laboratorio Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Laboratorio visual e interactivo que permite experimentar con múltiples manifestaciones del <em>random walk</em> a través de simulaciones, paneles temáticos y controles dinámicos. Incluye exploraciones de caminatas en una dimensión, sesgo y ruina del jugador, puentes aleatorios, caminatas en <span>\(\mathbb{Z}^2\)</span>, recorridos sobre grafos y escalamiento hacia el movimiento browniano, ofreciendo una articulación entre teoría, visualización y experimentación computacional.</p></details> | [![Ver Laboratorio](https://img.shields.io/badge/Ver%20Laboratorio-Interactivo-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk__Laboratorio.html) |

<br>

### Fundamentos combinatorios y estructura inicial

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Conteo y Probabilidad · Guía de Ejercicios**<br><br><details><summary><strong>Resumen</strong></summary><p>Material avanzado de ejercicios resueltos centrado en la dimensión combinatoria y probabilística de las caminatas aleatorias. Desarrolla temas como paridad, principio de reflexión, números de Catalán, conteo de trayectorias admisibles, esperanza, varianza y desvío estándar en el caso simétrico, integrando técnica de resolución formal con una presentación académica orientada a fortalecer el razonamiento paso a paso.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Introducci%C3%B3n%20y%20Conteo-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_Guia_Ejercicios_introducci%C3%B3n.html) |

<br>

### Momentos, deriva y comportamiento medio

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Momentos y Deriva · Guía de Ejercicios**<br><br><details><summary><strong>Resumen</strong></summary><p>Guía interactiva dedicada al estudio de la esperanza, la varianza, el desvío estándar y la deriva en caminatas aleatorias unidimensionales. El material enfatiza la diferencia entre tendencia media y dispersión, mostrando que una deriva positiva no elimina la incertidumbre y que la variabilidad sigue creciendo con el tiempo. Su estructura por ejercicios resueltos permite fijar fórmulas clave y desarrollar intuición probabilística sobre horizontes largos.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Momentos%20y%20Deriva-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random%20Walk%20%C2%B7%20Momentos%20y%20Deriva.html) |
| **Random Walk · Momentos y Deriva · Simulador Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Simulador visual orientado a explorar trayectorias de caminatas aleatorias en una dimensión con control de parámetros y cambio de temas visuales. Permite observar trayectorias simétricas y asimétricas, seguir la evolución temporal del proceso y relacionar de manera empírica el comportamiento observado con los conceptos de deriva, fluctuación y dispersión estudiados en la guía teórica.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulador%20de%20Momentos%20y%20Deriva-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random%20Walk%20%C2%B7%20Momentos%20y%20Deriva_Simulacion.html) |

<br>

### Recurrencia, transitoriedad y retorno

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Transitoriedad y Retorno · Guía de Ejercicios**<br><br><details><summary><strong>Resumen</strong></summary><p>Bloque de ejercicios resueltos dedicado a distinguir rigurosamente entre recurrencia y transitoriedad en caminatas aleatorias sobre <span>\(\mathbb{Z}\)</span>. Desarrolla la probabilidad de retorno al origen, las probabilidades de alcanzar un estado dado bajo deriva y la interpretación conceptual de los procesos recurrentes y transientes, articulando fórmulas cerradas, discusión cualitativa y consecuencias de largo plazo.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Transitoriedad%20y%20Retorno-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random%20Walk%20%C2%B7%20Transitoriedad%20y%20Retorno.html) |
| **Random Walk · Recurrencia y Transitoriedad · Simulación Comparativa**<br><br><details><summary><strong>Resumen</strong></summary><p>Visualización interactiva centrada en la comparación entre comportamiento recurrente y comportamiento transiente. El recurso permite estudiar, desde una perspectiva visual, cómo cambian las trayectorias y las probabilidades de retorno cuando varían la simetría y el sesgo del proceso, reforzando con experimentación la comprensión de uno de los contrastes estructurales más importantes del modelo.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Recurrencia%20y%20Transitoriedad-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_walk_recurrencia_Simulaci%C3%B3n_transitoriedad.html) |
| **Random Walk · Teorema de Pólya · Simulación Interactiva**<br><br><details><summary><strong>Resumen</strong></summary><p>Simulador dedicado al teorema de Pólya y al estudio del retorno al origen en caminatas aleatorias simples simétricas. Permite comparar dimensiones, estimar empíricamente probabilidades de retorno dentro de un horizonte finito, registrar pasos de simulación y explorar visualmente la diferencia fundamental entre los casos recurrentes y transientes desde una perspectiva experimental.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Teorema%20de%20P%C3%B3lya-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_Simulaci%C3%B3n_Teorema%20de%20Polya.html) |

<br>

### Ruina del jugador y procesos absorbentes

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Ruina del Jugador · Guía de Ejercicios**<br><br><details><summary><strong>Resumen</strong></summary><p>Guía de ejercicios resueltos sobre el problema clásico de la ruina del jugador. Presenta la formulación mediante ecuaciones en diferencias, las condiciones de borde asociadas a los estados absorbentes y las fórmulas cerradas para el caso simétrico y asimétrico. El material permite comprender cómo varían las probabilidades de éxito y ruina en función del capital inicial, la meta y el sesgo del juego.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Ruina%20del%20Jugador-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random%20Walk%20%C2%B7%20Ruina%20del%20Jugador_Guia%20Ejercicios.html) |
| **Random Walk · Ruina del Jugador · Simulador Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Simulador interactivo del problema de ruina del jugador modelado como cadena de Markov con dos estados absorbentes. Permite contrastar probabilidad teórica y empírica de ruina, observar tiempos de absorción, explorar la distribución de duraciones y verificar visualmente cómo influyen el capital inicial, la meta y la probabilidad de avance sobre el destino final del proceso.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulador%20de%20Ruina-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_La%20ruina%20del%20jugador_Simulacion.html) |

<br>

### Tiempos de parada y hitting times

| **📄 Recurso** | **📥 Acceso** |
| :--- | :--- |
| **Random Walk · Stopping Times · Guía de Ejercicios**<br><br><details><summary><strong>Resumen</strong></summary><p>Guía académica dedicada a los tiempos de parada en caminatas aleatorias unidimensionales. Introduce la filtración natural del proceso, la definición formal de <em>stopping time</em>, la medibilidad de los tiempos de primer arribo y la relación entre tiempos de llegada, probabilidades de hitting y deriva. El formato por ejercicios resueltos permite trabajar con precisión formal sin perder la intuición del problema.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Stopping%20Times-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_stopping_times_Guia%20Ejercicios.html) |
| **Random Walk · Stopping Times · Simulación Interactiva**<br><br><details><summary><strong>Resumen</strong></summary><p>Simulación dinámica del primer tiempo de llegada a un nivel objetivo. El recurso permite visualizar la trayectoria del caminante, identificar la primera llegada, modificar el nivel objetivo y el sesgo del proceso, y estudiar experimentalmente cómo se relacionan <em>hitting time</em>, trayectoria y probabilidad de alcance dentro de un entorno gráfico diseñado para aprendizaje visual.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir%20HTML-Simulador%20de%20Stopping%20Times-1f6feb?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Random_Walk_Stopping_times_%20Simulacion.html) |

### 🎥 Videos recomendados · Random Walks

#### 1. Introducción e intuición visual

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **¿Qué es un Random Walk?**<br><sub>*Introduce la idea de caminata aleatoria con ejemplos en finanzas, algoritmos y biología. Muy recomendable para construir intuición visual desde el comienzo.*</sub> | **Infinite Series (PBS)**<br><sub>*What is a Random Walk?*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=stgYW6M5o4k) |
| **Random Walk como metáfora de incertidumbre y progreso**<br><sub>*Charla motivacional que parte de la caminata aleatoria 1D y la conecta con la idea de avanzar en entornos inciertos. Muy útil para abrir una clase o contextualizar el tema.*</sub> | **TEDx St. Gilgen International School**<br><sub>*Random walking*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=-yDTUE-QVno) |

#### 2. Desarrollo formal y enfoque universitario

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Introducción formal a los Random Walks**<br><sub>*Presentación más técnica del modelo, enlazándolo con procesos en física y finanzas. Ideal para pasar de la intuición a una formulación más rigurosa.*</sub> | **Complexity Explorer / Santa Fe Institute**<br><sub>*Random Walks Tutorial: Introduction*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ilwEHzovpJk) |
| **Simulación y análisis probabilístico del Random Walk**<br><sub>*Clase de MIT donde se simulan caminatas aleatorias y se estudian propiedades como la distancia al origen, articulando teoría probabilística y experimentación computacional.*</sub> | **MIT OpenCourseWare**<br><sub>*5. Random Walks*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=6wUD_gp5WeE) |

#### 3. Escalamiento, difusión y movimiento browniano

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Del Random Walk al Movimiento Browniano**<br><sub>*Explica cómo la caminata aleatoria se relaciona con la difusión y el movimiento browniano, mostrando el paso desde el modelo discreto hacia su límite continuo.*</sub> | **Complexity Explorer / Santa Fe Institute**<br><sub>*Random Walks Tutorial: Brownian Motion*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=89LP5pHWxM8) |

#### 4. Conexiones con econometría y series de tiempo

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Random Walk y Series de Tiempo**<br><sub>*Presenta la caminata aleatoria como caso particular de un modelo AR(1) con \(\rho = 1\), muy útil para conectar el tema con econometría y análisis de series temporales.*</sub> | **Ben Lambert**<br><sub>*A Random Walk – introduction and properties*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ouahL4HbwBE) |

#### 5. Código, simulación y aplicaciones

| 🎬 Tema y Concepto Clave | 👨‍🏫 Canal / Autor | 🔗 Enlace |
| :--- | :--- | :--- |
| **Código y visualización de un Random Walk simple**<br><sub>*Video breve centrado en programación y visualización de una caminata aleatoria simple. Útil como complemento práctico para simulaciones básicas.*</sub> | **YouTube / Recurso de programación**<br><sub>*Simple Random Walk*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ZZcne16szFM) |
| **Aplicaciones del Random Walk**<br><sub>*Lección dedicada a aplicaciones en física, juegos de azar y finanzas, con simulaciones y ejemplos computacionales que permiten vincular teoría y práctica.*</sub> | **YouTube / Lección aplicada**<br><sub>*14. Random Walk Applications*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=aDmFbsBp_u4) |
## Proceso browniano

Visualización generativa de movimiento browniano, inspirada en la dispersión aleatoria de partículas y en la forma global de una distribución gaussiana en tres dimensiones.

<p align="center">
  <img src="https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/d7d3a421873972291756a245ee82bc18bc39a5c1/src/classroom/probabilidad/images/movimiento_browniano_liviano.gif" alt="Visualización científica de un proceso browniano" width="1000">
</p>

<sub>Prompt de generación: “Scientific visualization of Brownian motion: thousands of glowing particles drifting randomly in dark space, leaving light trails forming a 3D Gaussian bell curve distribution. Color gradient from deep blue to bright white-gold. Camera slowly zooming out. 4K, scientific aesthetic, dark background”.</sub>

# 🌊 Movimiento Browniano, Proceso de Wiener y Cálculo de Itô
## Ruta interactiva para estudiar procesos estocásticos, difusión, finanzas cuantitativas e IA generativa

> Esta versión 2.0 reorganiza el material como una **ruta de aprendizaje progresiva**. El objetivo no es solo listar recursos, sino mostrar cómo cada notebook, simulación, video, cuestionario y glosario cumple una función dentro del estudio del movimiento browniano: desde la intuición física de partículas en movimiento hasta el cálculo de Itô, los modelos financieros, los procesos con reversión a la media y las ideas modernas detrás de los modelos generativos por difusión.

<p align="center">
  <img src="https://img.shields.io/badge/Tema-Movimiento%20Browniano-0B7285?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Proceso-Wiener-364FC7?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Cálculo-Itô-7B2CBF?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Aplicaciones-Finanzas%20%7C%20Difusión%20%7C%20IA-2F9E44?style=for-the-badge" />
</p>

---

## 🧭 Cómo leer este módulo

El recorrido está pensado como una escalera conceptual. Primero se observa el fenómeno, luego se simula, después se formaliza matemáticamente y finalmente se conecta con aplicaciones avanzadas.

| Etapa | Pregunta guía | Recurso central | Resultado esperado |
| :---: | :--- | :--- | :--- |
| **1** | ¿Qué fenómeno físico dio origen al movimiento browniano? | Videos introductorios y demostraciones experimentales | Comprender la intuición física: partículas erráticas, choques microscópicos y evidencia indirecta del mundo atómico. |
| **2** | ¿Cómo se pasa de una caminata aleatoria discreta a un proceso continuo? | Videos sobre random walk y simulación 1D | Entender el browniano como límite escalado de caminatas aleatorias. |
| **3** | ¿Cómo se define formalmente el proceso de Wiener? | Notebook principal + simulaciones iniciales | Identificar incrementos gaussianos, independencia, continuidad y distribución normal. |
| **4** | ¿Qué significa difusión? | Histograma dinámico, nube 2D y mapa de calor | Ver cómo trayectorias individuales erráticas producen una distribución agregada regular. |
| **5** | ¿Qué propiedades hacen especial al browniano? | Autosimilaridad, tiempo de llegada y variación cuadrática | Comprender autosimilaridad, hitting time y rugosidad extrema de las trayectorias. |
| **6** | ¿Por qué aparece el cálculo de Itô? | Variación cuadrática e integral de Itô | Diferenciar integrar respecto de `dt` e integrar respecto de `dW_t`. |
| **7** | ¿Cómo se modelan precios y sistemas con tendencia de retorno? | Browniano geométrico y Ornstein–Uhlenbeck | Conectar SDEs con finanzas, señales, física y modelos de reversión a la media. |
| **8** | ¿Cómo conecta esto con IA generativa? | Difusión forward y reverse diffusion | Entender cómo el ruido gaussiano y su reversión inspiran modelos generativos modernos. |
| **9** | ¿Cómo consolidar el aprendizaje? | Cuestionario y glosario | Repasar definiciones, fórmulas, intuiciones y aplicaciones. |

---

## 🧠 Mapa conceptual general

```text
Movimiento Browniano
│
├── Origen físico e histórico
│   ├── Robert Brown
│   ├── Einstein
│   ├── evidencia del mundo atómico
│   └── partículas en suspensión
│
├── Construcción probabilística
│   ├── caminata aleatoria
│   ├── Teorema Central del Límite
│   ├── proceso de Wiener
│   ├── incrementos gaussianos independientes
│   └── continuidad de trayectorias
│
├── Difusión y distribución
│   ├── X(t) ~ N(0, σ²t)
│   ├── ecuación del calor
│   ├── nube de partículas
│   └── mapa de calor
│
├── Propiedades avanzadas
│   ├── autosimilaridad
│   ├── tiempos de llegada
│   ├── martingalas
│   ├── variación cuadrática
│   └── cálculo de Itô
│
└── Aplicaciones
    ├── finanzas cuantitativas
    ├── movimiento browniano geométrico
    ├── Ornstein–Uhlenbeck
    ├── difusión forward
    └── modelos generativos por difusión
```

---

## 📌 Fórmulas mínimas para orientar el recorrido

| Concepto | Fórmula orientativa | Lectura conceptual |
| :--- | :--- | :--- |
| **Incremento browniano** | `ΔW = sqrt(Δt) · Z`, con `Z ~ N(0,1)` | Cada pequeño paso aleatorio se escala con la raíz del tiempo. |
| **Distribución marginal** | `W_t ~ N(0,t)` | En un tiempo mayor, la dispersión aumenta. |
| **Incrementos independientes** | `W_t - W_s ~ N(0,t-s)` | El cambio futuro no depende del pasado, sino del intervalo temporal. |
| **Difusión con volatilidad** | `X(t) ~ N(0, σ²t)` | La varianza crece linealmente con el tiempo. |
| **Variación cuadrática** | `[W]_t = t` | Aunque la trayectoria es continua, es extremadamente irregular. |
| **Regla informal de Itô** | `(dW_t)^2 = dt` | La rugosidad del browniano cambia las reglas del cálculo clásico. |
| **Browniano geométrico** | `dS_t = μS_tdt + σS_tdW_t` | Modelo clásico para precios positivos con crecimiento y volatilidad. |
| **Ornstein–Uhlenbeck** | `dX_t = θ(μ - X_t)dt + σdW_t` | Modelo con ruido y retorno hacia una media de largo plazo. |

---

# 📘 Bloque 1 · Recurso eje del módulo

| Recurso | Nivel | Función dentro del módulo | Acceso |
| :--- | :---: | :--- | :---: |
| **Notebook: Procesos Estocásticos Gaussianos y Brownianos – De la Teoría Clásica a la IA Generativa**<br><br><details><summary><strong>Resumen desarrollado</strong></summary><p>Este notebook funciona como el eje conceptual del módulo. Presenta un recorrido profundo desde los fundamentos de los procesos estocásticos gaussianos y brownianos hasta sus conexiones con la inteligencia artificial generativa. Desarrolla procesos de Lévy, procesos de Markov, martingalas, movimiento browniano, cálculo de Itô, geometría de alta dimensión, transporte óptimo y distancia de Wasserstein. El recorrido culmina con una explicación técnica de los modelos de difusión generativos, mostrando cómo la inyección progresiva de ruido gaussiano y su reversión mediante una función de score constituyen una de las bases matemáticas de arquitecturas modernas de generación de contenido.</p></details> | 🔴 Avanzado | Usarlo como material de referencia general. Conviene volver a este notebook después de recorrer las simulaciones, porque muchas ideas visuales se formalizan allí. | [![Abrir Notebook](https://img.shields.io/badge/Colab-Abrir%20Notebook-orange?style=for-the-badge&logo=google-colab)](https://colab.research.google.com/drive/19IY4zqBi-qzm0cn1zXIQGfI9ywc7UzKX#scrollTo=89P_lF0kFckG) |

---

# 🧪 Bloque 2 · Simulaciones interactivas principales

## 2.1 De la trayectoria individual a la distribución agregada

| Orden | Recurso | Nivel | Qué muestra | Uso pedagógico | Acceso |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **1** | **Movimiento browniano en una dimensión**<br><br><details><summary><strong>Resumen</strong></summary><p>Introduce el movimiento browniano en una dimensión como una trayectoria aleatoria construida a partir de incrementos gaussianos independientes. La simulación permite observar cómo se forma una trayectoria browniana a medida que avanza el tiempo, conectando la idea de proceso continuo con su aproximación discreta. Presenta la noción de trayectoria <code>W_t</code>, los incrementos <code>ΔW_i</code>, la relación con el tiempo y la interpretación del browniano como límite continuo de un paseo aleatorio.</p></details> | 🟢 Inicial | Una trayectoria `W_t` que evoluciona con saltos pequeños y aleatorios. | Primer recurso para mostrar que el browniano no es una función suave, sino una trayectoria continua pero rugosa. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/movimiento_browniano_simulacion_1%20D.html) |
| **2** | **Muchas partículas brownianas e histograma dinámico**<br><br><details><summary><strong>Resumen</strong></summary><p>Muestra muchas partículas brownianas moviéndose en una dimensión junto con un histograma dinámico de sus posiciones. La simulación permite ver cómo, detrás de trayectorias individuales erráticas, emerge una distribución normal agregada. La teoría explica que <code>X(t) ~ N(0, σ²t)</code>, que la dispersión crece con el tiempo y que la evolución de la densidad puede interpretarse en relación con la ecuación del calor.</p></details> | 🟢 Inicial / 🟡 Intermedio | Muchas trayectorias individuales y su distribución colectiva. | Excelente para conectar azar microscópico con regularidad estadística macroscópica. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Brownianohistograma_browniano_particulas.html) |
| **3** | **Movimiento browniano en 2D: nube de partículas y mapa de calor**<br><br><details><summary><strong>Resumen</strong></summary><p>Presenta el movimiento browniano en dos dimensiones mediante una nube de partículas y un mapa de calor. La simulación permite observar la difusión espacial en el plano y visualizar cómo la nube se expande radialmente con el tiempo. La teoría muestra que el browniano bidimensional se construye con dos componentes brownianas independientes y que <code>W_t ~ N(0, tI₂)</code>, lo cual permite interpretar la geometría probabilística de la expansión.</p></details> | 🟡 Intermedio | Difusión espacial en el plano, nube de partículas y concentración de probabilidad. | Ideal para visualizar que el browniano puede pensarse como proceso vectorial, no solo como una curva en una dimensión. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_2d_nube_mapa_calor.html) |

---

## 2.2 Propiedades estructurales del movimiento browniano

| Orden | Recurso | Nivel | Qué muestra | Uso pedagógico | Acceso |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **4** | **Autosimilaridad del movimiento browniano**<br><br><details><summary><strong>Resumen</strong></summary><p>Trabaja una de las propiedades más importantes del movimiento browniano: la autosimilaridad. La simulación muestra una trayectoria completa, selecciona un fragmento pequeño y lo reescala para compararlo con el proceso original. Permite observar la relación de escala <code>{W_{ct}} ≍ sqrt(c)W_t</code>, mostrando que el browniano conserva su forma estadística bajo transformaciones temporales y espaciales adecuadas.</p></details> | 🟡 Intermedio | Un fragmento de la trayectoria puede ampliarse y conservar una estructura estadística semejante. | Útil para explicar por qué las trayectorias brownianas tienen apariencia fractal y no derivable. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_autosimilaridad_html.html) |
| **5** | **Tiempo de llegada a una barrera**<br><br><details><summary><strong>Resumen</strong></summary><p>Simula el primer tiempo en que una trayectoria browniana alcanza una barrera. Permite estudiar el concepto de hitting time o first passage time, muy importante en finanzas, física, biología y teoría de procesos estocásticos. El recurso ayuda a comprender que no solo interesa la posición del proceso en un tiempo fijo, sino también el momento aleatorio en que se alcanza determinado umbral.</p></details> | 🟡 Intermedio | El instante aleatorio en que una trayectoria toca por primera vez una barrera. | Recurso clave para discutir riesgo, umbrales, defaults, absorción y eventos extremos. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_tiempo_llegada_barrera.html) |
| **6** | **Variación cuadrática y cálculo de Itô**<br><br><details><summary><strong>Resumen</strong></summary><p>Explica la variación cuadrática del movimiento browniano, una propiedad central que lo diferencia de las funciones suaves del cálculo clásico. La simulación muestra cómo la suma de los cuadrados de los incrementos se aproxima al tiempo total, es decir, <code>Σ(ΔW_i)² ≈ T</code>. Esta propiedad es la base intuitiva de la regla informal <code>(dW_t)² = dt</code>, fundamental para comprender el cálculo de Itô.</p></details> | 🔴 Avanzado | La suma de incrementos cuadrados converge al tiempo. | Es el puente conceptual entre trayectoria rugosa y cálculo estocástico. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_variacion_cuadratica_ito.html) |
| **7** | **Integral de Itô: integrar contra dWₜ versus integrar contra dt**<br><br><details><summary><strong>Resumen</strong></summary><p>Compara una integral ordinaria respecto del tiempo con una integral estocástica respecto de <code>dW_t</code>. Muestra que integrar contra una señal browniana no equivale a integrar contra una variable temporal regular. El recurso permite visualizar por qué el cálculo de Itô requiere reglas propias y por qué aparece una corrección adicional respecto del cálculo clásico.</p></details> | 🔴 Avanzado | Diferencia entre acumulación temporal regular e integración contra ruido browniano. | Recomendado después de variación cuadrática, porque muestra la consecuencia operacional de esa propiedad. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_integral_ito_dwt_vs_dt.html) |

---

## 2.3 Modelos estocásticos aplicados

| Orden | Recurso | Nivel | Qué muestra | Uso pedagógico | Acceso |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **8** | **Movimiento browniano geométrico**<br><br><details><summary><strong>Resumen</strong></summary><p>Presenta el movimiento browniano geométrico, ampliamente utilizado para modelar precios financieros positivos. La simulación permite modificar parámetros como deriva y volatilidad para observar trayectorias de precios simuladas. Este recurso conecta el movimiento browniano con ecuaciones diferenciales estocásticas y con el modelo de Black-Scholes, donde la dinámica típica puede escribirse como <code>dS_t = μS_tdt + σS_tdW_t</code>.</p></details> | 🟡 Intermedio / 🔴 Avanzado | Trayectorias positivas con tendencia y volatilidad proporcional. | Ideal para explicar por qué en finanzas suele modelarse el logaritmo del precio con browniano y no el precio directamente con un browniano simple. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_geometrico.html) |
| **9** | **Reversión a la media: proceso de Ornstein–Uhlenbeck**<br><br><details><summary><strong>Resumen</strong></summary><p>Simula el proceso de Ornstein–Uhlenbeck, un proceso estocástico con ruido browniano y fuerza de retorno hacia una media de largo plazo. Permite observar cómo el proceso fluctúa aleatoriamente, pero tiende a regresar hacia un nivel central. Es útil para modelar tasas de interés, señales físicas, velocidades de partículas, series temporales con equilibrio y fenómenos con estabilización dinámica.</p></details> | 🟡 Intermedio / 🔴 Avanzado | Ruido más fuerza de retorno hacia una media. | Permite comparar procesos puramente difusivos con procesos que tienen estructura de equilibrio. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_reversion_media_ornstein_uhlenbeck.html) |

---

## 2.4 Movimiento browniano e inteligencia artificial generativa

| Orden | Recurso | Nivel | Qué muestra | Uso pedagógico | Acceso |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **10** | **Difusión forward para modelos generativos**<br><br><details><summary><strong>Resumen</strong></summary><p>Conecta el movimiento browniano con los modelos generativos modernos de inteligencia artificial. La simulación muestra cómo una señal o conjunto de datos puede contaminarse progresivamente con ruido gaussiano hasta perder su estructura original. Este proceso forward es una analogía visual de la etapa de difusión utilizada en modelos generativos, donde los datos son transformados gradualmente en ruido.</p></details> | 🔴 Avanzado | Agregado progresivo de ruido gaussiano sobre datos. | Excelente para conectar probabilidad, SDEs e IA generativa de manera visual. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_difusion_forward_modelos_generativos.html) |
| **11** | **Reverse diffusion conceptual: de ruido a datos**<br><br><details><summary><strong>Resumen</strong></summary><p>Presenta de forma conceptual el proceso inverso de difusión. La simulación muestra cómo una estructura puede recuperarse progresivamente desde ruido, reforzando la intuición detrás de los modelos generativos por difusión. Aunque no implementa un modelo neuronal completo, funciona como puente visual para comprender por qué aprender a revertir el ruido permite generar datos nuevos.</p></details> | 🔴 Avanzado | Reconstrucción conceptual desde ruido hacia estructura. | Recurso de cierre para mostrar cómo el browniano aparece detrás de una de las familias más importantes de modelos generativos modernos. | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_reverse_diffusion_conceptual.html) |

---

# 🎥 Bloque 3 · Material audiovisual complementario

> Esta curaduría de videos acompaña el aprendizaje desde tres ángulos: historia física, construcción matemática y aplicaciones. Puede utilizarse antes de las simulaciones para abrir la intuición o después de ellas para profundizar conceptos.

## 3.1 Intuición física e histórica

| Orden | Video | Nivel | Concepto central | Uso recomendado | Enlace |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **1** | **Movimiento Browniano como física de la aleatoriedad**<br><sub>Introducción divulgativa para abrir el tema. Presenta la historia de Einstein, la evidencia de la existencia de los átomos, trayectorias fractales y aplicaciones en finanzas.</sub> | 🟢 Inicial | Física de la aleatoriedad | Usarlo como apertura general del módulo. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=5jBVYvHeG2c) |
| **2** | **El experimento que reveló el mundo atómico**<br><sub>Motivación física altamente visual. Muestra el fenómeno con modelos reales y microscopio, ideal antes de formalizar el concepto matemáticamente.</sub> | 🟢 Inicial | Evidencia experimental | Usarlo para mostrar que la matemática surge de un fenómeno observable. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ZNzoTGv_XiQ) |
| **3** | **Einstein y la existencia de los átomos**<br><sub>Mini-clip ideal como gancho inicial. Explica en pocos minutos cómo el Movimiento Browniano permitió aportar evidencia indirecta sobre la existencia de los átomos.</sub> | 🟢 Inicial | Einstein y mundo atómico | Ideal como introducción breve antes de una clase o post. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=nrUBPO6zZ40) |
| **4** | **La danza caótica que probó que los átomos existen**<br><sub>Video divulgativo con énfasis en historia, difusión, geometría fractal de trayectorias y aplicaciones en física, biología y finanzas.</sub> | 🟢 Inicial / 🟡 Intermedio | Historia, difusión y aplicaciones | Útil para conectar narrativa histórica con aplicaciones modernas. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=HJ92U37seBA) |
| **5** | **Historia, visualización y primeras propiedades matemáticas**<br><sub>Conecta la historia de Brown, Einstein y Wiener con visualizaciones de trayectorias y propiedades básicas del proceso browniano.</sub> | 🟡 Intermedio | Historia y primeras propiedades | Conviene verlo después de las primeras simulaciones 1D. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=6EHzu-nyTyk) |

## 3.2 Del random walk al proceso de Wiener

| Orden | Video | Nivel | Concepto central | Uso recomendado | Enlace |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **6** | **De la caminata aleatoria al Movimiento Browniano**<br><sub>Explica cómo una caminata aleatoria discreta puede converger hacia el Movimiento Browniano. Es clave para comprender el paso de lo discreto a lo continuo.</sub> | 🟡 Intermedio | Límite de caminatas aleatorias | Usarlo para explicar que el browniano puede verse como límite continuo de procesos discretos. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=7wBqiOR90UQ) |
| **7** | **Caminatas aleatorias, Teorema Central del Límite y Browniano**<br><sub>Serie que permite conectar caminatas aleatorias, Teorema Central del Límite, distribución normal multivariada, Movimiento Browniano y aplicaciones financieras.</sub> | 🟡 Intermedio | CLT y escalamiento | Excelente puente entre estadística clásica y procesos estocásticos. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=BUJCF900I0A) |
| **8** | **Derivación formal del Movimiento Browniano**<br><sub>Clase sistemática que parte de la caminata aleatoria de un paso y avanza hacia la definición y propiedades del Movimiento Browniano.</sub> | 🔴 Avanzado | Derivación formal | Recomendado para estudiantes que ya manejan probabilidad y quieren formalización. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=6iRY8N7WZr4) |

## 3.3 Cálculo estocástico, propiedades avanzadas y aplicaciones

| Orden | Video | Nivel | Concepto central | Uso recomendado | Enlace |
| :---: | :--- | :---: | :--- | :--- | :---: |
| **9** | **Proceso Browniano formal: Markov, incrementos y variación cuadrática**<br><sub>Clase universitaria avanzada sobre procesos estocásticos. Incluye propiedad de Markov, incrementos independientes, variación cuadrática, principio de reflexión y resultados fundamentales.</sub> | 🔴 Avanzado | Markov, incrementos y variación cuadrática | Usarlo junto con las simulaciones de variación cuadrática y tiempo de llegada. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=VM29JyI1sio) |
| **10** | **Cálculo de Itô y variación cuadrática**<br><sub>Clase avanzada para conectar Movimiento Browniano con cálculo estocástico. Trabaja la idea fundamental de variación cuadrática, la regla informal dB² = dt, Black-Scholes y el proceso de Ornstein–Uhlenbeck.</sub> | 🔴 Avanzado | Itô, Black-Scholes y SDEs | Usarlo como recurso de profundización para cálculo de Itô y modelos financieros. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=Z5yRMMVUC5w) |
| **11** | **Aplicaciones del Movimiento Browniano**<br><sub>Recorrido por aplicaciones en física, finanzas, biología, ingeniería y ciencia de datos. Ideal como cierre integrador del tema.</sub> | 🟡 Intermedio | Aplicaciones interdisciplinarias | Recomendado para cerrar la unidad y conectar con casos reales. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=Ajezz2nuqiw) |
| **12** | **Simulación computacional del Movimiento Browniano**<br><sub>Video práctico para mostrar cómo simular Movimiento Browniano mediante distancias normalmente distribuidas y ángulos uniformes.</sub> | 🟡 Intermedio | Simulación computacional | Útil para complementar el trabajo con HTML, Python o notebooks. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=3KcRVfqHqRk) |
| **13** | **Demostración experimental del fenómeno browniano**<br><sub>Demostración real con microscopio y partículas de humo. Útil para mostrar el fenómeno físico directamente antes o después de la formalización matemática.</sub> | 🟢 Inicial | Observación experimental | Recurso breve para recordar que el browniano nace de un fenómeno físico observable. | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=gPMVaAnij88) |

---

# 🧩 Bloque 4 · Recursos de consolidación

| Recurso | Nivel | Función | Acceso |
| :--- | :---: | :--- | :---: |
| **Movimiento Browniano · Guía Visual y Cuestionario Interactivo 2.0**<br><br><details><summary><strong>Resumen</strong></summary><p>Guía interactiva avanzada para estudiar movimiento browniano de manera progresiva, visual y didáctica. Integra 30 preguntas desarrolladas con respuestas explicativas, fórmulas estables en HTML, mapa conceptual, simulación de trayectorias brownianas, histograma de posiciones finales, laboratorio de variación cuadrática y glosario mínimo previo al cuestionario. El recorrido conecta caminatas aleatorias, proceso de Wiener, incrementos gaussianos, continuidad y no derivabilidad, variación cuadrática, cálculo de Itô, ecuaciones diferenciales estocásticas, movimiento browniano geométrico, Ornstein–Uhlenbeck, difusión, Fokker–Planck, Langevin y modelos generativos de inteligencia artificial. Es recomendable utilizarlo como cuestionario adicional de consolidación profunda, especialmente después de haber trabajado las simulaciones principales y antes de cerrar el bloque con el glosario general.</p></details> | 🟢🟡🔴 Progresivo | Consolidar comprensión teórica, visual y aplicada mediante preguntas desarrolladas, simulaciones y lectura guiada. | [![Ver Guía 2.0](https://img.shields.io/badge/Ver%20Gu%C3%ADa%202.0-Interactiva-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_Cuestionario.html) |
| **Movimiento Browniano · Cuestionario Académico Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Cuestionario interactivo diseñado para consolidar el estudio del movimiento browniano desde una perspectiva progresiva. Permite repasar fundamentos físicos, proceso de Wiener, incrementos gaussianos, difusión, variación cuadrática, cálculo de Itô, movimiento browniano geométrico, Ornstein–Uhlenbeck, difusión generativa y aplicaciones. Es recomendable utilizarlo como cierre evaluativo luego de recorrer las simulaciones principales.</p></details> | 🟢🟡🔴 Progresivo | Evaluar comprensión conceptual y técnica. | [![Ver Cuestionario](https://img.shields.io/badge/Ver%20Cuestionario-Interactivo-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_Cuestionario.html) |
| **Movimiento Browniano · Glosario Interactivo**<br><br><details><summary><strong>Resumen</strong></summary><p>Glosario académico avanzado dedicado al movimiento browniano, el proceso de Wiener y el cálculo estocástico. Reúne 39 términos clave con definiciones desarrolladas, fórmulas, intuiciones geométricas y ejemplos concretos sobre difusión anómala, puente browniano, caminata aleatoria, coeficiente de difusión, covarianza, ecuación de difusión, Fokker-Planck, Langevin, SDE, filtración, movimiento browniano fraccionario, movimiento browniano geométrico, procesos gaussianos, índice de Hurst, integral y lema de Itô, martingalas, propiedad de Markov, ruido blanco, Ornstein-Uhlenbeck, principio de reflexión, autosimilaridad, teorema de Donsker, tiempos de parada y variación cuadrática.</p></details> | 🟢🟡🔴 Progresivo | Servir como diccionario técnico y guía de repaso. | [![Ver Glosario](https://img.shields.io/badge/Ver%20Glosario-Interactivo-2ea44f?style=for-the-badge)](https://sgevatschnaider.github.io/estadisticas-para-ciencia-de-datos/src/classroom/probabilidad/html/Movimiento_Browniano_Glosario.html) |
---

# 📊 Tabla de síntesis conceptual

| Bloque | Qué se aprende | Conceptos clave | Conexión con ciencia de datos e IA |
| :--- | :--- | :--- | :--- |
| **Fenómeno físico** | El movimiento irregular de partículas surge de choques microscópicos. | Brown, Einstein, partículas, mundo atómico. | Permite entender cómo un fenómeno observable motiva un modelo probabilístico. |
| **Caminata aleatoria** | Un proceso discreto puede aproximar un proceso continuo al escalar tiempo y espacio. | Random walk, CLT, convergencia, Donsker. | Base de simulaciones Monte Carlo y modelos discretos aproximados. |
| **Proceso de Wiener** | El browniano formal tiene incrementos gaussianos independientes y trayectorias continuas. | `W_t`, incrementos, normalidad, independencia. | Modelo base para ruido, señales, series temporales y SDEs. |
| **Difusión** | El azar individual produce regularidad colectiva. | Densidad normal, ecuación del calor, mapa de calor. | Aparece en física, biología, dinámica de partículas e IA generativa. |
| **Variación cuadrática** | La trayectoria es continua, pero no suave. | `[W]_t = t`, rugosidad, no derivabilidad. | Justifica el cálculo estocástico y las reglas de Itô. |
| **Cálculo de Itô** | Integrar contra ruido requiere reglas diferentes al cálculo clásico. | `dW_t`, `dt`, lema de Itô, SDE. | Base de modelos financieros, filtros, control estocástico y procesos generativos. |
| **Modelos aplicados** | Se pueden construir procesos con tendencia, volatilidad o reversión. | GBM, OU, deriva, volatilidad. | Finanzas cuantitativas, series temporales, física estadística y señales. |
| **Modelos de difusión** | El ruido puede agregarse y luego aprenderse a revertir. | Forward diffusion, reverse diffusion, score. | Fundamento conceptual de modelos generativos modernos. |

---

# 🧪 Secuencia sugerida para una clase o repositorio

1. **Abrir con una demostración física** del movimiento browniano para instalar la pregunta: ¿por qué una partícula se mueve de manera errática?
2. **Mostrar la simulación 1D** para construir una trayectoria desde incrementos gaussianos.
3. **Pasar al histograma dinámico** para mostrar que muchas trayectorias producen una distribución normal.
4. **Extender a 2D** con nube de partículas y mapa de calor para visualizar difusión espacial.
5. **Trabajar autosimilaridad** para conectar browniano con fractalidad y escalamiento.
6. **Introducir tiempos de llegada** para estudiar umbrales y eventos aleatorios.
7. **Explicar variación cuadrática** como el punto de quiebre con el cálculo clásico.
8. **Entrar al cálculo de Itô** mostrando la diferencia entre `dt` y `dW_t`.
9. **Aplicar a modelos concretos**: browniano geométrico y Ornstein–Uhlenbeck.
10. **Cerrar con IA generativa**, explicando difusión forward y reverse diffusion.
11. **Evaluar con el cuestionario** y reforzar con el glosario.

---

# ✅ Ideas clave para recordar

- El movimiento browniano es un modelo matemático para trayectorias continuas, aleatorias y altamente irregulares.
- Su construcción puede entenderse como límite de caminatas aleatorias bajo un escalamiento adecuado.
- Sus incrementos son gaussianos, independientes y con varianza proporcional al tiempo transcurrido.
- La distribución agregada de muchas partículas brownianas se vuelve regular, aunque cada trayectoria individual sea errática.
- La variación cuadrática del browniano no es cero: es igual al tiempo, y esa propiedad explica por qué el cálculo de Itô no coincide con el cálculo clásico.
- El movimiento browniano geométrico permite modelar variables positivas con crecimiento y volatilidad, como precios financieros idealizados.
- El proceso de Ornstein–Uhlenbeck combina ruido con retorno hacia una media, por eso es útil para series con equilibrio dinámico.
- Los modelos generativos por difusión pueden entenderse, conceptualmente, como procesos que agregan ruido de manera progresiva y luego aprenden a revertirlo.

---

## Geometría Hiperbólica, Grafos e Inteligencia Artificial 

<div align="center">

<img src="https://raw.githubusercontent.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/29fb87a575bc09783ba3c6e2d0617231ef3f5d6d/src/classroom/graphs/recursos/teselado.gif" alt="Teselado hiperbólico en el disco de Poincaré" width="100%">

</div>

<br>

### Embeddings Hiperbólicos y Teoría de Grafos

Esta sección reúne una serie de recursos interactivos para estudiar la relación entre **geometría hiperbólica, teoría de grafos y embeddings**. El recorrido parte de la visualización del plano hiperbólico y del disco de Poincaré, avanza hacia teselaciones, bolas métricas y grafos conexos no ponderados, y finalmente conecta estas ideas con embeddings dinámicos, tipos de representaciones y análisis de distorsión.

| 📄 Recurso | 📥 Acceso |
|---|---|
| **El Problema del Embedding: Geometría Hiperbólica y Jerarquías** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Un recorrido exhaustivo de 6 módulos sobre la representación de jerarquías y grafos en espacios continuos. Aborda el <em>mismatch</em> geométrico del espacio euclidiano frente al crecimiento exponencial de los árboles, introduciendo la <strong>Geometría Hiperbólica</strong> y la <strong>Bola de Poincaré</strong> como una solución estructural natural. Incluye optimización riemanniana, enfoques constructivos con garantías de baja distorsión, trade-offs numéricos y aplicaciones en taxonomías, link prediction y redes filogenéticas.</p></details> | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WDxb8kUw6F6HJ6hJG1s0zGCz6YaE-ksU?usp=sharing) <br><br> [![Ver Lección Interactiva](https://img.shields.io/badge/Ver%20Lección-Interactiva-9cf?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/5eff3f62f4b8f22d48d610183af72e47438d4ca6/src/classroom/graphs/recursos/arbol_hiperbolico.html) |

## Mapa general del recorrido

| Etapa | Eje conceptual | Objetivo de aprendizaje |
|---|---|---|
| **1** | Fundamentos visuales de geometría hiperbólica | Construir intuición sobre curvatura negativa, disco de Poincaré, modelos y teselaciones. |
| **2** | Crecimiento, árboles y bolas métricas | Comprender por qué la geometría hiperbólica representa bien jerarquías y grafos ramificados. |
| **3** | Grafos como espacios métricos | Pasar de vértices y aristas a distancia, caminos mínimos, conectividad y estructura métrica. |
| **4** | Embeddings y distorsión | Entender cómo un grafo, texto o imagen puede representarse como puntos en un espacio geométrico. |
| **5** | Laplaciano y señales sobre grafos | Conectar grafos con álgebra lineal, energía, difusión, consenso y clustering espectral. |
| **6** | Optimización geométrica | Comparar GD, SGD y RSGD, y ver por qué la geometría del espacio modifica el entrenamiento. |
| **7** | Integración con IA | Relacionar grafos, embeddings, GNN, GraphRAG, jerarquías, sistemas dinámicos y modelos semánticos. |
| **8** | Consolidación | Usar el glosario y el cuestionario como cierre de estudio, repaso y preparación de clase. |

---

# 1. Fundamentos visuales de geometría hiperbólica

Esta primera etapa desarrolla la intuición geométrica necesaria antes de hablar de grafos, embeddings u optimización. La prioridad es comprender que el espacio hiperbólico no se comporta como el plano euclidiano: las distancias se deforman, el borde del disco concentra una enorme cantidad de espacio métrico y el crecimiento es mucho más rápido que en geometría plana.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **1. Visualización del plano hiperbólico** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Introducción visual al plano hiperbólico y a sus diferencias con la geometría euclidiana. La visualización permite observar cómo se comportan las distancias, las curvas, las deformaciones y la estructura del espacio cuando la curvatura es negativa. Es el primer recurso recomendado porque permite construir intuición geométrica antes de avanzar hacia modelos, grafos, embeddings y optimización.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Interactivo-9cf?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Visualizaci%C3%B3n%20del%20plano%20hiperb%C3%B3lico.html) |
| **2. Disco de Poincaré** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización interactiva del <strong>modelo del disco de Poincaré</strong>, uno de los modelos más utilizados para representar la geometría hiperbólica. Permite comprender cómo todo el plano hiperbólico puede proyectarse dentro de un disco euclidiano finito, donde las distancias reales se expanden hacia el borde y las geodésicas aparecen como diámetros o arcos ortogonales a la frontera.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Disco%20de%20Poincar%C3%A9-9cf?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Disco%20de%20Poincar%C3%A9.html) |
| **3. Modelos de representación del espacio hiperbólico** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Lección interactiva dedicada a comparar distintos modelos de representación del espacio hiperbólico, incluyendo el disco de Poincaré, el modelo de Beltrami-Klein, el semiplano superior, el hiperboloide y la pseudoesfera. Resulta útil ubicar este recurso después del disco de Poincaré porque permite entender que la geometría hiperbólica no se visualiza de una única manera, sino a través de modelos equivalentes que preservan propiedades distintas.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Modelos%20hiperb%C3%B3licos-9cf?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_modelos_hiperbolicos_v_2_html.html) |
| **4. Teselación estilo disco de Poincaré** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Recurso visual que muestra una teselación inspirada en el disco de Poincaré. Permite observar cómo patrones repetidos pueden cubrir el espacio hiperbólico de manera diferente a una teselación euclidiana. Ayuda a consolidar la intuición sobre curvatura negativa, expansión hacia el borde, simetría hiperbólica y repetición geométrica en espacios no euclidianos.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Teselaci%C3%B3n-9cf?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Teselaci%C3%B3n%20estilo%20disco%20de%20Poincar%C3%A9.html) |

---

# 2. Crecimiento, árboles y bolas métricas

Esta etapa explica el punto central que justifica el uso de geometría hiperbólica en grafos jerárquicos: mientras el plano euclidiano crece de manera polinómica, el espacio hiperbólico crece de manera exponencial. Esa propiedad lo vuelve especialmente adecuado para representar árboles, taxonomías, ontologías, redes jerárquicas y estructuras ramificadas.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **5. Crecimiento euclídeo, hiperbólico y árbol regular** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Comparación interactiva entre el crecimiento polinómico del plano euclídeo, el crecimiento exponencial del plano hiperbólico y el crecimiento ramificado de un árbol regular. Es una pieza central para entender por qué la geometría hiperbólica se adapta tan bien a jerarquías, taxonomías y grafos con expansión rápida.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Crecimiento%20comparado-22c55e?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Crecimiento%20eucl%C3%ADdeo%2C%20hiperb%C3%B3lico%20y%20%C3%A1rbol%20regular.html) |
| **6. Disco de Poincaré con árbol interactivo** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación interactiva que representa un árbol dentro del disco de Poincaré. Permite visualizar por qué la geometría hiperbólica es especialmente adecuada para grafos jerárquicos: a medida que aumentan los niveles del árbol, el espacio disponible crece hacia el borde del disco, permitiendo ubicar más nodos sin colapsar la estructura visual.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-%C3%81rbol%20en%20Poincar%C3%A9-22c55e?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/poincare_tree_interactive_html.html) |
| **7. Bola métrica en grafos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización dinámica del concepto de <strong>bola métrica</strong> en un grafo. A partir de un nodo central y un radio determinado, se muestra el conjunto de vértices alcanzables según la distancia interna del grafo. Conecta la expansión discreta de los grafos con el crecimiento de volumen en geometrías continuas.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Bola%20m%C3%A9trica-22c55e?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Bola%20m%C3%A9trica.html) |

---

# 3. Grafos como espacios métricos

Una vez construida la intuición geométrica, el recorrido pasa a la teoría de grafos. La idea clave es que un grafo no es solamente una red visual de nodos y aristas: también puede entenderse como un **espacio métrico discreto**, donde la distancia entre dos vértices se define por la longitud del camino más corto.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **8. Grafos conexos no ponderados** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Explicación matemática y visual de los grafos conexos no ponderados como espacios métricos discretos. Muestra cómo definir una distancia interna entre vértices mediante la longitud del camino más corto y cómo esa distancia permite estudiar bolas métricas, expansión, estructura global y embeddings hacia espacios euclidianos o hiperbólicos.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Grafos%20conexos-38bdf8?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_SGrafos%20conexos%20no%20ponderados.html) |
| **9. De un grafo a un espacio métrico** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Visualización didáctica que explica cuándo un grafo puede interpretarse como un espacio métrico a partir de la distancia de camino mínimo. Compara grafos conexos no dirigidos, árboles, grafos no conexos y grafos dirigidos, mostrando cómo cambian conectividad, simetría, finitud de distancias y propiedades métricas. Es un puente fundamental entre teoría de grafos y geometría.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Grafo%20a%20m%C3%A9trica-38bdf8?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_De%20un%20grafo%20a%20un%20espacio%20m%C3%A9trico.html) |
| **10. Espacio geométrico y grafos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Recurso dedicado a conectar grafos discretos con espacios geométricos continuos. Presenta la idea de un embedding como una función que transforma vértices en puntos de un espacio destino, preservando en lo posible relaciones de distancia, vecindad o jerarquía. Compara espacios euclídeos, distancia Manhattan, modelo hiperbólico, espacio esférico y similitud coseno.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Espacios%20geom%C3%A9tricos-38bdf8?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Espacio_Geom%C3%A9trico_y_Grafos_Tipos.html) |

---

# 4. Embeddings, simulación y distorsión

Esta etapa introduce el problema central de los embeddings: representar objetos discretos o complejos como puntos de un espacio geométrico. En grafos, el objetivo suele ser preservar distancias, vecindades, comunidades, jerarquías o relaciones semánticas. Pero todo embedding introduce algún grado de pérdida o distorsión, por eso es importante medirla y visualizarla.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **11. Tipos de embeddings: grafos, texto, imágenes y más** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Panorama amplio sobre distintos tipos de embeddings aplicados a grafos, texto, imágenes y otros datos. Explica cómo objetos discretos o complejos pueden transformarse en vectores o puntos de un espacio geométrico, permitiendo medir similitud, distancia, agrupamiento y relaciones semánticas o estructurales.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Tipos%20de%20embeddings-b694ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_Tipos%20de%20embeddings%20grafos%2C%20texto%2C%20im%C3%A1genes%20y%20m%C3%A1s.html) |
| **12. Embedding dinámico: simulación** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación interactiva del proceso de embedding como transformación desde datos discretos hacia un espacio vectorial. Permite observar cómo distintos objetos pueden convertirse en vectores, cómo se reorganizan en el espacio y cómo la cercanía geométrica puede interpretarse como similitud, relación estructural o proximidad semántica.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Embedding%20din%C3%A1mico-b694ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_embedding_dinamico_simulacion.html) |
| **13. Dashboard de distorsión de embeddings de grafos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Dashboard interactivo para analizar la <strong>distorsión</strong> producida al embeber grafos en espacios geométricos. Permite comparar distancias originales del grafo con distancias en el espacio destino, observar errores relativos y evaluar la calidad de la representación. Es clave para comprender que un embedding no solo busca ubicar nodos visualmente, sino preservar de manera controlada la estructura métrica del grafo.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Distorsion%20embedding-b694ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_dashboard_distorsion_embeddings_grafos.html) |
| **14. El problema del embedding: geometría hiperbólica y jerarquías** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Recorrido exhaustivo de 6 módulos sobre la representación de jerarquías y grafos en espacios continuos. Aborda el <em>mismatch</em> geométrico del espacio euclidiano frente al crecimiento exponencial de los árboles, introduciendo la <strong>geometría hiperbólica</strong> y la <strong>bola de Poincaré</strong> como solución estructural natural. Incluye optimización riemanniana, enfoques constructivos con garantías de baja distorsión, trade-offs numéricos y aplicaciones.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Problema%20del%20embedding-b694ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/5eff3f62f4b8f22d48d610183af72e47438d4ca6/src/classroom/graphs/recursos/arbol_hiperbolico.html) |

---

# 5. Laplaciano y señales sobre grafos

Antes de pasar a optimización, conviene incorporar el laplaciano porque permite estudiar difusión, suavidad, energía, consenso, clustering espectral y propagación de información sobre grafos. Este recurso conecta álgebra lineal, teoría espectral, redes y aprendizaje automático.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **15. Laplaciano de un grafo: teoría y visualización interactiva** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Recurso interactivo para estudiar el laplaciano de un grafo, especialmente en el caso no ponderado, no dirigido y conexo. Presenta las matrices de adyacencia <em>A</em>, grados <em>D</em> y laplaciano <em>L = D - A</em>, la forma cuadrática <em>xᵀLx</em> como medida de energía o rugosidad de una señal sobre el grafo, propiedades espectrales, difusión, consenso, vector de Fiedler y clustering espectral.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Laplaciano%20de%20Grafos-a78bfa?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_laplaciano_grafo_visual.html) |

---

# 6. Optimización: de GD a SGD y RSGD

Esta etapa muestra cómo se entrenan modelos o embeddings cuando el espacio de representación tiene una geometría específica. Primero se presenta Gradient Descent en espacio euclídeo, luego su versión estocástica, y finalmente Riemannian Stochastic Gradient Descent, donde los pasos deben respetar la geometría curva del espacio hiperbólico.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **16. Gradient Descent euclídeo: simulador avanzado** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador interactivo para explicar Gradient Descent como movimiento sobre una superficie de pérdida en espacio euclídeo. Permite observar el punto actual, la trayectoria de optimización, la norma del gradiente, el tamaño del paso, la pérdida y el diagnóstico del aprendizaje. Es conveniente ubicarlo antes de SGD y RSGD porque introduce la lógica base del descenso por gradiente.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Gradient%20Descent-38bdf8?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_GD.html) |
| **17. SGD clásico en espacio euclídeo: simulador avanzado** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulador avanzado de <strong>Stochastic Gradient Descent</strong> en espacio euclídeo. Permite visualizar por qué el entrenamiento es estocástico: el modelo no calcula siempre el gradiente exacto sobre todos los datos, sino una aproximación basada en muestras o mini-batches. Esto introduce ruido, oscilaciones y trayectorias irregulares, pero permite entrenar modelos grandes de manera eficiente.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-SGD%20Eucl%C3%ADdeo-fb923c?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperbolico_SGD.html) |
| **18. RSGD en el disco de Poincaré: recurso comparativo** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Simulación comparativa de RSGD en espacio hiperbólico que muestra de forma directa la diferencia entre un paso euclídeo y un paso riemanniano. Presenta fórmulas comparativas de SGD plano y RSGD curvo, controles de simulación, métricas del punto entrenable, geodésicas, objetivo, gradiente y lectura visual del movimiento dentro del disco de Poincaré.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-RSGD%20Comparativo-22c55e?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperbolico_RSSD_adicional.html) |
| **19. RSGD en geometría hiperbólica: laboratorio avanzado** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Laboratorio avanzado para explicar <strong>Riemannian Stochastic Gradient Descent</strong> dentro del disco de Poincaré. Muestra cómo un embedding se entrena dentro de una geometría curva, con nodos generales cerca del centro y nodos específicos hacia la frontera. Incluye simulación dinámica, cambio de paleta visual, escenarios conceptuales, geodésicas, comparación con SGD euclídeo, ruido estocástico y tabla comparativa entre SGD tradicional y RSGD.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-RSGD%20Hiperb%C3%B3lico-36e7c7?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperbolico_RGSD.html) |

---

# 7. Integración con inteligencia artificial

Esta etapa funciona como síntesis aplicada. La geometría, los grafos y los embeddings se conectan con inteligencia artificial: GNN, GraphRAG, grafos de conocimiento, redes sociales, mapas semánticos, sistemas financieros, grafos moleculares, modelos basados en agentes y representación de jerarquías.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **20. Tabla avanzada: grafos, espacios geométricos e IA** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Matriz interactiva que relaciona tipos de grafos, espacios geométricos convenientes y algoritmos posibles. Conecta grafos simples, árboles, grafos jerárquicos, redes sociales, grafos de conocimiento, grafos dinámicos, grafos financieros, grafos moleculares, GraphRAG, mapas de conocimiento personal y modelos basados en agentes con espacios euclídeos, hiperbólicos, riemannianos, temporales o semánticos.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Tabla%20Grafos%20IA-42d9ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperbolico%20Tabla_grafos_AI.html) |
| **21. Grafos, espacios geométricos e inteligencia artificial** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Lección interactiva amplia que conecta grafos, métricas, embeddings, geometrías de representación e inteligencia artificial. Presenta la idea de pasar de una estructura discreta a un espacio continuo, muestra simuladores de embeddings, compara espacios euclídeos, hiperbólicos y esféricos, incluye matriz de decisión, glosario conceptual y vínculos con GNN, GraphRAG, conocimiento semántico, rutas, jerarquías y aprendizaje automático sobre grafos. Funciona como recurso integrador antes del cierre de estudio.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Grafos%20Geometr%C3%ADa%20IA-b694ff?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperb%C3%B3lico_GRAFOS_GEOMETRIA_IA.html) |

---

# 8. Cierre de estudio: glosario y cuestionario

Estos dos recursos deben quedar al final del recorrido de estudio. Primero se consulta el glosario para consolidar el vocabulario técnico y luego se utiliza el cuestionario como instancia de autoevaluación, repaso y preparación de clase.

| 📄 Recurso | 📥 Acceso HTML |
|---|---|
| **22. Glosario: Geometría Hiperbólica, Grafos y Embeddings** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Glosario interactivo con 79 términos organizados en 13 categorías. Incluye conceptos de fundamentos métricos, embeddings, geometría hiperbólica, modelos hiperbólicos, funciones matemáticas, optimización, optimización riemanniana, evaluación, límites, construcción, garantías y aplicaciones. Se ubica al final porque funciona como recurso de consulta y consolidación después de haber recorrido las visualizaciones, los modelos, los grafos, los embeddings y los algoritmos.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Glosario-f0c040?style=for-the-badge&logo=html5)](https://htmlpreview.github.io/?https://github.com/sgevatschnaider/BigData-Graphs-Evo-CA-Classroom/blob/main/src/classroom/graphs/recursos/Hiperbolico_glosario.html) |
| **23. Cuestionario: Geometría Hiperbólica, Grafos y Embeddings** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Cuestionario académico interactivo con 30 preguntas organizadas en 6 módulos: embeddings y grafos, geometría hiperbólica, optimización riemanniana, construcción y garantías, evaluación y límites, y aplicaciones. Incluye búsqueda por conceptos, filtro por módulo, modo examen, progreso de estudio, botones para expandir o colapsar respuestas, opción de imprimir o exportar a PDF y tarjetas con respuestas desarrolladas. Se deja como último recurso porque funciona como instancia final de repaso, autoevaluación y preparación de clase.</p></details> | [![Ver HTML](https://img.shields.io/badge/Ver%20HTML-Cuestionario-36e6c1?style=for-the-badge&logo=html5)](https://clinquant-meringue-3930c2.netlify.app/src/classroom/graphs/recursos/hiperbolica_cuestionario_geometria_hiperbolica) |

# Guías de estudio: geometría hiperbólica, grafos y embeddings

Esta sección reúne las guías de apoyo vinculadas específicamente con geometría hiperbólica, grafos, embeddings y aplicaciones en machine learning. Los materiales están pensados para acompañar el estudio conceptual, la resolución de ejercicios y la preparación de clase.

Los documentos completos se encuentran disponibles en la siguiente carpeta de Google Drive:

[![Abrir carpeta en Drive](https://img.shields.io/badge/Abrir%20carpeta-Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)](https://drive.google.com/drive/folders/1jFB8G6uUIU73hAKb-J_b9eyT_dOsUt_7?usp=sharing)

| 📄 Guía | 🧭 Tema principal | 📌 Descripción |
|---|---|---|
| **1. Guía de ejercicios resueltos: Grafos, embeddings y geometría hiperbólica** | Métrica de grafos, embeddings y disco de Poincaré | Guía organizada para trabajar la relación entre grafos, matrices, laplaciano, espectro, embeddings euclídeos e hiperbólicos. Incluye ejercicios sobre distancia en grafos, bolas métricas, crecimiento jerárquico, distorsión, geometría del disco de Poincaré, optimización, Gradient Descent, RSGD, matriz de adyacencia, matriz de distancia, laplaciano, autovalores, autovectores y conectividad. |
| **2. Guía completa de ejercicios: Geometría hiperbólica, grafos y embeddings en machine learning** | Geometría hiperbólica aplicada a machine learning | Material de ejercicios conceptuales y avanzados sobre el uso de geometría hiperbólica para representar grafos jerárquicos, taxonomías, ontologías, redes complejas y embeddings utilizados en machine learning. Incluye fundamentos, embeddings aprendidos, aplicaciones, simulaciones, optimización, funciones de pérdida, curvatura y tareas de aprendizaje automático. |

## Secuencia sugerida de uso

1. Comenzar con la **guía de grafos, embeddings y geometría hiperbólica**, porque introduce la base matemática necesaria: distancia en grafos, bolas métricas, crecimiento jerárquico, distorsión, disco de Poincaré, laplaciano y espectro.

2. Continuar con la **guía completa de geometría hiperbólica, grafos y embeddings en machine learning**, que amplía el recorrido hacia aplicaciones modernas como taxonomías, ontologías, grafos de conocimiento, redes complejas, simulaciones, funciones de pérdida y optimización riemanniana.

## Articulación con recursos interactivos

Estas guías complementan los recursos HTML interactivos del repositorio. La lectura sugerida es trabajar primero las visualizaciones y simulaciones, luego consultar las guías de ejercicios resueltos y finalmente utilizar el glosario y el cuestionario como instancia de consolidación y autoevaluación.


# 🎥 Geometría Hiperbólica, Disco de Poincaré y RSGD  
## Curaduría audiovisual guiada para estudiar modelos, visualizaciones y aplicaciones en ciencia de datos

> Esta sección reúne videos seleccionados para construir una comprensión progresiva de la geometría hiperbólica: primero desde la intuición visual, luego desde el modelo formal del disco de Poincaré, después desde las teselaciones tipo Escher y finalmente desde la optimización riemanniana aplicada a embeddings, grafos jerárquicos y aprendizaje automático.

<p align="center">
  <img src="https://img.shields.io/badge/Tema-Geometría%20Hiperbólica-4B0082?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Modelo-Disco%20de%20Poincaré-0B7285?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Aplicación-RSGD%20%7C%20Embeddings-2F9E44?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Nivel-Progresivo-FF922B?style=for-the-badge" />
</p>

---

## 🧭 Ruta de estudio recomendada

La curaduría está organizada como una secuencia didáctica. La idea no es ver los videos de manera aislada, sino avanzar desde la intuición geométrica hasta la aplicación computacional.

| Etapa | Pregunta guía | Qué conviene mirar primero | Objetivo conceptual |
| :---: | :--- | :--- | :--- |
| **1** | ¿Qué es una geometría no euclidiana? | Introducciones visuales | Comprender la diferencia entre espacio euclídeo e hiperbólico. |
| **2** | ¿Cómo se representa un plano infinito dentro de un disco finito? | Disco de Poincaré | Entender frontera ideal, geodésicas y deformación de distancias. |
| **3** | ¿Por qué las teselaciones se comprimen hacia el borde? | Escher y patrones hiperbólicos | Visualizar crecimiento exponencial y simetrías hiperbólicas. |
| **4** | ¿Cómo se optimiza una función cuando el espacio no es plano? | Optimización riemanniana | Conectar gradientes, variedades, RSGD y embeddings hiperbólicos. |
| **5** | ¿Por qué esto importa para grafos, jerarquías e IA? | Riemannian optimization + aplicaciones | Relacionar geometría, ciencia de datos y representación de estructuras complejas. |

---

## 🧠 Mapa conceptual de la curaduría

```text
Geometría hiperbólica
│
├── Intuición geométrica
│   ├── curvatura negativa
│   ├── crecimiento exponencial
│   └── geometrías no euclidianas
│
├── Modelos de representación
│   ├── disco de Poincaré
│   ├── geodésicas
│   ├── frontera ideal
│   └── isometrías
│
├── Visualización artística y matemática
│   ├── teselaciones
│   ├── patrones tipo Escher
│   └── repetición hacia el borde
│
└── Aplicaciones computacionales
    ├── variedades riemannianas
    ├── RSGD
    ├── embeddings hiperbólicos
    └── grafos jerárquicos
```

---

## 📌 Criterio de lectura

Cada video fue clasificado según su función dentro del aprendizaje:

- **Intuición visual:** permite comprender la idea geométrica sin comenzar por fórmulas.
- **Modelo matemático:** introduce el disco de Poincaré, geodésicas, métricas e isometrías.
- **Visualización avanzada:** conecta geometría hiperbólica con teselaciones y patrones tipo Escher.
- **Optimización y aprendizaje automático:** permite vincular la geometría con RSGD, embeddings y grafos.

---

# 🎬 Biblioteca audiovisual curada

## 1. Puerta de entrada: intuición geométrica

| Recurso | Nivel | Concepto central | Uso recomendado | Enlace |
| :--- | :---: | :--- | :--- | :---: |
| **Introducción visual a la geometría hiperbólica**<br><sub>Video ideal para comenzar. Desarrolla intuición sobre el plano hiperbólico, la curvatura negativa y distintos modelos de representación, incluyendo el disco de Poincaré.</sub> | 🟢 Inicial | Curvatura negativa y modelos visuales | Usarlo antes de entrar en fórmulas. Sirve para que el estudiante entienda por qué la geometría hiperbólica no se comporta como la geometría euclidiana. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=eGEQ_UuQtYs) |
| **Geometría hiperbólica y disco de Poincaré**<br><sub>Complemento breve de divulgación para reforzar la idea de geometría no euclidiana y visualizar cómo el disco de Poincaré permite representar un plano infinito dentro de una región finita.</sub> | 🟢 Inicial | Plano infinito dentro de un disco finito | Recurso de refuerzo para explicar la diferencia entre mirar el disco con ojos euclidianos y entenderlo como representación hiperbólica. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=bOPaGHqQxeY) |

---

## 2. Disco de Poincaré: del dibujo a la estructura matemática

| Recurso | Nivel | Concepto central | Uso recomendado | Enlace |
| :--- | :---: | :--- | :--- | :---: |
| **Modelo formal del disco de Poincaré**<br><sub>Clase más técnica sobre el modelo del disco, la métrica hiperbólica, las geodésicas y las isometrías. Es útil para pasar de la intuición visual a la formulación matemática.</sub> | 🟡 Intermedio | Métrica, geodésicas e isometrías | Usarlo cuando ya se comprendió visualmente el disco y se quiere justificar matemáticamente por qué las rectas hiperbólicas aparecen como diámetros o arcos ortogonales al borde. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=KbR55AX7DUs) |
| **Introducción técnica al disco de Poincaré**<br><sub>Recurso de apoyo para estudiar el modelo del disco desde una perspectiva matemática, reforzando conceptos como frontera ideal, geodésicas y transformación de distancias.</sub> | 🟡 Intermedio | Frontera ideal y distancias hiperbólicas | Conveniente para acompañar una simulación del disco de Poincaré o una explicación sobre por qué el borde está infinitamente lejos en la métrica hiperbólica. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=OErKcpfSfn8) |
| **Serie sobre el disco de Poincaré**<br><sub>Playlist recomendada para profundizar paso a paso en el modelo del disco, sus propiedades geométricas y su interpretación dentro de la geometría no euclidiana.</sub> | 🟡 Intermedio | Estudio progresivo del modelo | Ideal como material complementario para estudiantes que quieran revisar el tema en varias sesiones y no solo con un único video introductorio. | [![Ver playlist](https://img.shields.io/badge/YouTube-Ver%20playlist-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PL1BF3AE959970630F) |

---

## 3. Teselaciones hiperbólicas: de Escher a los algoritmos geométricos

| Recurso | Nivel | Concepto central | Uso recomendado | Enlace |
| :--- | :---: | :--- | :--- | :---: |
| **Teselaciones hiperbólicas y patrones tipo Escher**<br><sub>Explica cómo generar patrones hiperbólicos dentro del disco de Poincaré, conectando algoritmos geométricos con las obras de M. C. Escher y las teselaciones del plano hiperbólico.</sub> | 🔵 Visual avanzado | Teselaciones y repetición hiperbólica | Usarlo para mostrar que la geometría hiperbólica no es solo una abstracción, sino también una estructura que puede generar patrones visuales, arte matemático y algoritmos de repetición espacial. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](http://www.youtube.com/watch?v=uX5dGZ6Kzyw) |
| **Circle Limit III y teselaciones hiperbólicas**<br><sub>Animación visual inspirada en Circle Limit III, útil para observar cómo los patrones hiperbólicos se repiten hacia el borde del disco y generan una sensación de profundidad infinita.</sub> | 🔵 Visual avanzado | Escher, simetría y profundidad infinita | Recomendado para conectar matemática, visualización y comunicación. Es especialmente útil después de explicar que el borde del disco representa una frontera ideal infinitamente lejana. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=xkkJcNwrDVM) |
| **Geometría no euclidiana y disco de Poincaré**<br><sub>Conferencia conceptual sobre el disco de Poincaré, su historia matemática y su importancia para representar geometrías no euclidianas de manera visualmente comprensible.</sub> | 🟡 Intermedio | Historia, modelo y significado geométrico | Puede usarse como recurso de profundización para unir historia matemática, interpretación visual y formalización geométrica. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=Ao-Otx6ik_Q) |

---

## 4. Optimización riemanniana, RSGD y aprendizaje automático

| Recurso | Nivel | Concepto central | Uso recomendado | Enlace |
| :--- | :---: | :--- | :--- | :---: |
| **Optimización riemanniana y variedades**<br><sub>Introducción al gradiente riemanniano, retracciones y métodos de optimización sobre variedades. Sirve como puente hacia RSGD y embeddings en espacios no euclidianos.</sub> | 🔴 Avanzado | Gradiente riemanniano y optimización sobre variedades | Usarlo cuando se quiera explicar por qué el descenso de gradiente clásico no alcanza si los parámetros viven en un espacio curvo como el disco de Poincaré o una variedad riemanniana. | [![Ver video](https://img.shields.io/badge/YouTube-Ver%20video-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=NZSW-oqDq9A) |
| **Geometría riemanniana aplicada a aprendizaje y control**<br><sub>Playlist avanzada sobre geometría riemanniana aplicada, útil para vincular el enfoque geométrico con aprendizaje automático, robótica, control y optimización sobre espacios curvos.</sub> | 🔴 Avanzado | Geometría aplicada, aprendizaje y control | Recurso para ampliar la conexión entre geometría diferencial, optimización, inteligencia artificial, robótica y modelos de representación. | [![Ver playlist](https://img.shields.io/badge/YouTube-Ver%20playlist-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PL_oEZ6dld4ignAdbFvcP_LAJgNbdrNBKC) |

---

# 🧩 Tabla sintética para orientar al estudiante

| Bloque | Qué se aprende | Conceptos que conviene recordar | Relación con IA y ciencia de datos |
| :--- | :--- | :--- | :--- |
| **Intuición hiperbólica** | Que existen geometrías donde las reglas euclidianas no describen bien el espacio. | Curvatura negativa, crecimiento exponencial, no euclidiano. | Ayuda a entender por qué algunos datos no se representan bien en espacios planos. |
| **Disco de Poincaré** | Que un plano hiperbólico infinito puede representarse dentro de un disco finito. | Geodésicas, frontera ideal, métrica hiperbólica. | Permite construir embeddings hiperbólicos para jerarquías y grafos. |
| **Teselaciones** | Que el plano hiperbólico admite patrones con crecimiento visual hacia el borde. | Simetrías, teselación, repetición, Escher. | Sirve para visualizar expansión exponencial, muy común en árboles y taxonomías. |
| **Optimización riemanniana** | Que optimizar en espacios curvos requiere adaptar el gradiente. | Variedad, gradiente riemanniano, retracción, RSGD. | Base matemática para entrenar embeddings en espacios hiperbólicos. |

---

# 🔎 Cómo usar esta curaduría junto con las simulaciones interactivas

1. **Antes de la simulación**, mirar los videos introductorios para instalar la intuición visual.
2. **Durante la simulación**, relacionar cada elemento visual con un concepto: borde, geodésica, distancia, curvatura y crecimiento.
3. **Después de la simulación**, avanzar hacia optimización riemanniana para comprender cómo se entrenan embeddings en espacios no euclidianos.
4. **Como cierre**, conectar el tema con grafos jerárquicos, taxonomías, redes complejas e inteligencia artificial geométrica.

---

# ✅ Ideas clave para recordar

- El disco de Poincaré no es simplemente un dibujo circular: es una representación conforme del plano hiperbólico.
- Los puntos cercanos al borde parecen comprimidos visualmente, pero en la métrica hiperbólica pueden estar muy lejos.
- Las geodésicas del disco son diámetros o arcos de circunferencia ortogonales al borde.
- Las teselaciones hiperbólicas muestran cómo el espacio disponible crece rápidamente al alejarse del centro.
- RSGD adapta el descenso de gradiente clásico para trabajar sobre variedades y espacios curvos.
- Los embeddings hiperbólicos son especialmente útiles cuando los datos tienen estructura jerárquica, como árboles, taxonomías, grafos de conocimiento o redes con expansión exponencial.

---
### 8. Perspectiva Algebraica: Grafos de Cayley
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
## 🏆 Proyecto Final: Detector de Anomalías Multivariante

<p align="center">
  <img src="https://img.shields.io/badge/Dificultad-Avanzada-red?style=for-the-badge" alt="Dificultad">
  <img src="https://img.shields.io/badge/Herramienta-Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter" alt="Jupyter">
  <img src="https://img.shields.io/badge/Librer%C3%ADas-NumPy%20%7C%20SciPy-blue?style=for-the-badge" alt="Librerías">
</p>



### 📝 Descripción del Problema
En espacios de alta dimensión donde las variables están correlacionadas, la distancia Euclidiana es engañosa. Un punto puede parecer "cercano" al centroide pero violar por completo la estructura de covarianza del sistema. 

El objetivo de este proyecto es implementar un sistema de **Detección de Anomalías (Outlier Detection)** desde cero utilizando la **Distancia de Mahalanobis**, aplicándolo a un conjunto de datos real (por ejemplo, transacciones bancarias o lecturas de sensores industriales).

### 🛠️ Requisitos de Implementación (Step-by-Step)

1. **Adquisición y Limpieza:**
   * Cargar un dataset multivariante continuo (se recomienda el *Credit Card Fraud Detection* de Kaggle o un dataset de telemetría).
   * Separar un subconjunto de datos "sanos" (inliers) para calibrar el modelo.

2. **Ajuste del Modelo Paramétrico (MVN):**
   * Calcular el vector de medias $\mu \in \mathbb{R}^d$.
   * Estimar la matriz de covarianza muestral $\Sigma \in \mathbb{R}^{d \times d}$.
   * *Control de estabilidad:* Verificar si $\Sigma$ es mal condicionada y aplicar regularización (Ridge/Tikhonov) o usar la pseudoinversa (`np.linalg.pinv`) si es necesario.

3. **Ingeniería de Distancias:**
   * Implementar vectorizadamente el cálculo del cuadrado de la distancia de Mahalanobis para cada nueva observación $x$:
     $$D_M^2(x) = (x - \mu)^T \Sigma^{-1} (x - \mu)$$

4. **Decisión Estadística y Umbrales:**
   * **Teoría:** Sabiendo que $D_M^2$ sigue una distribución $\chi^2$ (Chi-cuadrado) con $d$ grados de libertad.
   * **Práctica:** Utilizar `scipy.stats.chi2.ppf` para establecer un umbral de corte estricto (ej. $\alpha = 0.01$ o $\alpha = 0.001$). Todo punto que supere este umbral es clasificado como anomalía.

5. **Análisis y Visualización:**
   * Proyectar los datos a 2D utilizando Análisis de Componentes Principales (PCA) calculado manualmente mediante la descomposición espectral de $\Sigma$.
   * Graficar las observaciones normales, las anomalías detectadas y los isocontornos (elipsoides de confianza).

### 📦 Entregables Esperados

* Un archivo `Proyecto_Mahalanobis.ipynb` completamente documentado.
* El código debe estar estructurado en funciones limpias (ej. `fit_mvn(X)`, `mahalanobis_score(X_test, mu, cov)`, `predict_anomalies(scores, alpha)`).
* Un breve reporte final (en celdas Markdown) discutiendo:
  1. ¿Qué ventajas observaste respecto a usar simplemente una métrica Euclidiana?
  2. ¿Qué ocurre con la eficacia del detector si los datos subyacentes no son verdaderamente Gaussianos?

<details>
<summary>💡 <strong>Pista para la vectorización (clic para ver)</strong></summary>

Evita usar bucles `for` para calcular la distancia de miles de filas. Si `X` es tu matriz de datos centrada $(X - \mu)$ de dimensión $(n, d)$ y `InvSigma` es la matriz inversa $(d, d)$, puedes calcular todas las distancias simultáneamente usando un producto de matrices y sumando a lo largo del eje correcto:

```python
delta = X_test - mu
# (n, d) @ (d, d) -> (n, d)
left_term = np.dot(delta, inv_sigma) 
# Producto elemento a elemento y suma por filas
D_squared = np.sum(left_term * delta, axis=1)
## ⚠️ Errores Comunes (Troubleshooting)

* **Matriz Singular:** Si `np.linalg.inv(Sigma)` falla, tu matriz de covarianza no es invertible (tienes variables colineales). *Solución:* Usar `np.linalg.pinv` (pseudoinversa).
* **Maldición de la Dimensionalidad:** En alta dimensión, casi todos los puntos parecen "lejanos" (concentración en la corteza). No confíes en la intuición 2D/3D ciegamente.
* **Interpretación de Correlación:**  implica independencia **solo** si la distribución es Gaussiana. En otros casos, puede haber dependencia no lineal.

```

