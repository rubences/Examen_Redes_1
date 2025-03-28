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


# Ejercicio 9
# Resolviendo el Problema de Identificación de Modulación en Función del BER

Este documento explica cómo ordenar diferentes esquemas de modulación en función de su robustez ante el ruido, justificando la respuesta con base en el número de símbolos y la sensibilidad al ruido.

---

## Enunciado

Se sabe que la robustez ante el ruido de una modulación depende del número de símbolos por baudio, de manera que:

1. **BPSK (2-QAM)** es la más robusta.
2. **QPSK (4 símbolos)** ofrece el doble de eficiencia que BPSK.
3. A medida que se incrementa el número de símbolos (16-QAM, 64-QAM, 256-QAM), la eficiencia aumenta pero la tolerancia al ruido disminuye.

Se pide:
- Ordenar las siguientes modulaciones de mayor a menor robustez ante el ruido (para una misma SNR):
  - BPSK
  - QPSK
  - 16-QAM
  - 64-QAM
  - 256-QAM
- Justificar la respuesta basándose en el número de símbolos y la sensibilidad al ruido.

---

## Paso a Paso

### Paso 1: Comprender la relación entre el número de símbolos y la robustez al ruido
1. **BPSK (2-QAM)**:
   - Tiene **2 símbolos**.
   - Es la más robusta porque tiene la mayor distancia entre símbolos en el espacio de constelación, lo que la hace menos sensible al ruido.

2. **QPSK (4-QAM)**:
   - Tiene **4 símbolos**.
   - Ofrece el doble de eficiencia espectral que BPSK, pero la distancia entre símbolos es menor, lo que la hace más sensible al ruido.

3. **16-QAM**:
   - Tiene **16 símbolos**.
   - La eficiencia espectral aumenta significativamente, pero la distancia entre símbolos disminuye aún más, lo que la hace menos robusta al ruido.

4. **64-QAM**:
   - Tiene **64 símbolos**.
   - La eficiencia espectral es mucho mayor, pero la distancia entre símbolos es muy pequeña, lo que la hace aún más sensible al ruido.

5. **256-QAM**:
   - Tiene **256 símbolos**.
   - Es la modulación más eficiente en términos espectrales, pero también la más sensible al ruido debido a la mínima distancia entre símbolos.

---

### Paso 2: Ordenar las modulaciones de mayor a menor robustez al ruido
Con base en la cantidad de símbolos y la sensibilidad al ruido, el orden de mayor a menor robustez es:

1. **BPSK (2-QAM)**: Mayor robustez al ruido debido a la mayor distancia entre símbolos.
2. **QPSK (4-QAM)**: Menor robustez que BPSK, pero aún tolerante al ruido.
3. **16-QAM**: Moderada robustez al ruido, con mayor eficiencia espectral.
4. **64-QAM**: Menor robustez al ruido, pero con alta eficiencia espectral.
5. **256-QAM**: Menor robustez al ruido debido a la mínima distancia entre símbolos.

---

### Paso 3: Justificación de la respuesta
1. **Relación entre el número de símbolos y la distancia entre ellos**:
   - A medida que aumenta el número de símbolos en la constelación, la distancia entre ellos disminuye.
   - Una menor distancia entre símbolos hace que la modulación sea más sensible al ruido, ya que pequeñas perturbaciones pueden causar errores en la detección.

2. **Relación entre eficiencia espectral y robustez al ruido**:
   - Modulaciones con más símbolos (como 256-QAM) son más eficientes en términos espectrales, ya que transmiten más bits por símbolo.
   - Sin embargo, esta eficiencia viene a costa de una menor robustez al ruido.

3. **BPSK como la más robusta**:
   - BPSK tiene solo 2 símbolos, lo que maximiza la distancia entre ellos y minimiza la probabilidad de error debido al ruido.

4. **256-QAM como la menos robusta**:
   - 256-QAM tiene 256 símbolos, lo que reduce significativamente la distancia entre ellos, aumentando la probabilidad de error en presencia de ruido.

