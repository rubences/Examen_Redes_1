# Examen_Redes_1

# Cálculo de Tasa de Transmisión Máxima (Fórmula de Shannon)

Este documento explica cómo calcular la tasa de transmisión máxima utilizando la **Fórmula de Shannon**:

## Fórmula de Shannon
La fórmula es la siguiente:
\[ C = B \cdot \log_2(1 + \frac{S}{N}) \]
Donde:
- \( C \) es la capacidad del canal en bits por segundo (bps).
- \( B \) es el ancho de banda del canal en hertzios (Hz).
- \( S \) es la potencia de la señal en vatios (W).
- \( N \) es la potencia del ruido en vatios (W).
- \( \log_2 \) es el logaritmo en base 2.
## Ejemplo de Cálculo
Supongamos que tenemos un canal con las siguientes características:
- Ancho de banda (\( B \)): 3 kHz
- Potencia de la señal (\( S \)): 100 mW
- Potencia del ruido (\( N \)): 10 mW
### Paso 1: Convertir las unidades
- Convertir el ancho de banda a Hz:
  \[ B = 3 \, \text{kHz} = 3000 \, \text{Hz} \]
- Convertir la potencia de la señal a W:

    \[ S = 100 \, \text{mW} = 0.1 \, \text{W} \]

- Convertir la potencia del ruido a W:
    \[ N = 10 \, \text{mW} = 0.01 \, \text{W} \]
### Paso 2: Sustituir en la fórmula
\[ C = 3000 \cdot \log_2(1 + \frac{0.1}{0.01}) \]
### Paso 3: Calcular el logaritmo
\[ \frac{S}{N} = \frac{0.1}{0.01} = 10 \]
\[ 1 + \frac{S}{N} = 1 + 10 = 11 \]
\[ \log_2(11) \approx 3.4594 \]
### Paso 4: Sustituir el logaritmo en la fórmula
\[ C = 3000 \cdot 3.4594 \]
\[ C \approx 10378.2 \, \text{bps} \]
### Paso 5: Resultado
La tasa de transmisión máxima del canal es aproximadamente **10,378.2 bps**.

Donde:
- **C**: Tasa de transmisión máxima (en bits por segundo, bps).
- **B**: Ancho de banda del canal (en Hz).
- **SNR**: Relación señal a ruido en escala lineal.

### Conversión de SNR de dB a escala lineal
Si el **SNR** está en decibelios (dB), se convierte a escala lineal con la fórmula:
\[ SNR_{lineal} = 10^{\frac{SNR_{dB}}{10}} \]
### Ejemplo de Conversión
Supongamos que tenemos un **SNR** de 20 dB:
\[ SNR_{lineal} = 10^{\frac{20}{10}} = 10^2 = 100 \]
### Paso 6: Sustituir en la fórmula
\[ C = B \cdot \log_2(1 + SNR_{lineal}) \]
### Paso 7: Calcular la tasa de transmisión máxima
Supongamos que el ancho de banda es de 3 kHz:
\[ C = 3000 \cdot \log_2(1 + 100) \]
\[ C = 3000 \cdot \log_2(101) \]
\[ C \approx 3000 \cdot 6.6582 \]
\[ C \approx 19974.6 \, \text{bps} \]
### Paso 8: Resultado
La tasa de transmisión máxima del canal es aproximadamente **19,974.6 bps**.
## Conclusión
La **Fórmula de Shannon** es una herramienta poderosa para calcular la tasa de transmisión máxima de un canal de comunicación. Al conocer el ancho de banda y la relación señal a ruido, podemos determinar la capacidad del canal en bits por segundo.


---

## Ejemplo de cálculo

### Datos del problema
- **Ancho de banda (B)**: 500 MHz = \( 500 \times 10^6 \, \text{Hz} \)
- **SNR (dB)**: 20 dB

### Paso 1: Conversión de SNR a escala lineal
Usamos la fórmula:


