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
| **Teoría de la Medida e Integral de Lebesgue**<br><sub>*Complemento para entender por qué la integración de Riemann falla en el continuo y cómo Lebesgue agrupa por preimagen.*</sub> | **The Bright Side of Mathematics**<br><sub>*Measure Theory (Curso Completo)*</sub> | [![Ver Playlist](https://img.shields.io/badge/Playlist-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLBh2i93oe2qvMVqAzsX1Kuv6-4fjazZ8j) |
| **Desigualdades de Concentración**<br><sub>*La demostración rigurosa de Markov y Chebyshev, fundamental para entender las cotas de error en algoritmos.*</sub> | **Steve Brunton**<br><sub>*Chebyshev's Inequality*</sub><br><br>**MIT OpenCourseWare**<br><sub>*Prof. John Tsitsiklis (Lecture 20)*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=otCHN3s52ho) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=nrDkb2MAwSA) |
| **Método de la Transformada Inversa**<br><sub>*La matemática detrás de la simulación de variables aleatorias usando la función cuantil ($F^{-1}$).*</sub> | **Ben Lambert**<br><sub>*Inverse transform sampling*</sub><br><br>**ritvikmath**<br><sub>*Inverse Transform Sampling*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=rnBbYsysPaU) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=9ixzzPQWuAY) |
| **Topología del Continuo y Medida Cero**<br><sub>*Paradojas del espacio muestral continuo, mapeos infinitos y por qué probabilidad 0 $\neq$ imposible.*</sub> | **3Blue1Brown**<br><sub>*Probabilities of continuous spaces*</sub><br><br>**Vsauce**<br><sub>*How To Count Past Infinity*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=ZA4JkHKZM50) <br><br> [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=SrU9YDoXE88) |
| **Censura vs. Truncamiento (Econometría)**<br><sub>*Entendiendo la formación de átomos (masas puntuales) en las colas, esencial para los Modelos Tobit.*</sub> | **Anders Munk-Nielsen**<br><sub>*The Tobit Model*</sub><br><br>**Jake Clifton / Ben Lambert**<br><sub>*Econometrics II (Playlist)*</sub> | [![Ver Video](https://img.shields.io/badge/Video-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/watch?v=IwsE8Rr6l6E) <br><br> [![Ver Playlist](https://img.shields.io/badge/Playlist-YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/playlist?list=PLLZ4uVeiDmR_rzu-uYl9A5BrmvTKtH_aB) |

---
## 📖 Evaluaciones y Referencias (Recursos HTML)

| 📄 Recurso | 📥 Acceso |
| ---------- | --------- |
| **HTML: Cuestionario Experto** <br><br><details><summary><strong>Resumen:</strong> <em>(clic para expandir/colapsar)</em></summary><p>Cuestionario interactivo con 20 preguntas de nivel experto diseñadas para evaluar la comprensión profunda de la teoría de la medida, probabilidad continua y desigualdades de concentración. Cada pregunta incluye una respuesta detallada estructurada analíticamente.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML5-green?style=for-the-badge&logo=html5)](https://sgevatschnaider.github.io/blockchain-finanzas-descentralizadas/unidades/u02-criptoactivos-consenso-seguridad/html/Cuestionario.html) |
| **HTML: Glosario Interactivo** <br><br><details><summary><strong>Resumen:</strong> <em>(clic para expandir/colapsar)</em></summary><p>Glosario completo con definiciones detalladas de los conceptos fundamentales. Incluye un filtro de búsqueda en tiempo real y navegación alfabética para facilitar la consulta y el estudio de términos clave.</p></details> | [![Abrir HTML](https://img.shields.io/badge/Abrir-HTML5-green?style=for-the-badge&logo=html5)](https://sgevatschnaider.github.io/blockchain-finanzas-descentralizadas/unidades/u02-criptoactivos-consenso-seguridad/html/Glosario.html) |

---

### Cuestionario Experto: Desarrollo Analítico

<details>
<summary><strong>1) ¿Qué diferencia conceptual separa a Riemann de Lebesgue, y por qué eso importa para probabilidad moderna?</strong></summary>
<br>
<p>La diferencia fundamental reside en la estrategia de partición antes de sumar. La integral de Riemann intenta calcular el área bajo una curva particionando el eje horizontal (el dominio, $x$) en pequeños intervalos contiguos y aproximando rectángulos. Cuando una función es altamente discontinua o fractal, este enfoque colapsa porque no se puede definir un límite consistente para los rectángulos.</p>

<p>Lebesgue revoluciona este concepto: en lugar de particionar el dominio, particiona el codominio (el eje vertical, $y$). Agrupa los puntos del dominio que comparten el mismo valor de la función (preimágenes) y simplemente mide el "tamaño" (la medida) de ese conjunto. En probabilidad moderna, esto es vital porque una variable aleatoria es exactamente una función sobre un espacio abstracto de resultados ($\Omega$). Calcular una esperanza matemática mediante Lebesgue se traduce naturalmente en una suma ponderada: el valor de la variable multiplicado por la probabilidad (medida) del conjunto de eventos que producen ese valor.</p>
</details>

<details>
<summary><strong>2) ¿Cómo se define el “Juego de las Esperas” con monedas y cuál es exactamente la variable aleatoria de interés?</strong></summary>
<br>
<p>El "Juego de las Esperas" es un modelo estocástico donde se lanza una moneda repetidamente hasta que aparece la primera Cara (H). La recompensa o resultado del juego es el número total de lanzamientos requeridos.</p>
<p>Formalmente, la variable aleatoria de interés, $X$, es una función medible que mapea el espacio de secuencias infinitas de cruces y caras hacia los números naturales ($\mathbb{N}$). Representa el "tiempo de espera" hasta el primer éxito. Si sale Cara en el primer intento, $X=1$. Si la secuencia comienza con Cruz-Cara (TH), $X=2$. En el caso general, $X=k$ corresponde a una racha inicial de $k-1$ cruces seguidas de una cara ($T^{k-1}H$). Esta variable aleatoria sigue una distribución de probabilidad Geométrica, caracterizada por modelar el número de ensayos de Bernoulli independientes necesarios para obtener el primer éxito.</p>
</details>

<details>
<summary><strong>3) ¿Qué significa en este contexto que “cada pila de premio es un Conjunto Cilíndrico”?</strong></summary>
<br>
<p>En la teoría de la medida aplicada a espacios de secuencias infinitas, como $\{H,T\}^{\mathbb{N}}$, es imposible asignar una probabilidad positiva a una única secuencia infinita específica. Para resolver esto, se construyen "conjuntos cilíndricos". Un cilindro es un evento definido por la fijación estricta de un prefijo finito de coordenadas, dejando el resto de la secuencia infinita completamente libre.</p>
<p>Cuando agrupamos todas las secuencias que nos otorgan el mismo premio $k$, estamos definiendo un conjunto cilíndrico. Por ejemplo, el evento "$X=3$" agrupa a todas las secuencias infinitas que comienzan inevitablemente con el patrón TTH. Todo lo que ocurre a partir del cuarto lanzamiento es irrelevante para el premio. Esta estructura topológica es crucial porque permite asignar medidas de probabilidad exactas operando únicamente sobre el segmento finito conocido.</p>
</details>