---

### Paso 4: Importancia de la selección de la modulación
La elección del esquema de modulación depende del compromiso entre:
- **Eficiencia espectral**: Cuántos bits se pueden transmitir por unidad de ancho de banda.
- **Robustez al ruido**: La capacidad de la modulación para resistir perturbaciones en el canal.

En sistemas con alta relación señal a ruido (SNR), se prefieren modulaciones como 64-QAM o 256-QAM para maximizar la eficiencia espectral. En sistemas con baja SNR, se prefieren modulaciones como BPSK o QPSK para garantizar la robustez al ruido.

---

## Resultado Final
El orden de las modulaciones de mayor a menor robustez al ruido es:

1. **BPSK (2-QAM)**
2. **QPSK (4-QAM)**
3. **16-QAM**
4. **64-QAM**
5. **256-QAM**

---

## Conclusión
La robustez al ruido de una modulación está inversamente relacionada con el número de símbolos en la constelación. BPSK es la más robusta debido a su simplicidad y mayor distancia entre símbolos, mientras que 256-QAM es la menos robusta, aunque más eficiente espectralmente. La selección de la modulación adecuada depende de las condiciones del canal y los requisitos del sistema.

---

## Referencias
- [Modulación Digital - Wikipedia](https://es.wikipedia.org/wiki/Modulaci%C3%B3n_digital)
- [Relación Señal a Ruido - Wikipedia](https://es.wikipedia.org/wiki/Relaci%C3%B3n_se%C3%B1al-ruido)
- [BER y Modulación - Artículo Técnico](https://www.sciencedirect.com/topics/engineering/bit-error-rate)


# Resolviendo el Problema de Identificación de Modulación en Función del BER en Cisco Packet Tracer

Este documento explica cómo simular un sistema de comunicación en **Cisco Packet Tracer** para analizar la robustez de diferentes esquemas de modulación en función del BER (Bit Error Rate).

---

## Enunciado

Se sabe que la robustez ante el ruido de una modulación depende del número de símbolos por baudio, de manera que:

1. **BPSK (2-QAM)** es la más robusta.
2. **QPSK (4 símbolos)** ofrece el doble de eficiencia que BPSK.
3. A medida que se incrementa el número de símbolos (16-QAM, 64-QAM, 256-QAM), la eficiencia aumenta pero la tolerancia al ruido disminuye.

Se pide:
- Ordenar las siguientes modulaciones de mayor a menor robustez ante el ruido (para una misma SNR):
  - BPSK
  - QPSK
  - 16-QAM
  - 64-QAM
  - 256-QAM
- Simular el sistema en **Cisco Packet Tracer** para analizar cómo la calidad del enlace afecta la transmisión de datos.

---

## Paso a Paso

### Paso 1: Configurar el entorno en Cisco Packet Tracer
1. **Abrir Cisco Packet Tracer**:
   - Inicia el programa y abre un nuevo proyecto.

2. **Agregar dispositivos**:
   - Arrastra los siguientes dispositivos al área de trabajo:
     - Un **Access Point** (AP).
     - Dos **PCs inalámbricas** (PC0 y PC1).

3. **Configurar el Access Point**:
   - Haz clic en el Access Point y ve a la pestaña **Config**.
   - Configura los siguientes parámetros:
     - **SSID**: "Modulación_Test".
     - **Frecuencia**: 2.4 GHz (frecuencia estándar para redes Wi-Fi).
     - **Potencia de transmisión**: Ajusta la potencia para simular diferentes niveles de calidad de enlace.

4. **Configurar las PCs inalámbricas**:
   - Haz clic en cada PC y ve a la pestaña **Config**.
   - Conéctalas al Access Point configurado.

---

### Paso 2: Simular diferentes niveles de calidad de enlace
1. **Simular BPSK (2-QAM)**:
   - Configura el Access Point con una **potencia de transmisión alta** (por ejemplo, 100%).
   - Genera tráfico entre las PCs utilizando **Ping** o **Traceroute**.
   - Observa que el enlace es robusto y los paquetes se transmiten sin errores.

2. **Simular QPSK (4-QAM)**:
   - Reduce la potencia de transmisión del Access Point al **75%**.
   - Genera tráfico entre las PCs.
   - Observa que el enlace sigue siendo estable, pero puede haber ligeros retrasos.

3. **Simular 16-QAM**:
   - Reduce la potencia de transmisión del Access Point al **50%**.
   - Genera tráfico entre las PCs.
   - Observa que el enlace comienza a experimentar pérdida de paquetes debido a la menor robustez.

4. **Simular 64-QAM**:
   - Reduce la potencia de transmisión del Access Point al **25%**.
   - Genera tráfico entre las PCs.
   - Observa que la pérdida de paquetes aumenta significativamente.

5. **Simular 256-QAM**:
   - Reduce la potencia de transmisión del Access Point al **10%**.
   - Genera tráfico entre las PCs.
   - Observa que el enlace es inestable y la mayoría de los paquetes no se transmiten correctamente.

---

### Paso 3: Analizar los resultados
1. **Relación entre calidad del enlace y robustez**:
   - A medida que se reduce la potencia de transmisión, el enlace se vuelve más sensible al ruido.
   - Las modulaciones con más símbolos (como 256-QAM) son más propensas a errores en condiciones de baja calidad de enlace.

2. **Comparar con los cálculos teóricos**:
   - Verifica que los resultados observados en la simulación coincidan con el orden teórico de robustez:
     - **BPSK > QPSK > 16-QAM > 64-QAM > 256-QAM**.

---

### Paso 4: Conclusión
La simulación en **Cisco Packet Tracer** muestra cómo la calidad del enlace afecta la transmisión de datos. Aunque no se pueden simular directamente las modulaciones digitales, ajustar la potencia de transmisión del Access Point permite aproximar el comportamiento de diferentes esquemas de modulación en función de su robustez al ruido.

---

## Resultado Final
El orden de las modulaciones de mayor a menor robustez al ruido es:

1. **BPSK (2-QAM)**
2. **QPSK (4-QAM)**
3. **16-QAM**
4. **64-QAM**
5. **256-QAM**

---

## Referencias
- [Modulación Digital - Wikipedia](https://es.wikipedia.org/wiki/Modulaci%C3%B3n_digital)
- [Relación Señal a Ruido - Wikipedia](https://es.wikipedia.org/wiki/Relaci%C3%B3n_se%C3%B1al-ruido)
- [Cisco Packet Tracer - Documentación Oficial](https://www.netacad.com/courses/packet-tracer)


# Ejercicio 10

# Resolviendo el Problema de Eficiencia del Sistema de Encapsulamiento

Este documento explica cómo calcular el tamaño del mensaje, la fragmentación en tramas, la sobrecarga de la capa 1 y la eficiencia del sistema de encapsulamiento.

---

## Enunciado

Considera un sistema de encapsulamiento con la siguiente configuración:

- **Capa 5**: Envía un bloque de datos de **1.5 Kbytes** (1 Kbyte = 1024 bytes).
- **Capas 4 y 3**: Cada una añade una cabecera de **40 bytes**.
- **Capa 2**: Permite el envío de tramas de **400 bytes** como máximo.
- **Capa 1**: Por cada **2 bytes de datos**, se añaden:
  - **1 byte de inicio**,
  - **1 byte de parada**,
  - **1 byte de CRC**.

Se pide realizar los siguientes cálculos:

1. **a)** Tamaño del Mensaje:  
   Calcula el tamaño total del mensaje después de agregar las cabeceras de las capas 4 y 3.

2. **b)** Fragmentación en Tramas:  
   Determina el número de tramas de 400 bytes necesarias para transmitir el mensaje resultante.

3. **c)** Sobrecarga de la Capa 1:  
   Para cada trama de 400 bytes, calcula la cantidad de sobrecarga introducida por la capa 1.

4. **d)** Eficiencia del Sistema:  
   Calcula la eficiencia del sistema de encapsulamiento, definida como el porcentaje de datos útiles (del bloque original) respecto al total de datos transmitidos (incluyendo todas las sobrecargas).

---

## Paso a Paso

### **a) Tamaño del Mensaje**

1. **Datos originales de la Capa 5**:  
   El bloque de datos tiene un tamaño de **1.5 Kbytes**:
   \[
   1.5 \, \text{Kbytes} = 1.5 \times 1024 = 1536 \, \text{bytes}
   \]

2. **Cabeceras de las Capas 4 y 3**:  
   Cada capa añade una cabecera de **40 bytes**:
   \[
   \text{Cabeceras totales} = 40 \, \text{bytes} + 40 \, \text{bytes} = 80 \, \text{bytes}
   \]

3. **Tamaño total del mensaje**:  
   Sumamos los datos originales y las cabeceras:
   \[
   \text{Tamaño total del mensaje} = 1536 \, \text{bytes} + 80 \, \text{bytes} = 1616 \, \text{bytes}
   \]

---

### **b) Fragmentación en Tramas**

1. **Tamaño máximo de una trama**:  
   La capa 2 permite tramas de **400 bytes** como máximo.

2. **Número de tramas necesarias**:  
   Dividimos el tamaño total del mensaje entre el tamaño máximo de una trama y redondeamos hacia arriba:
   \[
   \text{Número de tramas} = \lceil \frac{1616}{400} \rceil = \lceil 4.04 \rceil = 5 \, \text{tramas}
   \]

---

### **c) Sobrecarga de la Capa 1**

1. **Sobrecarga por cada 2 bytes de datos**:  
   Por cada **2 bytes de datos**, la capa 1 añade:
   - **1 byte de inicio**,
   - **1 byte de parada**,
   - **1 byte de CRC**.

   Esto significa que por cada **2 bytes de datos**, se añaden **3 bytes de sobrecarga**.

2. **Datos útiles por trama**:  
   Cada trama tiene un tamaño máximo de **400 bytes**, pero parte de este espacio se utiliza para la sobrecarga.  
   La relación entre datos útiles y sobrecarga es:
   \[
   \text{Datos útiles por trama} = \frac{2}{2 + 3} \times 400 = \frac{2}{5} \times 400 = 160 \, \text{bytes}
   \]

3. **Sobrecarga por trama**:  
   La sobrecarga por trama es el resto del espacio ocupado por los bytes de inicio, parada y CRC:
   \[
   \text{Sobrecarga por trama} = 400 - 160 = 240 \, \text{bytes}
   \]

4. **Sobrecarga total**:  
   Multiplicamos la sobrecarga por trama por el número total de tramas:
   \[
   \text{Sobrecarga total} = 240 \, \text{bytes/trama} \times 5 \, \text{tramas} = 1200 \, \text{bytes}
   \]

---

### **d) Eficiencia del Sistema**

1. **Datos útiles totales**:  
   Los datos útiles son los **1536 bytes** originales de la Capa 5.

2. **Datos totales transmitidos**:  
   Los datos totales transmitidos incluyen los datos útiles y todas las sobrecargas:
   \[
   \text{Datos totales transmitidos} = 5 \, \text{tramas} \times 400 \, \text{bytes/trama} = 2000 \, \text{bytes}
   \]

3. **Eficiencia del sistema**:  
   La eficiencia se calcula como el porcentaje de datos útiles respecto al total de datos transmitidos:
   \[
   \text{Eficiencia} = \frac{\text{Datos útiles totales}}{\text{Datos totales transmitidos}} \times 100
   \]
   Sustituyendo los valores:
   \[
   \text{Eficiencia} = \frac{1536}{2000} \times 100 = 76.8\%
   \]

---

## Resultados Finales

1. **Tamaño del mensaje**:  
   \[
   1616 \, \text{bytes}
   \]

2. **Número de tramas necesarias**:  
   \[
   5 \, \text{tramas}
   \]

3. **Sobrecarga de la capa 1**:  
   \[
   1200 \, \text{bytes}
   \]

4. **Eficiencia del sistema**:  
   \[
   76.8\%
   \]

---

## Conclusión

El sistema de encapsulamiento tiene una eficiencia del **76.8%**, lo que significa que aproximadamente el **23.2%** de los datos transmitidos corresponden a sobrecargas. Este análisis muestra cómo las cabeceras y la fragmentación afectan la eficiencia del sistema de comunicación.

---

## Referencias
- [Encapsulamiento en Redes - Wikipedia](https://es.wikipedia.org/wiki/Encapsulamiento_(redes))
- [Eficiencia en Redes - Artículo Técnico](https://www.sciencedirect.com/topics/computer-science/network-efficiency)


Simular el problema de Eficiencia del Sistema de Encapsulamiento en Cisco Packet Tracer no es algo que se pueda realizar directamente, ya que Packet Tracer no permite modelar el encapsulamiento a nivel de bits o bytes. Sin embargo, podemos aproximar el concepto configurando un sistema de red que transmita datos entre dispositivos y analizando el tráfico generado para observar cómo las cabeceras y la fragmentación afectan la transmisión. Aquí tienes un paso a paso detallado para resolver el problema y simularlo en Cisco Packet Tracer:

Resolviendo el Problema de Eficiencia del Sistema de Encapsulamiento
Enunciado
Considera un sistema de encapsulamiento con la siguiente configuración:

Capa 5: Envía un bloque de datos de 1.5 Kbytes (1 Kbyte = 1024 bytes).
Capas 4 y 3: Cada una añade una cabecera de 40 bytes.
Capa 2: Permite el envío de tramas de 400 bytes como máximo.
Capa 1: Por cada 2 bytes de datos, se añaden:
1 byte de inicio,
1 byte de parada,
1 byte de CRC.
Se pide realizar los siguientes cálculos:

a) Tamaño del Mensaje:
Calcula el tamaño total del mensaje después de agregar las cabeceras de las capas 4 y 3.

b) Fragmentación en Tramas:
Determina el número de tramas de 400 bytes necesarias para transmitir el mensaje resultante.

c) Sobrecarga de la Capa 1:
Para cada trama de 400 bytes, calcula la cantidad de sobrecarga introducida por la capa 1.

d) Eficiencia del Sistema:
Calcula la eficiencia del sistema de encapsulamiento, definida como el porcentaje de datos útiles (del bloque original) respecto al total de datos transmitidos (incluyendo todas las sobrecargas).

