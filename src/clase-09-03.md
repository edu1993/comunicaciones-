# COMUNICACIONES — 9 DE MARZO

## Repaso: Contenido Previo

### Definición de $f(t)$
La función del tiempo asigna un **único valor de amplitud** para cada instante. Trabajamos directamente con el dominio del tiempo ($t$).

### Funciones Angulares
$$A(t) = A \cdot \cos\left(\frac{t}{2\pi}\right)$$

> **Nota:** El argumento de la función debe estar siempre en **radianes**.

---

### Análisis del Periodo ($$T$$)
La función se repite cíclicamente. Según el gráfico:
* El periodo es $2\pi$.
* Relación fundamental: $2\pi \longrightarrow T$ (donde $T$ es el periodo).

**Conversión Universo Tiempo:**
Para relacionar el ángulo $\theta$ con el tiempo $t$:
$$\theta = \frac{2\pi \cdot t}{T}$$



---

### Funciones por Trozos

#### 1. Función Cajón (Unitario)
También expresada como $\Pi(t - 1/2)$. Se define matemáticamente como:

$$x(t) = \begin{cases} 1 & |t| < 1 \\ 0 & |t| > 1 \end{cases}$$

* **Gráfico:** Pulso rectangular de amplitud $1$ en el intervalo $(-1, 1)$.



#### 2. Función Unitaria (Escalón)
Denotada como $u(t)$. Representa un cambio de estado que se mantiene en $1$ para todo $t > 0$.



---

### Análisis de Funciones
$$\sum_{n=1}^{\infty} n = 36$$
*(Gráfico de una función constante $x(t) = 36$ sobre el eje $T$)*

---

#### Función Sinc
$$\text{Sinc}(T) = \frac{\sin(\pi T)}{\pi T}$$

* **Propiedad:** NO es periódica.
* **Decaimiento:** Es de $\frac{1}{T}$.



---

### CONCEPTOS CLAVE

* **Sistema de Comunicaciones:** Sistema de transmisión de datos en formato binario. Todo se transforma en una cadena de bits.
* **Arquitectura Informática:** Define el sistema (ej. `x86`, `ARM`, `MIPS`).
* **Sistema Embebido:** Orientado a una solución o actividad específica.
* **Interfaz, Norma y Protocolo:**
    * **Interfaz:** Conexión física/lógica del sistema.
    * **Norma:** Reglas de desarrollo.
    * **Protocolo:** Cómo se ejecutan/usan esas reglas.

---

### SISTEMAS DE COMUNICACIONES DIGITALES
Modelamos el sistema a través de un **Canal (medio físico)** que une Emisor y Receptor.

**Componentes del Modelo:**
* **F $\implies$ Fuente:** Origina los datos.
* **TX $\implies$ Transmisor:** Adapta los datos al canal.
* **Mensaje:** Soporte que viaja por el canal (no contiene la información en sí, sino la señal).
* **RX $\implies$ Receptor:** Estima el mensaje original.
* **D $\implies$ Destino:** Receptor final de la información.
* **Ruido:** Perturbación inevitable del canal que genera distorsión.

---

### LATENCIA
Es el tiempo esperado $\tau$ que tarda el mensaje en viajar de un punto a otro.



**Diagrama de flujo del mensaje:**
$$(F) \xrightarrow{M_f} [TX] \xrightarrow{M_{tx}} [CH] \xrightarrow{M_{ch}} \oplus \xrightarrow{N(t)} [RX] \xrightarrow{M_{rx}} (D)$$

* **$N(t) \implies$ Ruido:** Se suma en el canal. Solo se puede mitigar.

---

### Modelo de Shannon (Modelo Sistémico)
Este modelo permite analizar el sistema como una **Caja Negra**.
* Se enfoca en el *input* y el *output*.
* No requiere conocer el proceso interno exacto, lo que simplifica el análisis de sistemas complejos.
