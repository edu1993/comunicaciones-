# COMUNICACIONES — 9 DE MARZO
## Repaso: Contenido Previo

### Definición de $f(t)$
La función del tiempo asigna un **único valor de amplitud** para cada instante. Trabajamos directamente con el dominio del tiempo ($t$).

### Funciones Angulares
$$A(t) = A \cdot \cos\left(\frac{t}{2\pi}\right)$$
> **Nota:** El argumento de la función debe estar siempre en **radianes**.

---

### Análisis del Periodo ($T$)
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
Denotada como $u(t)$.
* Representa un cambio de estado que se mantiene en $1$ para todo $t > 0$.




#### Análisis de Funciones
$$\sum_{n=1}^{\infty} n = 36$$
(Gráfico de una función constante $x(t) = 36$ sobre el eje $T$)

---

#### Función Sinc
$$\frac{\text{sen}(*) }{*}$$
* **Propiedad:** NO es periódica.
* **Decaimiento:** Es de $\frac{1}{T}$.
* **Definición:** $$Sinc(T) = \frac{\text{sen}(\pi T)}{\pi T}$$

(Gráfico de la función Sinc mostrando el lóbulo principal centrado en el origen y lóbulos secundarios amortiguados).

---

### EXPLICACIONES

#### ¿Qué es un Sistema de Comunicaciones?
Es un **Sistema de Transmisión de Datos** (en formato numérico binario).
* Todo lo que queremos transmitir se transforma en una **cadena de bits**.

#### ¿Qué es una Arquitectura Informática?
La arquitectura define el **Sistema Informático**.
* Ejemplos: `x86`, `ARM`, `MIPS`.
* Una misma arquitectura puede tener varios sistemas.

#### ¿Qué es un Sistema Embebido?
Un sistema que está orientado a una **solución o actividad específica**.

#### ¿Qué es Interfaz, Norma y Protocolo?
* **Interfaz:** Desarrollo sistema.
* **Norma:** Reglas desarrollo.
* **Protocolo:** Cómo [se usan] esas reglas.

**Ejemplos mencionados:**
`I2C`, `Radio`, `USB`, `WIFI`, `BT` (Bluetooth), `PS/2`, `SATA`, `HDMI`, `Ethernet`, `Audio In`.


#### Diferencia entre un sistema Analógico y Digital
* **Analógico:** Señales continuas.

#### ¿Qué es la Convergencia Informática?
Varios sistemas de comunicación en un solo lugar (ejemplo: TV y Radio por Internet). Migración a un solo soporte.

---

### LIBROS DE REFERENCIA
* **Transmisión Digital de Información** - Cesar Juarez Vargas.
* **Tomasi**.

---

### SISTEMAS DE COMUNICACIONES DIGITALES
* Transferencia de datos numéricos `"1011"` $\longrightarrow$ Número binario.
* El primer sistema digital fue el **Morse**.

#### ¿Cómo modelamos un sistema de comunicaciones?
Lo primero que necesitamos es un **Canal (medio físico)**, es lo que va a unir dos puntos (Emisor, Receptor).


**Componentes del Modelo:**
* **F $\implies$ Fuente:** Quien emite los datos.
* **TX $\implies$ Transmisor:** Quien adapta los datos al canal.
* **Mensaje $\implies$** Donde van a ir los datos, no lleva información [directamente].
* **RX $\implies$ Receptor:** Convierte el mensaje, estimándolo.
* **D $\implies$ Destino/Receptor final.**
* **Ruido $\implies$** Señal que provoca el canal, sucede en todos los canales. Genera distorsión.

**Éxito en la Comunicación:**
Podemos decir que la comunicación fue exitosa cuando el mensaje llega en cierto **tiempo esperado**.

**El Error:**
Significa que cuando envío un mensaje llega otro. ¡Se da en el **RX** al hacer la estimación!

### Continuación de Apuntes: Comunicaciones (Página 4)

El mensaje va a salir desde la fuente al destino cambiando su forma en cada una de las instancias.

**Diagrama de flujo del mensaje:**
$$(F) \xrightarrow{M_f} [TX] \xrightarrow{M_{tx}} [CH] \xrightarrow{M_{ch}} \oplus \xrightarrow{N(t)} [RX] \xrightarrow{M_{rx}} (D)$$

* **$N(t) \implies$ Ruido:** Se suma. No se puede sacar, pero sí mitigar.
* El mensaje va cambiando de acuerdo al sistema.
* **TX $\implies$** Adapta el mensaje al canal.

---

### LATENCIA
En los sistemas de comunicaciones reales (físicos), la salida del mensaje tarda en llegar de un punto a otro. **Ese tiempo es la latencia.**


* **Gráfico de Latencia:** Muestra un pulso binario `"101"` que sale de la fuente en $t=0$ y llega al receptor con un desplazamiento temporal ($\tau$).
* El mensaje tarda un cierto tiempo $\tau$.
* El tiempo $\tau$ se produce dentro de la fuente.

---

### Sistema de Comunicaciones
Se define bajo estas premisas para su estudio:
* **Invariante en el tiempo.**
* **Lineal.**
* Como sistema físico, va a tener una latencia; no va a ser instantáneo.

---

### Modelo de Shannon (Modelo Sistémico)
Este modelo de comunicaciones es el de **Shannon**.
* **Modelo de Caja Negra:** Sabemos el *input* y el *output*, pero no [necesariamente] lo que pasa en el medio. Ayuda a simplificar modelos complejos.