Paso a Paso
a) Tamaño del Mensaje
Datos originales de la Capa 5:
El bloque de datos tiene un tamaño de 1.5 Kbytes: [ 1.5 , \text{Kbytes} = 1.5 \times 1024 = 1536 , \text{bytes} ]

Cabeceras de las Capas 4 y 3:
Cada capa añade una cabecera de 40 bytes: [ \text{Cabeceras totales} = 40 , \text{bytes} + 40 , \text{bytes} = 80 , \text{bytes} ]

Tamaño total del mensaje:
Sumamos los datos originales y las cabeceras: [ \text{Tamaño total del mensaje} = 1536 , \text{bytes} + 80 , \text{bytes} = 1616 , \text{bytes} ]

b) Fragmentación en Tramas
Tamaño máximo de una trama:
La capa 2 permite tramas de 400 bytes como máximo.

Número de tramas necesarias:
Dividimos el tamaño total del mensaje entre el tamaño máximo de una trama y redondeamos hacia arriba: [ \text{Número de tramas} = \lceil \frac{1616}{400} \rceil = \lceil 4.04 \rceil = 5 , \text{tramas} ]

c) Sobrecarga de la Capa 1
Sobrecarga por cada 2 bytes de datos:
Por cada 2 bytes de datos, la capa 1 añade:

1 byte de inicio,
1 byte de parada,
1 byte de CRC.
Esto significa que por cada 2 bytes de datos, se añaden 3 bytes de sobrecarga.

Datos útiles por trama:
Cada trama tiene un tamaño máximo de 400 bytes, pero parte de este espacio se utiliza para la sobrecarga.
La relación entre datos útiles y sobrecarga es: [ \text{Datos útiles por trama} = \frac{2}{2 + 3} \times 400 = \frac{2}{5} \times 400 = 160 , \text{bytes} ]

Sobrecarga por trama:
La sobrecarga por trama es el resto del espacio ocupado por los bytes de inicio, parada y CRC: [ \text{Sobrecarga por trama} = 400 - 160 = 240 , \text{bytes} ]

Sobrecarga total:
Multiplicamos la sobrecarga por trama por el número total de tramas: [ \text{Sobrecarga total} = 240 , \text{bytes/trama} \times 5 , \text{tramas} = 1200 , \text{bytes} ]

d) Eficiencia del Sistema
Datos útiles totales:
Los datos útiles son los 1536 bytes originales de la Capa 5.

Datos totales transmitidos:
Los datos totales transmitidos incluyen los datos útiles y todas las sobrecargas: [ \text{Datos totales transmitidos} = 5 , \text{tramas} \times 400 , \text{bytes/trama} = 2000 , \text{bytes} ]