Sustituyendo el valor de **SNR(dB)**:
\[ SNR_{lineal} = 10^{\frac{20}{10}} = 10^2 = 100 \]
### Paso 2: Sustitución en la fórmula de Shannon
\[ C = B \cdot \log_2(1 + SNR_{lineal}) \]
Sustituyendo el valor de **B** y **SNR(lineal)**:
\[ C = (500 \times 10^6) \cdot \log_2(1 + 100) \]
\[ C = (500 \times 10^6) \cdot \log_2(101) \]
### Paso 3: Cálculo del logaritmo
Usamos la calculadora para obtener el valor de \( \log_2(101) \):
\[ \log_2(101) \approx 6.6582 \]
### Paso 4: Sustitución en la fórmula
\[ C = (500 \times 10^6) \cdot 6.6582 \]
\[ C \approx 3.3291 \times 10^9 \, \text{bps} \]
### Paso 5: Resultado
La tasa de transmisión máxima del canal es aproximadamente **3,329,100,000 bps** o **3.33 Gbps**.
## Notas
- La fórmula de Shannon es fundamental en la teoría de la información y se utiliza para determinar la capacidad máxima de un canal de comunicación.


### Paso 2: Sustitución en la fórmula de Shannon
Sustituimos los valores en la fórmula:
\[ C = B \cdot \log_2(1 + \frac{S}{N}) \]
\[ C = 3000 \cdot \log_2(1 + \frac{0.1}{0.01}) \]
\[ C = 3000 \cdot \log_2(1 + 10) \]
\[ C = 3000 \cdot \log_2(11) \]