<details>
<summary><strong>4) ¿Por qué en el juego de esperas se obtiene $P(X=k)=2^{-k}$ con moneda justa?</strong></summary>
<br>
<p>Para que la variable aleatoria tome exactamente el valor $X=k$, debe ocurrir un evento altamente específico: una secuencia ininterrumpida de $k-1$ cruces, terminada abruptamente por una cara en el lanzamiento número $k$ (el patrón $T^{k-1}H$).</p>
<p>Bajo el supuesto de una moneda justa (probabilidad simétrica $p=1/2$) y el axioma de independencia estricta entre lanzamientos, la probabilidad de una intersección de eventos independientes es el producto de sus probabilidades individuales. Por lo tanto, la probabilidad del patrón se calcula multiplicando $1/2$ repetidas veces:</p>
$$P(T^{k-1}H) = \left(\frac{1}{2}\right)^{k-1} \times \left(\frac{1}{2}\right) = \left(\frac{1}{2}\right)^k = 2^{-k}$$
<p>Esta es la medida geométrica exacta que corresponde a ese conjunto cilíndrico particular en el espacio muestral.</p>
</details>

<details>
<summary><strong>5) ¿Cómo se calcula la esperanza $\mathbb{E}[X]$ en el juego de esperas y por qué da exactamente 2?</strong></summary>
<br>
<p>La esperanza matemática se define formalmente como la integral de la variable aleatoria respecto a su medida de probabilidad, que en un espacio discreto se reduce a una suma infinita ponderada:</p>
$$\mathbb{E}[X] = \sum_{k=1}^{\infty} k P(X=k)$$
<p>Sustituyendo la probabilidad geométrica hallada previamente:</p>
$$\mathbb{E}[X] = \sum_{k=1}^{\infty} k 2^{-k} = 1\left(\frac{1}{2}\right) + 2\left(\frac{1}{4}\right) + 3\left(\frac{1}{8}\right) + \dots$$
<p>Esta es una serie aritmético-geométrica convergente. Al resolverla analíticamente, la suma converge de manera exacta al valor 2. La intuición geométrica es que el peso probabilístico decae exponencialmente (los denominadores crecen en potencias de 2), lo cual aplasta rápidamente el crecimiento lineal de los premios ($k$), resultando en un promedio teórico finito y manejable de 2 lanzamientos.</p>
</details>

