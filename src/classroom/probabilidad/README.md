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

| 📄 Recurso | 📥 Acceso |
|---|---|
| **Dependencia lineal vs. independencia estadística** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este recurso interactivo desarrolla la diferencia entre dependencia lineal e independencia estadística desde una perspectiva algebraica, geométrica y aplicada. Explica cómo ambas nociones no deben confundirse, analiza su relación con correlación, caso gaussiano y multicolinealidad, y muestra por qué son conceptos centrales en regresión, selección de variables y análisis de datos. Es un material útil para comprender la diferencia entre estructura algebraica de los datos y relaciones probabilísticas entre variables.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/f11ed7e45e3b4c815c7945e35fa4875448931001/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia_lineal_independencia_estadistica.html) |
| **Dependencia lineal: elipsoide y geometría de datos** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este material presenta el elipsoide como objeto geométrico central en la geometría de datos. Explica cómo la matriz de covarianza y la descomposición espectral permiten interpretar dependencia lineal, multicolinealidad e independencia estadística a partir de la forma, orientación y degeneración del elipsoide. El recurso conecta álgebra lineal, estadística multivariada y visualización geométrica, mostrando cómo los autovalores y autovectores describen dispersión, anisotropía y alineación de los datos.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/f11ed7e45e3b4c815c7945e35fa4875448931001/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia%20lineal_elipsoide_geometria_datos.html) |
| **Glosario: dependencia lineal, independencia estadística, correlación y multicolinealidad** <br><br> <details><summary><strong>Resumen:</strong> <em>(haz clic para expandir/colapsar)</em></summary><p>Este glosario reúne y organiza los conceptos fundamentales vinculados con dependencia lineal, independencia estadística, correlación y multicolinealidad. Presenta definiciones claras, precisiones terminológicas y relaciones entre los conceptos principales, sirviendo como material de consulta y apoyo para el estudio de álgebra lineal, geometría de datos y estadística. Es especialmente útil como referencia rápida para consolidar vocabulario técnico y comprender diferencias conceptuales clave.</p></details> | [![HTML Interactivo](https://img.shields.io/badge/HTML-Interactivo-blue?style=for-the-badge&logo=google-chrome)](https://htmlpreview.github.io/?https://raw.githubusercontent.com/sgevatschnaider/estadisticas-para-ciencia-de-datos/f11ed7e45e3b4c815c7945e35fa4875448931001/src/classroom/probabilidad/html/Modulo%20I_punto2_Dependencia_lineal_glosario.html) |

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