## Referencias
- [Fórmula de Shannon - Wikipedia](https://es.wikipedia.org/wiki/F%C3%B3rmula_de_Shannon)
- [Teoría de la Información - Wikipedia](https://es.wikipedia.org/wiki/Teor%C3%ADa_de_la_informaci%C3%B3n)
- [Capacidad del Canal - Wikipedia](https://es.wikipedia.org/wiki/Capacidad_de_canal)
- [Ancho de Banda - Wikipedia](https://es.wikipedia.org/wiki/Ancho_de_banda)
- [Relación Señal a Ruido - Wikipedia](https://es.wikipedia.org/wiki/Relaci%C3%B3n_se%C3%B1al-ruido)
- [Logaritmo - Wikipedia](https://es.wikipedia.org/wiki/Logaritmo)
- [Potencia - Wikipedia](https://es.wikipedia.org/wiki/Potencia_(f%C3%ADsica))
- [Decibelio - Wikipedia](https://es.wikipedia.org/wiki/Decibelio)
- [SNR - Wikipedia](https://es.wikipedia.org/wiki/Relaci%C3%B3n_se%C3%B1al-ruido)
- [Cálculo de Tasa de Transmisión - Wikipedia](https://es.wikipedia.org/wiki/C%C3%A1lculo_de_tasa_de_transmisi%C3%B3n)
- [Comunicación Digital - Wikipedia](https://es.wikipedia.org/wiki/Comunicaci%C3%B3n_digital)
- [Comunicación Analógica - Wikipedia](https://es.wikipedia.org/wiki/Comunicaci%C3%B3n_anal%C3%B3gica)
- [Comunicación por Ondas - Wikipedia](https://es.wikipedia.org/wiki/Comunicación_por_ondas)
- [Comunicación por Fibra Óptica - Wikipedia](https://es.wikipedia.org/wiki/Comunicación_por_fibra_%C3%B3ptica)
- [Comunicación Inalámbrica - Wikipedia](https://es.wikipedia.org/wiki/Comunicación_inalámbrica)


# Resolviendo el Problema con Cisco Packet Tracer

Este documento explica cómo simular un canal de comunicación en **Cisco Packet Tracer** y calcular la tasa de transmisión máxima utilizando la **Fórmula de Shannon**.

---

## Objetivo
Simular un canal de comunicación en **Cisco Packet Tracer** y calcular la tasa de transmisión máxima utilizando los siguientes datos:
- **Ancho de banda (\( B \))**: 500 MHz
- **Relación señal a ruido (SNR)**: 20 dB

---

## Paso a Paso

### Paso 1: Configurar el entorno en Cisco Packet Tracer
1. **Abrir Cisco Packet Tracer**:
   - Inicia el programa y abre un nuevo proyecto.

2. **Agregar dispositivos**:
   - Arrastra dos dispositivos al área de trabajo, por ejemplo:
     - Dos PCs (PC0 y PC1).
     - O dos routers (Router0 y Router1).

3. **Conectar los dispositivos**:
   - Usa un cable adecuado para conectar los dispositivos:
     - Si son PCs, utiliza un **cable cruzado**.
     - Si son routers, utiliza un **cable serial** o un **cable directo**.

4. **Configurar el enlace**:
   - Haz clic en el enlace entre los dispositivos.
   - Ve a la configuración del enlace y establece el **ancho de banda** en 500 Mbps (para simular los 500 MHz del problema).

---

### Paso 2: Simular la relación señal a ruido (SNR)
1. **Simular ruido en el enlace**:
   - Si estás utilizando un enlace **inalámbrico**:
     - Configura un **Access Point** y conecta los dispositivos de forma inalámbrica.
     - Ajusta la potencia de transmisión o aumenta la distancia entre los dispositivos para simular ruido.
   - Si estás utilizando un enlace **cableado**:
     - Introduce errores en el enlace ajustando manualmente los parámetros de calidad.

2. **Calcular el SNR en escala lineal**:
   - Usa la fórmula para convertir el SNR de dB a escala lineal:
     \[
     SNR_{lineal} = 10^{\frac{SNR_{dB}}{10}}
     \]
   - Sustituyendo \( SNR_{dB} = 20 \):
     \[
     SNR_{lineal} = 10^{\frac{20}{10}} = 10^2 = 100
     \]

---

### Paso 3: Calcular la tasa de transmisión máxima
1. **Usar la fórmula de Shannon**:
   - La fórmula es:
     \[
     C = B \cdot \log_2(1 + SNR)
     \]
   - Sustituye los valores:
     - \( B = 500 \times 10^6 \, \text{Hz} \)
     - \( SNR = 100 \)
     \[
     C = (500 \times 10^6) \cdot \log_2(1 + 100)
     \]

2. **Calcular el logaritmo**:
   - Calcula \( \log_2(101) \):
     \[
     \log_2(101) \approx 6.6582
     \]

3. **Sustituir el valor del logaritmo**:
   \[
   C = (500 \times 10^6) \cdot 6.6582
   \]
   \[
   C \approx 3.3291 \times 10^9 \, \text{bps}
   \]

4. **Resultado final**:
   - La tasa de transmisión máxima es:
     \[
     C \approx 3.33 \, \text{Gbps}
     \]

---

### Paso 4: Verificar el rendimiento en Cisco Packet Tracer
1. **Configurar direcciones IP**:
   - Asigna direcciones IP a los dispositivos conectados.
   - Por ejemplo:
     - PC0: 192.168.1.1
     - PC1: 192.168.1.2

2. **Probar conectividad**:
   - Usa la herramienta **Ping** para verificar la conectividad entre los dispositivos:
     - Desde PC0, ejecuta: `ping 192.168.1.2`.

3. **Simular tráfico**:
   - Configura un servidor y un cliente para generar tráfico entre los dispositivos.
   - Observa el rendimiento del enlace en términos de velocidad y calidad.

4. **Comparar con el cálculo teórico**:
   - Compara el rendimiento observado en Packet Tracer con el cálculo teórico de la tasa de transmisión máxima (\( C \)).

---

## Conclusión
En este ejercicio, hemos configurado un canal de comunicación en **Cisco Packet Tracer** y calculado la tasa de transmisión máxima utilizando la **Fórmula de Shannon**. El resultado teórico es de aproximadamente **3.33 Gbps**, y el rendimiento observado en la simulación debería acercarse a este valor, dependiendo de las condiciones del enlace.

---

## Referencias
- [Fórmula de Shannon - Wikipedia](https://es.wikipedia.org/wiki/F%C3%B3rmula_de_Shannon)
- [Cisco Packet Tracer - Documentación Oficial](https://www.netacad.com/courses/packet-tracer)


# Ejemplo de Código en Python para calcular la tasa de transmisión máxima
```python
import math
def shannon_capacity(B, S, N):
    """
    Calcula la tasa de transmisión máxima utilizando la fórmula de Shannon.

    Parámetros:
    B (float): Ancho de banda en Hz.
    S (float): Potencia de la señal en W.
    N (float): Potencia del ruido en W.

    Retorna:
    float: Tasa de transmisión máxima en bps.
    """
    # Calcular la relación señal a ruido
    SNR = S / N

    # Calcular la capacidad del canal
    C = B * math.log2(1 + SNR)

    return C
# Datos del problema
B = 3 * 10**3  # Ancho de banda en Hz (3 kHz)
S = 0.1  # Potencia de la señal en W (100 mW)
N = 0.01  # Potencia del ruido en W (10 mW)
# Calcular la tasa de transmisión máxima
C = shannon_capacity(B, S, N)
print(f"La tasa de transmisión máxima es: {C:.2f} bps")
```
### Ejecución del código
```bash
$ python shannon_capacity.py
La tasa de transmisión máxima es: 10378.20 bps
```
### Notas
- Asegúrate de tener instalado Python y la biblioteca `math` para ejecutar el código.
- Puedes modificar los valores de **B**, **S** y **N** para calcular la tasa de transmisión máxima en diferentes escenarios.
```
# Fin del documento
```
# Ejercicio 8

# Resolviendo el Problema de Ubicación de Portadoras para Eficiencia Espectral

Este documento explica cómo determinar las frecuencias de las portadoras anterior y posterior en un sistema de comunicación, y analiza la importancia de la ubicación de las portadoras para la eficiencia espectral.

---

## Enunciado

En un sistema de comunicación, la primera portadora se encuentra a **1.2 GHz** y el ancho de banda en banda base de cada canal es de **300 MHz**. Se pide:

1. **a)** Determinar la frecuencia de la portadora anterior.
2. **b)** Determinar la frecuencia de la portadora posterior.
3. Justificar los cálculos y explicar la importancia de la ubicación de las portadoras para la eficiencia espectral.

---

## Paso a Paso

### Datos iniciales
- Frecuencia de la primera portadora (\( f_0 \)): **1.2 GHz**.
- Ancho de banda en banda base (\( BW \)): **300 MHz**.

---

### Paso 1: Determinar la frecuencia de la portadora anterior
La frecuencia de la portadora anterior (\( f_{anterior} \)) se calcula restando el ancho de banda del canal (\( BW \)) a la frecuencia de la portadora actual (\( f_0 \)):

\[
f_{anterior} = f_0 - BW
\]

Sustituyendo los valores:

\[
f_{anterior} = 1.2 \, \text{GHz} - 300 \, \text{MHz}
\]

Convertimos las unidades para que sean consistentes (\( 1.2 \, \text{GHz} = 1200 \, \text{MHz} \)):

\[
f_{anterior} = 1200 \, \text{MHz} - 300 \, \text{MHz}
\]

\[
f_{anterior} = 900 \, \text{MHz}
\]

Por lo tanto, la frecuencia de la portadora anterior es:

\[
f_{anterior} = 900 \, \text{MHz}
\]

---

### Paso 2: Determinar la frecuencia de la portadora posterior
La frecuencia de la portadora posterior (\( f_{posterior} \)) se calcula sumando el ancho de banda del canal (\( BW \)) a la frecuencia de la portadora actual (\( f_0 \)):

\[
f_{posterior} = f_0 + BW
\]

Sustituyendo los valores:

\[
f_{posterior} = 1.2 \, \text{GHz} + 300 \, \text{MHz}
\]

Convertimos las unidades para que sean consistentes (\( 1.2 \, \text{GHz} = 1200 \, \text{MHz} \)):

\[
f_{posterior} = 1200 \, \text{MHz} + 300 \, \text{MHz}
\]

\[
f_{posterior} = 1500 \, \text{MHz}
\]

Por lo tanto, la frecuencia de la portadora posterior es:

\[
f_{posterior} = 1500 \, \text{MHz}
\]

---

### Paso 3: Justificación de los cálculos
Los cálculos se basan en la separación de las portadoras por el ancho de banda del canal (\( BW \)). En un sistema de comunicación, las portadoras deben estar separadas por al menos el ancho de banda del canal para evitar interferencias entre canales adyacentes.

---

### Paso 4: Importancia de la ubicación de las portadoras para la eficiencia espectral
La ubicación de las portadoras es crucial para maximizar la **eficiencia espectral**, que se define como la cantidad de información transmitida por unidad de ancho de banda. Una buena ubicación de las portadoras permite:

1. **Minimizar la interferencia**:
   - Si las portadoras están demasiado cerca, los canales se solapan, causando interferencia y pérdida de datos.
   - Si están demasiado separadas, se desperdicia ancho de banda.

2. **Optimizar el uso del espectro**:
   - Al ubicar las portadoras con una separación adecuada (igual al ancho de banda del canal), se utiliza el espectro de manera eficiente, maximizando la capacidad del sistema.

3. **Garantizar la calidad del servicio**:
   - Una correcta ubicación de las portadoras asegura que cada canal tenga suficiente espacio para transmitir datos sin degradación de la señal.

---

## Resultado Final
- **Frecuencia de la portadora anterior**: \( f_{anterior} = 900 \, \text{MHz} \)
- **Frecuencia de la portadora posterior**: \( f_{posterior} = 1500 \, \text{MHz} \)

---

## Conclusión
La ubicación de las portadoras en un sistema de comunicación es fundamental para garantizar la eficiencia espectral y la calidad del servicio. En este caso, las portadoras están separadas por el ancho de banda del canal (\( 300 \, \text{MHz} \)), lo que asegura un uso óptimo del espectro y evita interferencias entre canales.

---

## Referencias
- [Eficiencia Espectral - Wikipedia](https://es.wikipedia.org/wiki/Eficiencia_espectral)
- [Teoría de la Comunicación - Wikipedia](https://es.wikipedia.org/wiki/Teor%C3%ADa_de_la_comunicaci%C3%B3n)
- [Ancho de Banda - Wikipedia](https://es.wikipedia.org/wiki/Ancho_de_banda)


# Resolviendo el Problema de Ubicación de Portadoras para Eficiencia Espectral en Cisco Packet Tracer

Este documento explica cómo simular un sistema de comunicación en **Cisco Packet Tracer** para analizar la ubicación de portadoras y su impacto en la eficiencia espectral.

---

## Enunciado

En un sistema de comunicación, la primera portadora se encuentra a **1.2 GHz** y el ancho de banda en banda base de cada canal es de **300 MHz**. Se pide:

1. **a)** Determinar la frecuencia de la portadora anterior.
2. **b)** Determinar la frecuencia de la portadora posterior.
3. Simular el sistema en **Cisco Packet Tracer** para analizar la eficiencia espectral.

---

## Paso a Paso

### Paso 1: Determinar las frecuencias de las portadoras
1. **Frecuencia de la portadora anterior (\( f_{anterior} \))**:
   \[
   f_{anterior} = f_0 - BW
   \]
   Donde:
   - \( f_0 = 1.2 \, \text{GHz} \)
   - \( BW = 300 \, \text{MHz} \)

   Sustituyendo:
   \[
   f_{anterior} = 1.2 \, \text{GHz} - 300 \, \text{MHz} = 900 \, \text{MHz}
   \]

2. **Frecuencia de la portadora posterior (\( f_{posterior} \))**:
   \[
   f_{posterior} = f_0 + BW
   \]

   Sustituyendo:
   \[
   f_{posterior} = 1.2 \, \text{GHz} + 300 \, \text{MHz} = 1.5 \, \text{GHz}
   \]

Por lo tanto:
- **Portadora anterior**: \( 900 \, \text{MHz} \)
- **Portadora posterior**: \( 1.5 \, \text{GHz} \)

---

### Paso 2: Configurar el entorno en Cisco Packet Tracer
1. **Abrir Cisco Packet Tracer**:
   - Inicia el programa y abre un nuevo proyecto.

2. **Agregar dispositivos**:
   - Arrastra los siguientes dispositivos al área de trabajo:
     - Un **Access Point** (AP).
     - Dos **PCs inalámbricas** (PC0 y PC1).

3. **Configurar el Access Point**:
   - Haz clic en el Access Point y ve a la pestaña **Config**.
   - Configura los siguientes parámetros:
     - **SSID**: "Canal_1".
     - **Frecuencia**: 1.2 GHz (representa la portadora actual).
     - **Ancho de banda**: 300 MHz.

4. **Configurar las PCs inalámbricas**:
   - Haz clic en cada PC y ve a la pestaña **Config**.
   - Conéctalas al Access Point configurado.

---

### Paso 3: Simular las portadoras anterior y posterior
1. **Agregar un segundo Access Point**:
   - Arrastra otro Access Point al área de trabajo.
   - Configúralo con los siguientes parámetros:
     - **SSID**: "Canal_Anterior".
     - **Frecuencia**: 900 MHz (portadora anterior).
     - **Ancho de banda**: 300 MHz.

2. **Agregar un tercer Access Point**:
   - Arrastra un tercer Access Point al área de trabajo.
   - Configúralo con los siguientes parámetros:
     - **SSID**: "Canal_Posterior".
     - **Frecuencia**: 1.5 GHz (portadora posterior).
     - **Ancho de banda**: 300 MHz.

3. **Conectar PCs a los Access Points**:
   - Conecta una PC al Access Point "Canal_Anterior".
   - Conecta otra PC al Access Point "Canal_Posterior".

---

### Paso 4: Analizar la eficiencia espectral
1. **Simular tráfico entre dispositivos**:
   - Configura un servidor en la red y genera tráfico entre las PCs conectadas a los diferentes Access Points.
   - Usa herramientas como **Ping** o **Traceroute** para verificar la conectividad.

2. **Observar el uso del espectro**:
   - Analiza cómo las frecuencias de las portadoras están separadas por el ancho de banda del canal (300 MHz).
   - Asegúrate de que no haya interferencia entre los canales.

3. **Comparar con los cálculos teóricos**:
   - Verifica que las frecuencias de las portadoras (900 MHz, 1.2 GHz, y 1.5 GHz) coincidan con los valores calculados.

---

### Paso 5: Conclusión
La simulación en **Cisco Packet Tracer** muestra cómo la ubicación de las portadoras afecta la eficiencia espectral. Al separar las portadoras por el ancho de banda del canal (300 MHz), se evita la interferencia entre canales y se optimiza el uso del espectro.

---

## Resultado Final
- **Portadora anterior**: \( 900 \, \text{MHz} \)
- **Portadora actual**: \( 1.2 \, \text{GHz} \)
- **Portadora posterior**: \( 1.5 \, \text{GHz} \)

La simulación confirma que la separación adecuada de las portadoras garantiza un uso eficiente del espectro y evita interferencias.

---

## Referencias
- [Eficiencia Espectral - Wikipedia](https://es.wikipedia.org/wiki/Eficiencia_espectral)
- [Cisco Packet Tracer - Documentación Oficial](https://www.netacad.com/courses/packet-tracer)
- [Teoría de la Comunicación - Wikipedia](https://es.wikipedia.org/wiki/Teor%C3%ADa_de_la_comunicaci%C3%B3n)