<details>
<summary><strong>6) ¿Qué diferencia conceptual existe entre la “simulación” de un experimento y su cálculo exacto analítico?</strong></summary>
<br>
<p>La simulación computacional (métodos de Monte Carlo) se fundamenta en la Ley de los Grandes Números. Al repetir el experimento estocástico millones de veces y registrar las frecuencias empíricas, el promedio muestral tiende a converger hacia el valor esperado teórico. Es una herramienta poderosa para generar intuición o resolver integrales intratables en espacios de alta dimensionalidad.</p>
<p>Sin embargo, su limitación conceptual radica en que nunca constituye una demostración matemática rigurosa. Una simulación siempre arrastra un margen de error estadístico (varianza empírica) y está supeditada a las limitaciones de los generadores de números pseudoaleatorios (PRNG). El cálculo analítico exacto, ya sea mediante series discretas o la integral de Lebesgue, entrega un resultado absoluto, universal y libre de ruido estocástico.</p>
</details>

<details>
<summary><strong>7) ¿Cuál es un ejemplo donde “Riemann falla” y “Lebesgue triunfa”, y qué enseña sobre medir racionales e irracionales?</strong></summary>
<br>
<p>Un caso canónico es una función indicadora tipo Dirichlet modificada en el intervalo $[0,1]$: se define un pago de 1000 si el número es racional ($\mathbb{Q}$) y 0 si es irracional ($\mathbb{I}$).</p>
<p>La integral de Riemann colapsa al intentar calcular la esperanza. Como entre dos racionales siempre hay un irracional y viceversa, cualquier rectángulo que intente aproximar el área oscilará caóticamente entre 0 y 1000, impidiendo la convergencia del límite de las sumas.</p>
<p>Lebesgue triunfa al ignorar la posición en el eje $x$ y mirar directamente las preimágenes. La preimagen del pago 1000 son todos los racionales en $[0,1]$, cuya medida de Lebesgue es exactamente 0 (conjunto numerable). La preimagen del pago 0 son los irracionales, cuya medida es 1. La esperanza se calcula analíticamente: $\mathbb{E}[X] = 1000(0) + 0(1) = 0$. Esto demuestra que tener infinitos puntos no equivale a poseer masa probabilística positiva.</p>
</details>