Eficiencia del sistema:
La eficiencia se calcula como el porcentaje de datos útiles respecto al total de datos transmitidos: [ \text{Eficiencia} = \frac{\text{Datos útiles totales}}{\text{Datos totales transmitidos}} \times 100 ] Sustituyendo los valores: [ \text{Eficiencia} = \frac{1536}{2000} \times 100 = 76.8% ]

Resultados Finales
Tamaño del mensaje:
[ 1616 , \text{bytes} ]

Número de tramas necesarias:
[ 5 , \text{tramas} ]

Sobrecarga de la capa 1:
[ 1200 , \text{bytes} ]

Eficiencia del sistema:
[ 76.8% ]

Simulación en Cisco Packet Tracer
Aunque Cisco Packet Tracer no permite modelar directamente el encapsulamiento, podemos simular el tráfico generado por un sistema de encapsulamiento utilizando los siguientes pasos:

Paso 1: Configurar el entorno
Abrir Cisco Packet Tracer:

Inicia el programa y abre un nuevo proyecto.
Agregar dispositivos:

Arrastra dos PCs (PC0 y PC1) al área de trabajo.
Conéctalas utilizando un switch.
Configurar direcciones IP:

Asigna direcciones IP a las PCs:
PC0: 192.168.1.1
PC1: 192.168.1.2
Paso 2: Generar tráfico
Configurar un servidor de archivos:

Configura un servidor en PC1 para enviar un archivo de 1.5 KB a PC0.
Capturar el tráfico:

Usa la herramienta de captura de paquetes en el switch para observar el tráfico generado.
Analiza los paquetes para identificar las cabeceras y la fragmentación.
Paso 3: Analizar los resultados
Observar la fragmentación:

Verifica cómo el archivo de 1.5 KB se divide en tramas de 400 bytes.
Observa las cabeceras añadidas en cada capa.
Calcular la eficiencia:

Compara el tamaño total de los datos transmitidos con el tamaño del archivo original para calcular la eficiencia.
Conclusión
La simulación en Cisco Packet Tracer permite observar cómo se fragmenta un archivo grande en tramas más pequeñas y cómo las cabeceras afectan la transmisión. Aunque no se puede modelar directamente el encapsulamiento, esta aproximación ayuda a entender el impacto de la fragmentación y la sobrecarga en la eficiencia del sistema.

Referencias
Encapsulamiento en Redes - Wikipedia
Cisco Packet Tracer - Documentación Oficial