<details>
<summary><strong>8) ¿Qué es exactamente la “Paradoja del Cero” en probabilidad continua?</strong></summary>
<br>
<p>La Paradoja del Cero es una aparente contradicción lógica que surge al aplicar intuiciones discretas a espacios continuos reales. Se resume en el contraste entre el hecho matemático de que la probabilidad de que ocurra un evento puntual específico es estrictamente cero ($\mathbb{P}(\{x\}) = 0$) y la realidad física de que dicho evento, de hecho, ocurre al realizar el experimento.</p>
<p>En un modelo continuo (como elegir un real uniforme en $[0,1]$), existen infinitas opciones no numerables. El "área bajo la curva" para un único punto geométrico carece de anchura, resultando en probabilidad nula. La resolución de la paradoja exige comprender que "medida nula" es un concepto analítico de peso relativo frente al dominio total, no un sinónimo de "imposibilidad lógica" (representada exclusivamente por el conjunto vacío $\emptyset$).</p>
</details>

<details>
<summary><strong>9) ¿Cómo se utiliza el concepto de “bits” para explicar la transición de un modelo discreto a uno continuo?</strong></summary>
<br>
<p>Modelar un número continuo en el intervalo $[0,1]$ computacionalmente se logra discretizándolo mediante una cantidad $b$ de bits, lo que genera un espacio muestral de cardinalidad $N=2^b$.</p>
<p>Si se utilizan pocos bits (ej. $b=5$), el espacio tiene solo 32 valores posibles, creando una cuadrícula gruesa donde las probabilidades de repetición son altísimas. A medida que $b \to \infty$ (ej. 60 bits, $\sim 10^{18}$ valores), la cuadrícula (granularidad $2^{-b}$) se vuelve tan fina que emula el continuo real. La transición conceptual ocurre cuando el tamaño del espacio crece exponencialmente, haciendo que la probabilidad de extraer el mismo elemento se pulverice y colapse asintóticamente hacia cero.</p>
</details>

<details>
<summary><strong>10) ¿Qué es el “umbral del cumpleaños” y por qué es crítico en el análisis probabilístico de colisiones?</strong></summary>
<br>
<p>El umbral del cumpleaños cuantifica la sorpresiva rapidez con la que aparecen colisiones al extraer muestras aleatorias uniformes de un conjunto finito de tamaño $N$.</p>
<p>Matemáticamente, la probabilidad de que al menos dos muestras colisionen alcanza el 50% mucho antes de extraer $N/2$ elementos. La expansión de Taylor revela que este umbral crece proporcionalmente a $\sqrt{N}$. En un sistema modelado con $b$ bits ($N=2^b$), el umbral escala en el orden de $\sqrt{2^b} = 2^{b/2}$. Entender esta dinámica exponencial es crítico (por ejemplo, en criptografía y diseño de funciones Hash) para demostrar que en espacios inmensos las colisiones ocurren muchísimo antes de lo que dicta la intuición humana.</p>
</details>

<details>
<summary><strong>11) ¿Por qué en el límite estricto continuo “cada punto tiene probabilidad 0” y cuál es la lectura correcta de este fenómeno?</strong></summary>
<br>
<p>En un marco continuo regido por la Teoría de la Medida, el espacio muestral está compuesto por un continuo no numerable. Si asignáramos a un solo punto una probabilidad uniforme estrictamente mayor que cero (digamos $\epsilon>0$), por el axioma de aditividad numerable de Kolmogorov, la suma de las probabilidades de una infinidad de puntos tendería a infinito, violando la ley inquebrantable de que la probabilidad total debe ser 1.</p>
<p>La lectura teórica correcta es que la masa probabilística en el continuo no reside en los puntos aislados, sino en los intervalos medibles. Un evento de medida nula es simplemente aquel que carece de extensión geométrica (como el diferencial $dx$) para acumular densidad de probabilidad.</p>
</details>

<details>
<summary><strong>12) ¿Qué significa matemáticamente que la probabilidad de repetición “colapsa hacia el cero absoluto” al aumentar la resolución del espacio?</strong></summary>
<br>
<p>Al fijar un número constante de ensayos $n$ y estudiar la probabilidad de extraer dos valores idénticos, esta métrica depende inversamente del tamaño del espacio de estados $N$.</p>
<p>Para $n=1000$, si la resolución aumenta ($N \to \infty$), la probabilidad de colisión (regida asintóticamente por $1 - e^{-n^2/2N}$) se altera. Al crecer $N$ enormemente en el denominador, el exponente tiende a 0, haciendo que $e^0 \to 1$, y la probabilidad total converja a $1 - 1 = 0$. Este "colapso" no indica imposibilidad ontológica, sino que la escala de ensayos requeridos para presenciar el evento se vuelve inalcanzable operativamente.</p>
</details>

<details>
<summary><strong>13) ¿Qué son las “desigualdades de concentración” y por qué se las considera universales?</strong></summary>
<br>
<p>Las desigualdades de concentración son teoremas analíticos que permiten acotar superiormente la probabilidad de que una variable aleatoria tome valores alejados a su esperanza matemática (el comportamiento de sus colas).</p>
<p>Son consideradas herramientas universales (<i>distribution-free</i>) porque no requieren suponer que los datos sigan una distribución Gaussiana, continua o simétrica. Imponen límites matemáticos infranqueables "en el peor de los casos" valiéndose únicamente de momentos estadísticos básicos (media, varianza), actuando como garantes teóricos en entornos de alta incertidumbre.</p>
</details>

<details>
<summary><strong>14) Enuncia la desigualdad de Markov, enumera sus condiciones y proporciona una interpretación intuitiva sólida.</strong></summary>
<br>
<p>La desigualdad de Markov postula que para toda variable aleatoria estrictamente no negativa ($Z \ge 0$) y toda constante $a > 0$:</p>
$$\mathbb{P}(Z \ge a) \le \frac{\mathbb{E}[Z]}{a}$$
<p>Las condiciones vitales son la no-negatividad (evita que valores negativos extremos compensen espuriamente la media) y poseer un primer momento finito. Intuitivamente: "Si el promedio de un sistema cerrado es bajo, es imposible que una gran fracción de la población registre valores descomunales". Por ejemplo, si el salario medio es de \$1,000, es matemáticamente imposible que más del 10% de la muestra gane \$10,000 o más; dicha subpoblación por sí sola rompería la media global.</p>
</details>

<details>
<summary><strong>15) Enuncia la desigualdad de Chebyshev, detalla sus requerimientos y cómo se interpreta operando con $t=k\sigma$.</strong></summary>
<br>
<p>La desigualdad de Chebyshev afirma que para toda variable $X$ con esperanza $\mu$ y varianza finita $\mathrm{Var}(X)$, para cualquier distancia $t > 0$:</p>
$$\mathbb{P}(|X-\mu| \ge t) \le \frac{\mathrm{Var}(X)}{t^2}$$

<p>Al parametrizar la distancia en desviaciones estándar ($t=k\sigma$, con $\sigma=\sqrt{\mathrm{Var}(X)}$), se obtiene:</p>
$$\mathbb{P}(|X-\mu| \ge k\sigma) \le \frac{1}{k^2}$$
<p>El corolario analítico es profundo: sin conocer la distribución subyacente, se garantiza que la masa probabilística a más de $k$ desviaciones del centro jamás superará $1/k^2$. Para $k=3$, la cota superior estricta es $1/9 \approx 11.1\%$.</p>
</details>

<details>
<summary><strong>16) ¿Qué significa que la cota de Chebyshev sea “ajustada” (tight) y qué rol juega la distribución “Spike”?</strong></summary>
<br>
<p>Que una cota sea "ajustada" (<i>tight</i>) significa que no es una aproximación holgada; existe al menos un caso patológico real donde la desigualdad es una igualdad estricta. La cota no admite mejoras matemáticas sin sacrificar universalidad.</p>
<p>La distribución "Spike" (de tres átomos) materializa este peor escenario. Asigna una masa de $1/(2k^2)$ a los extremos $\mu-k\sigma$ y $\mu+k\sigma$, centralizando el resto ($1-1/k^2$) exactamente en $\mu$. Al evaluarla bajo Chebyshev, la masa real en las colas iguala milimétricamente la cota $1/k^2$, demostrando que el teorema está perfectamente calibrado para el nivel máximo de dispersión posible.</p>
</details>

<details>
<summary><strong>17) ¿De qué manera la integral de Lebesgue interpreta y calcula una esperanza como la suma de “premio × medida del conjunto que lo produce”?</strong></summary>
<br>
<p>Lebesgue abandona el escaneo secuencial del dominio temporal (Riemann) y adopta una agregación por niveles funcionales.</p>
<p>Identifica un "premio" $k$ en el codominio y agrupa todos los eventos atómicos heterogéneos en el espacio muestral que desencadenan dicho premio. Este supra-conjunto es la preimagen $X^{-1}(\{k\})$. Acto seguido, calcula la medida total (probabilidad $\mathbb{P}$) de esta preimagen. La esperanza es simplemente la combinatoria lineal de estos estratos funcionales:</p>
$$\mathbb{E}[X] = \sum_k k \cdot \mathbb{P}(X=k)$$
<p>Integrar, bajo Lebesgue, es ponderar los valores escalares de la variable por la medida volumétrica exacta de sus preimágenes algebraicas.</p>
</details>

<details>
<summary><strong>18) ¿Qué conexión teórica subyace entre el ejemplo de “racionales vs irracionales” y el concepto central de agrupación por niveles y preimágenes?</strong></summary>
<br>
<p>La asignación de pagos binarios (1000 a $\mathbb{Q}$, 0 a $\mathbb{I}$) expone el fracaso de la topología local ante funciones con alta discontinuidad. Al ser conjuntos densos en los reales, el intento de integración geométrica colapsa.</p>
<p>La teoría de preimágenes elude esta geografía fractal. La preimagen del nivel 1000 aglutina todos los racionales en un ente único (medida 0). La preimagen del nivel 0 agrupa los irracionales (medida 1). La resolución funcional ignora la vecindad espacial de los puntos y opera exclusivamente sobre el tamaño medible de los conjuntos preimagen, confirmando la superioridad de Lebesgue en topologías complejas.</p>
</details>

<details>
<summary><strong>19) ¿Cómo se aplica la desigualdad de Markov para establecer “garantías de sistema” y analizar la latencia en ciencias de la computación?</strong></summary>
<br>
<p>En el diseño de sistemas concurrentes o análisis de algoritmos aleatorizados, la distribución subyacente de la latencia (una variable estrictamente no-negativa) suele ser opaca o de colas asimétricas, volviendo inaplicables los modelos Gaussianos.</p>
<p>Markov actúa como un blindaje estocástico. Si un analista de datos conoce el tiempo medio de respuesta $\mu$, el teorema garantiza irrefutablemente que la probabilidad de sufrir un pico de latencia del orden de $10\mu$ jamás excederá el 10% de las transacciones ($\mathbb{P}(Z \ge 10\mu) \le 1/10$). Esto faculta a los ingenieros a firmar Acuerdos de Nivel de Servicio (SLAs) con certezas matemáticas hard-coded, libres de presunciones empíricas.</p>
</details>

<details>
<summary><strong>20) ¿De qué manera la desigualdad de Chebyshev es explotada en la “detección de anomalías” y cuál es el mensaje estadístico fundamental?</strong></summary>
<br>
<p>En analítica forense o monitoreo de fraude, clasificar anomalías asumiendo que los datos respetan la Regla Empírica Normal ($3\sigma = 0.3\%$) es altamente riesgoso ante distribuciones de cola pesada.</p>

<p>Chebyshev proporciona el filtro conservador definitivo. Demuestra que incluso en la topología más caótica imaginable con varianza finita, el límite absoluto de observaciones que exceden las $3\sigma$ está rígidamente fijado en $1/3^2 \approx 11.1\%$. El mensaje estadístico cardinal es el <i>diseño robusto</i>: la interrogante forense óptima no es indagar probabilidades exactas bajo normalidad ilusoria, sino establecer la peor desviación matemática garantizable. Un dato que quiebra el umbral de Chebyshev es, innegablemente, una anomalía estructural severa.</p>
</details>

---

| 📄 Recurso | 📥 Acceso |
| --- | --- |
| **01. La Geometría de la Aleatoriedad** <br>

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

